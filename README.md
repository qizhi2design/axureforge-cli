<p align="center">
  <img src="docs/images/banner.jpg" alt="AxureForge CLI —— 批量改原型，不用一个个点" width="100%">
</p>

<h1 align="center">AxureForge CLI</h1>

<p align="center"><b>批量改原型，不用一个个点。</b></p>
<p align="center">
  创建、读取和修改 Axure RP9 原型文件（<code>.rp</code>）<br>
  建页面、加元件、改文案、导入网页，都能一次做完。
</p>

<p align="center">
  <img alt="支持 Apple 芯片 Mac" src="https://img.shields.io/badge/macOS-Apple%20Silicon-000000?logo=apple&logoColor=white">
  <img alt="支持 Linux 64 位" src="https://img.shields.io/badge/Linux-x64-FCC624?logo=linux&logoColor=black">
  <img alt="支持 Windows 64 位" src="https://img.shields.io/badge/Windows-x64-0078D4?logo=windows&logoColor=white">
  <img alt="当前版本" src="https://img.shields.io/github/v/release/qizhi2design/axureforge-cli?color=0A7AFF">
  <img alt="许可证 MIT" src="https://img.shields.io/badge/license-MIT-22C55E">
</p>

<p align="center">
  <img alt="新建原型" src="https://img.shields.io/badge/%E6%96%B0%E5%BB%BA%E5%8E%9F%E5%9E%8B-22D3EE?style=flat-square">
  <img alt="批量修改" src="https://img.shields.io/badge/%E6%89%B9%E9%87%8F%E4%BF%AE%E6%94%B9-22D3EE?style=flat-square">
  <img alt="HTML 导入" src="https://img.shields.io/badge/HTML%E5%AF%BC%E5%85%A5-22D3EE?style=flat-square">
  <img alt="模板搜索" src="https://img.shields.io/badge/%E6%A8%A1%E6%9D%BF%E6%90%9C%E7%B4%A2-22D3EE?style=flat-square">
</p>

<p align="center">
  <a href="#能做什么">能做什么</a> ·
  <a href="#下载与安装">下载与安装</a> ·
  <a href="#快速上手">快速上手</a> ·
  <a href="#常见问题">常见问题</a>
</p>

## 能做什么

- 🆕 从零新建一个 RP9 原型文件，直接开始画。
- 🧩 往指定页面里添加文本、按钮、输入框等元件。
- ⚡ 批量修改元件文案和属性，不用一个个点。
- 🌐 把现成的网页（HTML）转成可编辑的原型页面。
- 🔍 查询内置的格式模板和元件，快速找到能用的东西。

想直接用中文提需求、不用记命令，可以配合 [axure-forge-skill](https://github.com/qizhi2design/axure-forge-skill) 使用。

## 下载与安装

1. 打开本项目的下载页，下载压缩包和校验文件。
2. 把这两个文件放在同一个文件夹里，先校验，再解压。
3. 进入解压出来的文件夹运行，能看到版本号就说明可用。

下载解压后即可使用，不用另外安装运行环境。请保留整个目录及 `_internal`，不能只复制可执行文件。
下面以 Apple 芯片的 Mac、最新版本 0.3.0 为例；Linux 和 Windows 下载各自的压缩包，步骤一样。
文件名按你实际下载到的版本替换即可。

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

可把整个目录移动到固定位置，再为其中的可执行文件创建命令入口；macOS 可使用 skill 的安装脚本自动完成校验和部署。

## 快速上手

在解压出来的文件夹里运行下面几条，先把主要功能走一遍。

```bash
./axure-forge project create --name Demo --output demo.rp
./axure-forge page list --project demo.rp
./axure-forge search explore --query 输入框 --category template
./axure-forge format list
```

- 第 1 行：新建一个叫 Demo 的原型文件，保存成 `demo.rp`。
- 第 2 行：列出这个文件里有哪些页面。
- 第 3 行：在内置模板里搜索「输入框」，看看哪些可以直接用。
- 第 4 行：查看程序认识的格式和元件清单。

往页面上加一个元件。先用第 2 条命令找到页面编号（`scope_id`），再填到下面：

```bash
./axure-forge node create --project demo.rp --scope-id YOUR_SCOPE_ID \
  --spec '{"kind":"text","text":"Hello Axure"}' --output edited.rp
```

这条命令往那个页面里加一段文字，结果另存为 `edited.rp`。

把网页转成原型：

```bash
./axure-forge html import --project demo.rp \
  --html '<h1>Hello Axure</h1><p>Editable prototype</p>' \
  --page-name HTML --output imported.rp
```

这条命令把这段网页内容转成一个叫 HTML 的新页面，另存为 `imported.rp`。

**改文件必须指定输出文件。** 会生成新文件的命令都要带 `--output`。

**默认不覆盖。** 输出文件已存在时命令会停下来提示；确认要覆盖时再加 `--force`。

## 0.3 工作目录与批量执行

```bash
./axure-forge capabilities --json
./axure-forge html import ./site --page-size 1440x900 --output imported.rp --verify
./axure-forge dump --project imported.rp
./axure-forge verify --index .forge/index
```

生成的数据位于当前工作目录 `.forge/`，可用 `--work-dir DIR` 指定。先读取 `summary.json`，按需查看计划、索引和报告。
HTML 自动缓存布局，支持 `html plan` 和 `html import --plan FILE`；输入或资源变化会使计划失效。
宽度固定、高度自动延展；固定画布用 `--page-mode fixed`。batch 支持 `as` 与 `{"$ref":"alias.field"}` 引用前一步结果。
自动检查区分结构和布局估算，视觉、交互仍需在 Axure 中验收。

## 常见问题

<details>
<summary><b>Mac 第一次打开被系统拦下了？</b></summary>

程序没经过 Apple 的开发者验证，请自己到「系统设置 → 隐私与安全性」里允许。
确认下载来源和校验文件无误后再允许。

</details>

<details>
<summary><b>启动失败，提示临时目录不可用？</b></summary>

0.3.0 默认使用目录包。请检查整个目录及 `_internal` 是否完整，以及文件是否允许执行。

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

默认不会，会停下来提示；确认覆盖要加 `--force`。

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

## 适用范围

- 目前提供 Apple 芯片的 Mac（M 系列芯片）、Linux 64 位（Ubuntu 22.04）和 Windows 64 位版本。
- 只面向 Axure RP9，生成的文件也是 RP9 格式。
- 更高版本的 Axure 文件只读取，不转换。
- 网页转换只覆盖程序已经实现的规则，网页脚本和所有布局不保证原样还原。
- 程序自带的自动检查只核对文件结构和元件属性。
- 交互效果请在实际的 Axure 里预览确认，自动检查不能代替你自己看一遍。

## 许可证

AxureForge 采用 [MIT License](LICENSE)。
安装包内附随第三方组件的许可证文本。
本项目与 Axure 官方无关。
