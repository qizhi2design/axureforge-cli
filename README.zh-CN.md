<p align="center">
  <a href="README.md">English</a> · <b>简体中文</b>
</p>

<p align="center">
  <img src="docs/images/banner.jpg" alt="AxureForge CLI —— 批量改原型，不用一个个点" width="100%">
</p>

<h1 align="center">AxureForge CLI</h1>

<p align="center"><b>批量改原型，不用一个个点。</b></p>
<p align="center">
  创建、读取和修改 Axure RP9 / RP11 原型文件（<code>.rp</code>）<br>
  建页面、加元件、改文案、导网页、转版本，一条命令做完。
</p>

<p align="center">
  <img alt="支持 Apple 芯片 Mac" src="https://img.shields.io/badge/macOS-Apple%20Silicon-000000?logo=apple&logoColor=white">
  <img alt="支持 Linux 64 位" src="https://img.shields.io/badge/Linux-x64-FCC624?logo=linux&logoColor=black">
  <img alt="支持 Windows 64 位" src="https://img.shields.io/badge/Windows-x64-0078D4?logo=windows&logoColor=white">
  <img alt="当前版本" src="https://img.shields.io/github/v/release/qizhi2design/axureforge-cli?color=0A7AFF">
  <img alt="许可证 MIT" src="https://img.shields.io/badge/license-MIT-22C55E">
</p>

<p align="center">
  <img alt="支持 RP9 与 RP11" src="https://img.shields.io/badge/RP9%20%2F%20RP11-22D3EE?style=flat-square">
  <img alt="HTML 导入" src="https://img.shields.io/badge/HTML%E5%AF%BC%E5%85%A5-22D3EE?style=flat-square">
  <img alt="批量修改" src="https://img.shields.io/badge/%E6%89%B9%E9%87%8F%E4%BF%AE%E6%94%B9-22D3EE?style=flat-square">
  <img alt="严格转换" src="https://img.shields.io/badge/%E4%B8%A5%E6%A0%BC%E8%BD%AC%E6%8D%A2-22D3EE?style=flat-square">
</p>

<p align="center">
  <a href="#能做什么">能做什么</a> ·
  <a href="#下载与安装">下载与安装</a> ·
  <a href="#三分钟上手">三分钟上手</a> ·
  <a href="#常用操作">常用操作</a> ·
  <a href="#进阶能力">进阶能力</a> ·
  <a href="#常见问题">常见问题</a> ·
  <a href="#适用范围与限制">适用范围</a> ·
  <a href="#更新与版本">更新与版本</a> ·
  <a href="#许可与合规">许可与合规</a>
</p>

## 能做什么

- 🆕 从零新建 RP9 或 RP11 原型，直接开始画。
- 🧩 30 个命令组、155 条命令，覆盖页面与页面树、元件、动态面板、中继器、表格、树、菜单、母版与母版树、自适应视图、连接线、交互与交互样式、表达式、元件库、分组、框架、文件夹、检索、格式与批量。
- 🌐 把现成网页一次性导入，自动完成布局，生成可编辑的页面。
- 🔍 `dump` 生成索引，之后在本地查页面和元件，不用反复打开原型。
- ⚡ 批量修改一次提交，要么全部成功，要么全部不生效。
- 🔄 RP9 与 RP11 严格互转，先预检再转换。
- ✅ 不打开 Axure 界面，也能检查文件结构、估算布局。

