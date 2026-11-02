# AxureForge CLI

通过命令行创建、读取和编辑 Axure `.rp` 原型文件，包括页面、元件、交互及 HTML 导入。
这是二进制发行仓库，仅提供 CLI 下载、使用说明和许可证；不包含项目源码、构建脚本或内部验证数据。

## 下载与安装

在本仓库的 **Releases** 页面下载对应系统和 CPU 架构的压缩包及 `SHA256SUMS`。
运行无需安装 Python 或 uv。当前首个发行提供 macOS ARM64（Apple Silicon）产物；
Linux x64、Windows x64 产物将在各平台构建验证后提供。

macOS：

```bash
shasum -a 256 -c SHA256SUMS
tar -xzf axure-forge-0.2.0-macos-arm64.tar.gz
cd axure-forge-0.2.0-macos-arm64
./axure-forge --version
./axure-forge --help
```

校验文件和压缩包应放在同一目录。也可以将可执行文件复制到自己的 PATH 目录。
macOS 产物未经开发者签名或公证，系统可能要求允许执行；请仅在确认下载来源和校验值后操作。
程序启动时需要可写且允许执行的系统临时目录。当前产物仍处于早期版本，建议用项目副本操作。

## 快速开始

在可执行文件所在目录运行：

```bash
./axure-forge project create --name Demo --output demo.rp
./axure-forge page list --project demo.rp
./axure-forge search explore --query 输入框 --category template
./axure-forge format list
```

从 `page list` 的 JSON 结果取得 `scope_id` 后创建元件：

```bash
./axure-forge node create --project demo.rp --scope-id YOUR_SCOPE_ID \
  --spec '{"kind":"text","text":"Hello Axure"}' --output edited.rp
```

HTML 导入：

```bash
./axure-forge html import --project demo.rp \
  --html '<h1>Hello Axure</h1><p>Editable prototype</p>' \
  --page-name HTML --output imported.rp
```

编辑命令需要 `--output`；已有输出文件默认受保护，确认覆盖时使用 `--force`。
正常结果以 JSON 写入 stdout，运行错误同时写入 stderr。退出码：成功 `0`、执行或文件错误 `1`、参数校验错误 `2`。
写出目标为 Axure RP 9；结构验证不代表所有原生编辑器与交互组合均已验收。

## 命令帮助

```bash
./axure-forge --help
./axure-forge node --help
./axure-forge node create --help
```

## 许可证

AxureForge 按 [MIT License](LICENSE) 分发。程序同时包含 Python 运行时和其他运行组件，
适用的第三方许可证随发行包提供。AxureForge 是独立项目，不隶属于 Axure。
