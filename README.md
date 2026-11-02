# AxureForge CLI

> 在电脑上创建、读取和修改 Axure RP9 原型文件（`.rp`）的独立小程序。

## 能做什么

- 从零新建一个 RP9 原型文件，直接开始画。
- 往指定页面里添加文本、按钮、输入框等元件。
- 批量修改元件文案和属性，不用一个个点。
- 把现成的网页（HTML）转成可编辑的原型页面。
- 查询内置的格式模板和元件，快速找到能用的东西。

想直接用中文提需求、不用记命令，可以配合 [axure-forge-skill](https://github.com/qizhi2design/axure-forge-skill) 使用。

## 下载与安装

1. 打开本项目的下载页，下载压缩包和校验文件。
2. 把这两个文件放在同一个文件夹里，先校验，再解压。
3. 进入解压出来的文件夹运行，能看到版本号就说明可用。

下载解压后就能用，不用另外安装运行环境。
下面以 Apple 芯片的 Mac、最新版本 0.2.1 为例；Linux 和 Windows 下载各自的压缩包，步骤一样。
文件名按你实际下载到的版本替换即可。

```bash
shasum -a 256 -c SHA256SUMS
tar -xzf axure-forge-0.2.1-macos-arm64.tar.gz
cd axure-forge-0.2.1-macos-arm64
./axure-forge --version
./axure-forge --help
```

第 1 行：核对下载的文件是否完整，没损坏才算下载成功。
第 2 行：解压压缩包。
第 3 行：进入解压出来的文件夹。
第 4 行：显示版本号，能显示出来就说明程序可用。
第 5 行：列出程序支持的所有命令。

也可以把解压出来的程序复制到自己常用的命令文件夹里，之后在任何位置直接输入 `axure-forge` 使用。

## 快速上手

在解压出来的文件夹里运行下面几条，先把主要功能走一遍。

```bash
./axure-forge project create --name Demo --output demo.rp
./axure-forge page list --project demo.rp
./axure-forge search explore --query 输入框 --category template
./axure-forge format list
```

第 1 行：新建一个叫 Demo 的原型文件，保存成 `demo.rp`。
第 2 行：列出这个文件里有哪些页面。
第 3 行：在内置模板里搜索「输入框」，看看哪些可以直接用。
第 4 行：查看程序认识的格式和元件清单。

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

## 遇到问题

**Mac 首次打开被系统拦下。** 程序没有经过 Apple 的开发者验证，Mac 首次打开时会提示无法验证开发者。请你自己到「系统设置 → 隐私与安全性」里允许它运行。确认下载来源和校验文件都无误后再允许。

**启动失败，提示临时目录不可用。** 程序启动时要往系统临时目录写文件并执行，那个目录必须可写、允许执行；被安全软件或系统策略锁住时会启动不了。

**担心改坏原型。** 建议先复制一份原型再操作，看过结果确认没问题，再替换正式文件。

**想看某个命令怎么用。** 在命令后面加 `--help`，例如：

```bash
./axure-forge --help
./axure-forge node --help
./axure-forge node create --help
```

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