想直接用中文提需求，可以配合 [axure-forge-skill](https://github.com/qizhi2design/axure-forge-skill) 使用。

## 下载与安装

AxureForge 以目录包分发，下载解压就能用。**必须保留整个目录和 `_internal`**，只复制可执行文件会启动失败。

1. 打开[下载页](https://github.com/qizhi2design/axureforge-cli/releases)，下载对应平台的压缩包和 `SHA256SUMS`。
2. 把两个文件放在同一个文件夹，先校验，再解压。
3. 进入解压后的目录，运行 `--version` 确认可用。

下面以 Apple 芯片 Mac 的 0.3.0 为例；Linux 和 Windows 换成对应平台的压缩包，步骤相同。

```bash
shasum -a 256 -c SHA256SUMS
tar -xzf axure-forge-0.3.0-macos-arm64.tar.gz
cd axure-forge-0.3.0-macos-arm64
./axure-forge --version
./axure-forge --help
```

- 第 1 行：核对下载的文件是否完整，没损坏才算下载成功。
- 第 2 行：解压压缩包。
- 第 3 行：进入解压出来的文件夹。
- 第 4 行：显示版本号，能显示出来就说明程序可用。
- 第 5 行：列出程序支持的所有命令。

可以把整个目录移动到固定位置，再为里面的可执行文件创建命令入口；macOS 也可以使用 skill 的安装脚本自动完成校验和部署。

## 三分钟上手

准备一个原型文件，放在当前目录，下面统一用 `demo.rp` 指代。还没有的话，先用下一节的 `project create` 建一个空文件。

先看看它能做什么：

```bash
./axure-forge capabilities --json
./axure-forge dump --project demo.rp
./axure-forge verify --project demo.rp
```

- `capabilities --json`：一次列出全部命令组、命令、参数、支持的版本和已知限制。
- `dump --project demo.rp`：在 `.forge/index` 生成索引，把页面和元件整理成可查询的清单。
- `verify --project demo.rp`：不打开界面，检查文件结构并估算布局；视觉与交互不在检查范围。

三条命令都不会修改 `demo.rp`。

## 常用操作

**新建一个原型，然后看页面列表：**

```bash
./axure-forge project create --name Demo --output demo.rp
./axure-forge page list --project demo.rp
```

- 第 1 行：新建名为 Demo 的原型，保存为 `demo.rp`；默认 RP9，要 RP11 就加 `--format-version 11`。
- 第 2 行：列出文件里的页面，记下页面编号（`scope_id`）。

**找模板和格式：**

```bash
./axure-forge search explore --query 输入框 --category template
./axure-forge format list
```

- 第 1 行：在内置模板里搜索「输入框」，看看哪些可以直接用。
- 第 2 行：查看程序认识的格式和元件清单。

**加一个元件：**

先用 `page list` 找到页面编号，替换下面的 `YOUR_SCOPE_ID`。

```bash
./axure-forge node create --project demo.rp --scope-id YOUR_SCOPE_ID \
  --spec '{"kind":"text","text":"Hello Axure"}' --output edited.rp
```

这条命令往该页面加一段文字，结果另存为 `edited.rp`。

**把网页转成页面：**

```bash
./axure-forge html import --project demo.rp \
  --html '<h1>Hello Axure</h1><p>可编辑原型</p>' \
  --page-name HTML --page-size 1440x900 --output imported.rp
```

这段网页会变成一个叫 `HTML` 的新页面：宽度固定 1440，高度不低于 900 并随内容延展，结果另存为 `imported.rp`。

**改文件必须指定输出文件。** 会生成新文件的命令都要带 `--output`。

**默认不覆盖。** 目标文件已存在时命令会停下；确认覆盖再加 `--force`。

## 进阶能力

<details>
<summary><b>工作目录与证据</b></summary>

默认工作目录是当前目录下的 `.forge/`，可用 `--work-dir DIR` 改。
索引、布局计划、校验报告和摘要都写在这里。

`html import` 和 `batch` 完成后会生成 `.forge/summary.json`；先读它拿到输出文件、索引和报告的路径，再按需看详情。

`dump` 负责生成索引；`verify` 可以检查原型，也可以直接检查已有索引。
写入类命令带 `--index` 时，会先核对源文件哈希；源文件变过就拒绝执行。

```bash
./axure-forge dump --project demo.rp --work-dir .forge
./axure-forge verify --index .forge/index
```

第二条命令直接读索引，不再解析原型。

</details>

<details>
<summary><b>HTML 导入能力与限制</b></summary>

支持的布局有 5 种：block、inline、flex、table、absolute。

限制：

- 不执行 JavaScript。
- 不加载远程资源，也不读取外部样式表。
- 不支持 CSS grid。
- 文字宽度是估算值。
- 不做 GUI 渲染。

`--page-size 1440x900` 固定宽度 1440，高度以 900 为下限随内容延展。
`--page-mode fixed` 改成固定宽高，`auto` 是默认值。
新建文件时用 `--format-version 9` 或 `--format-version 11` 指定格式。

`--plan` 可以复用已经算好的布局：

```bash
./axure-forge html plan ./site --page-size 1440x900 --output plan.json
./axure-forge html import ./site --page-size 1440x900 --plan plan.json --output imported.rp
```

`html plan` 只计算布局，不生成原型；输入或实际资源变了，计划会失效，需要重新生成。

</details>

<details>
<summary><b>批量与结果引用</b></summary>

一次 `batch` 提交多条修改：要么全部成功，要么全部不生效。
失败不保留中间结果，也不生成目标文件。

每个操作可以用 `as` 起别名，后续步骤用 `{"$ref":"别名.字段"}` 引用前一步结果。
比如刚建好一个页面，下一步直接引用它的 `scope_id`，不用再查一次。

```bash
./axure-forge batch ops.json --project demo.rp --index .forge/index --output batched.rp
```

`ops.json` 是批量请求文件，写法见[批量与验证](https://github.com/qizhi2design/axure-forge-skill/blob/main/skills/axure-forge/references/batch-and-verify.md)。
引用只能指向前面已成功的步骤；缺字段、重复别名都会报错。

</details>

<details>
<summary><b>格式与严格转换</b></summary>

RP9 和 RP11 都支持读取、编辑和写入，两个版本之间可以互转，策略是 `strict_lossless`。
转换前必须先预检，确认没有阻断项再执行：

```bash
./axure-forge project check-conversion --project demo.rp --target-version 11
./axure-forge project convert --project demo.rp --target-version 11 --output demo11.rp
```

`check-conversion` 只读，不改源文件；不兼容或未验证的数据会阻断转换。
`convert` 生成独立的新文件，源文件保持不变；未识别的数据会原样保留，不会被猜着解释。
反向转换同理，把 `--target-version` 改成 `9`。
打开旧版本文件不会自动升版本，要换版本就显式转换。

</details>

## 常见问题

<details>
<summary><b>Mac 第一次打开被系统拦下了？</b></summary>

程序没有经过 Apple 的开发者验证，请到「系统设置 → 隐私与安全性」里允许。
确认下载来源和 `SHA256SUMS` 校验无误后再允许。

</details>

<details>
<summary><b>启动失败，提示临时目录不可用？</b></summary>

0.3.0 使用目录包。请确认整个目录和 `_internal` 都在，程序文件有执行权限。

</details>

<details>
<summary><b>下载后 `_internal` 缺失，或只复制了单个程序？</b></summary>

重新解压压缩包，保留完整目录再运行。不能只拿 `axure-forge` 这一个文件。

</details>

<details>
<summary><b>没有装 Axure 编辑器能用吗？</b></summary>

能。新建、读取、编辑、导入网页、转换和校验都不需要编辑器。
视觉和交互验收仍需在 Axure 里打开确认。

</details>

<details>
<summary><b>担心把原型改坏了？</b></summary>

先复制一份原型再操作，看过结果没问题再替换正式文件。

</details>

<details>
<summary><b>改完的文件在哪？</b></summary>

由 `--output` 指定；不指定不会生成新文件。

</details>

<details>
<summary><b>已有同名文件会被覆盖吗？</b></summary>

默认不会，命令会停下提示；确认覆盖要加 `--force`。

</details>

<details>
<summary><b>想看某个命令怎么用？</b></summary>

在命令后加 `--help`，例如：

```bash
./axure-forge --help
./axure-forge node --help
./axure-forge node create --help
```

</details>

## 适用范围与限制

- 提供 Apple 芯片 Mac、Linux 64 位（Ubuntu 22.04）和 Windows 64 位版本。
- 支持 Axure RP9 和 RP11 的读取、编辑与写入，两个版本之间可以严格转换。
- HTML 导入只覆盖已实现的布局规则；JavaScript、远程资源、外部样式表和 CSS grid 都不在范围内。
- 自动检查只核对文件结构和估算布局，不能代替视觉与交互验收。
- 程序不做 GUI 渲染，最终效果以在 Axure 中打开为准。

退出码：`0` 成功，`1` 执行或校验失败，`2` 参数或输入非法。

## 更新与版本

当前发布版本是 0.3.0，还没有命令行自更新。

升级方式：重新下载整个目录包，解压后替换旧目录；macOS 也可以用 skill 的安装脚本完成校验和替换。
覆盖前先备份旧目录和原型。

`update` 和 `config` 命令会随下一个版本提供，参数与离线行为见[更新说明](docs/updates.md)。

## 许可与合规

AxureForge 采用 [MIT License](LICENSE)。

第三方组件的许可证文本随包提供，仓库内的说明见 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)。

本项目与 Axure 官方无关。
