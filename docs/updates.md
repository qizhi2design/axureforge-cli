# CLI 与 Skill 更新

更新代码位于 CLI 适配层，仅使用 Python 标准库。`config`、`update` 和元数据查询均不加载 RP 核心功能。

## 使用

```bash
axure-forge update check
axure-forge update check --json
axure-forge update cli
axure-forge update skill --path /ABS/skills/axure-forge
axure-forge update all --dry-run
axure-forge update all --yes
axure-forge update cli --version 0.4.0 --yes
```

裸 `update` 在终端展示检测与选择引导；显式 `update check` 不询问。非交互安装必须带 `--yes`。`--force` 允许重装同版本、覆盖本地修改或未知基线的 skill，替换前保留完整备份。降级另需 `--allow-downgrade`。

CLI 支持 macOS ARM64、Linux x64 和 Windows x64。skill 按其 `platforms` 声明判断，目前仅 macOS ARM64。检测共享 `.agents/skills`、Codex 与 Claude 的用户级及当前目录安装，按真实路径去重；多份独立安装需用 `--path` 选择。

二进制下载、SHA256、目录结构、版本及协议能力验证全部通过后才切换稳定入口；保留旧版本。手动解压包迁移到用户级稳定入口，原包保留，终端输出 PATH 引导。pip、uv tool 和源码安装给出原安装方式升级指引。组合更新先暂存全部产物，再切换，后一步失败恢复之前的组件。

Windows 使用 `.cmd` 稳定入口和独立更新进程。父进程退出后才切换，初始结果为 `submitted`，最终状态由 `update check` 返回。辅助进程的临时目录会保留，最终状态文件会记录其位置；确认辅助进程退出后可删除。安装锁位于用户配置目录，异常强制终止后需先确认无更新进程，再按提示删除残留锁。

## 离线行为

- 普通命令使用本地安装，离线不影响功能。交互终端每 24 小时至多检查一次，新增等待上限一秒；网络失败静默跳过并记录尝试时间。
- 非交互、JSON 调用、`--version`、`--help`、`capabilities` 不自动联网。`AXURE_FORGE_NO_UPDATE_CHECK=1` 也可关闭自动检查。
- 手动检查断网时返回 `ok: true`、`check_status: unavailable`、退出码 0；有历史缓存则给出最后成功检查时间。不会将无法检查称为“已是最新版”。
- 手动更新遇到断网或下载中断时返回 `update_status: not_applied`、退出码 0，旧安装保持可用；临时下载清理。
- 校验失败、非法参数、权限问题和损坏发布清单属于真实错误，返回非零退出码，且不输出异常堆栈。

## 来源配置

```bash
axure-forge config show
axure-forge config set sources.cli.repo qizhi2design/axureforge-cli
axure-forge config set sources.skill.repo qizhi2design/axure-forge-skill
axure-forge config set sources.cli.mirror-prefix https://mirror.example/
axure-forge config reset sources.cli
axure-forge config set updates.auto-check false
axure-forge update check --component cli --repo owner/repo
```

优先级为单次 `--repo` / `--mirror-prefix`、环境变量、配置、默认值。环境变量为 `AXURE_FORGE_CLI_REPO`、`AXURE_FORGE_CLI_MIRROR_PREFIX`，skill 将 `CLI` 替换成 `SKILL`。镜像请求采用“HTTPS 前缀 + 完整上游 URL”，代理 GitHub API 和资源下载。不静默回退其他仓库。

`update all` 使用两组件各自配置，不接受单个来源覆盖。`check` 单次来源覆盖必须通过 `--component cli|skill` 明确组件。清空镜像可使用 `config set sources.cli.mirror-prefix ''`。

配置和缓存位于系统用户目录，不写项目 `.forge/`：macOS 使用 `~/Library/Application Support/axure-forge` 和 `~/Library/Caches/axure-forge`；Linux 使用 XDG config/cache；Windows 使用 `%LOCALAPPDATA%/AxureForge/config` 和 `cache`。缓存按来源、组件、平台区分。

## 发布契约

CLI 与 skill 的正式 Release 都需要三个部分：`release-manifest.json`、`SHA256SUMS`、完整压缩包。清单格式版本为 1，包含 `component`、`version`、`protocol_version`、`assets`；asset 按 CLI 平台或 `skill` 键存储 `filename` 和 `sha256`。

skill 清单另含 `cli_min_version`、可空的 `cli_max_version`（不包含上限）及 `platforms`。包内 `skill-manifest.json` 同时记录名称和全部受管文件哈希，校验时拒绝缺失、额外文件及链接。旧安装没有清单时报告未知，不猜测版本。GitHub Release 中的 draft、prerelease 和非 X.Y.Z 标签不参与选择。

本次源码增加了更新能力，尚未发布新版。不要覆盖已有 0.3.0 Release；正式发布前递增包版本和 skill 版本。

1. 保持 core / cli / mcp 的包版本与依赖一致，运行现有构建、协议和业务检查。
2. 三个平台各运行 `scripts/build_binary.py`、`scripts/verify_binary.py`、`scripts/verify_workflow.py`、`scripts/verify_update_binary.py` 和 `scripts/package_binary.py TARGET`。
3. 使用 `python3 scripts/prepare_release.py PLATFORM_DIR... --output dist/combined-release` 合并三平台包。脚本拒绝版本不一致、缺少平台或哈希错误；输出目录必须不存在。
4. CI 的 `combined-release` artifact 包含可一起发布的压缩包、清单与校验文件。将全部资源发布到 `qizhi2design/axureforge-cli` 的对应新正式 Release，不覆盖既有资源。
5. 再按 skill 仓库 `docs/releasing.md` 发布兼容 skill。仓库 tag、skill 内容和生成清单必须一致。

历史 Release 缺少更新清单时返回 `metadata_missing`；不会假装能安全升级。先发布第一个含清单的新版后，后续版本才能通过此机制发现与更新。
