<p align="center">
  <b>English</b> · <a href="README.zh-CN.md">简体中文</a>
</p>

<p align="center">
  <img src="docs/images/banner.jpg" alt="AxureForge CLI — batch-edit prototypes, skip the clicking" width="100%">
</p>

<h1 align="center">AxureForge CLI</h1>

<p align="center"><b>Batch-edit prototypes. Skip the clicking.</b></p>
<p align="center">
  Create, read and edit Axure RP9 / RP11 prototype files (<code>.rp</code>).<br>
  Pages, widgets, copy, web pages, version conversion — one command each.
</p>

<p align="center">
  <img alt="macOS (Apple Silicon)" src="https://img.shields.io/badge/macOS-Apple%20Silicon-000000?logo=apple&logoColor=white">
  <img alt="Linux x64" src="https://img.shields.io/badge/Linux-x64-FCC624?logo=linux&logoColor=black">
  <img alt="Windows x64" src="https://img.shields.io/badge/Windows-x64-0078D4?logo=windows&logoColor=white">
  <img alt="Latest release" src="https://img.shields.io/github/v/release/qizhi2design/axureforge-cli?color=0A7AFF">
  <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-22C55E">
</p>

<p align="center">
  <img alt="Axure RP9 / RP11" src="https://img.shields.io/badge/RP9%20%2F%20RP11-22D3EE?style=flat-square">
  <img alt="HTML import" src="https://img.shields.io/badge/HTML%20import-22D3EE?style=flat-square">
  <img alt="Batch edits" src="https://img.shields.io/badge/Batch%20edits-22D3EE?style=flat-square">
  <img alt="Strict conversion" src="https://img.shields.io/badge/Strict%20conversion-22D3EE?style=flat-square">
</p>

<p align="center">
  <a href="#what-it-does">What it does</a> ·
  <a href="#download-and-install">Download and install</a> ·
  <a href="#three-minute-tour">Three-minute tour</a> ·
  <a href="#common-tasks">Common tasks</a> ·
  <a href="#advanced">Advanced</a> ·
  <a href="#faq">FAQ</a> ·
  <a href="#scope-and-limits">Scope</a> ·
  <a href="#updates-and-versions">Updates</a> ·
  <a href="#license-and-compliance">License</a>
</p>

## What it does

- 🆕 Start a new RP9 or RP11 prototype from scratch.
- 🧩 36 top-level entries and 170 leaf commands: pages and page tree, widgets, dynamic panels, repeaters, tables, trees, menus, masters and master tree, adaptive views, connectors, interactions and interaction styles, expressions, component libraries, groups, frames, folders, search, formats and batch.
- 🌐 Import an existing web page in one pass; layout is computed for you and you get an editable page.
- 🔍 `dump` builds an index, so you can query pages and widgets locally instead of reopening the file.
- ⚡ Batch edits commit in one go: either all of them land, or none of them do.
- 🔄 Convert between RP9 and RP11 with a strict, lossless policy: preflight first, then convert.
- ✅ Check structure and estimate layout without opening the Axure UI.

Prefer plain-language requests in Chinese? Use it together with [axure-forge-skill](https://github.com/qizhi2design/axure-forge-skill).

## Download and install

AxureForge ships as a directory package. **Keep the whole directory, `_internal` included.** Copying only the executable will fail to start.

1. Open the [releases page](https://github.com/qizhi2design/axureforge-cli/releases) and download the archive for your platform plus `SHA256SUMS`.
2. Put both files in the same folder, verify first, then extract.
3. Enter the extracted directory and run `--version` to confirm it works.

The example below uses 0.5.0 on an Apple-silicon Mac; for Linux and Windows grab the matching archive, the steps are the same.

```bash
shasum -a 256 -c SHA256SUMS
tar -xzf axure-forge-0.5.0-macos-arm64.tar.gz
cd axure-forge-0.5.0-macos-arm64
./axure-forge --version
./axure-forge --help
```

- Line 1: verify the download is intact; a clean check means the file arrived whole.
- Line 2: extract the archive.
- Line 3: enter the extracted folder.
- Line 4: print the version number; if it shows up, the tool works.
- Line 5: list every command the tool supports.

You can move the whole directory to a fixed location and create a command entry for the executable inside it. On macOS the skill's installer can verify and deploy it for you.

## CLI 0.5.0 interface

Run `axure-forge` to see the installed version and grouped command help. All CLI help and messages are in English. Errors retain protocol-v3 JSON on stdout and concise diagnostics on stderr; add `--debug` for tracebacks.

**Breaking change:** command groups use kebab-case: `adaptive-view`, `adaptive-view-set`, `interaction-style`, `master-folder`, `master-instance`, `master-tree`, and `page-tree`. Underscore spellings and abbreviated long options are rejected. Batch operation names such as `master_instance.create` are unchanged. See the [complete help snapshot](docs/cli-help.md) and [release notes](docs/RELEASE-0.5.md).

## Three-minute tour

Grab a prototype file and put it in the current directory; the examples call it `demo.rp`. If you do not have one yet, create an empty one with `project create` in the next section.

First, see what it can do:

```bash
./axure-forge capabilities --json
./axure-forge dump --project demo.rp
./axure-forge verify --project demo.rp
```

- `capabilities --json` lists every command group, command, parameter, supported version and known limitation in one response.
- `dump --project demo.rp` writes an index to `.forge/index` and turns pages and widgets into a queryable inventory.
- `verify --project demo.rp` checks the file structure and estimates layout without opening any UI; visual and interaction checks are out of scope.

None of these three commands modifies `demo.rp`.

## Common tasks

**Create a prototype, then list its pages:**

```bash
./axure-forge project create --name Demo --output demo.rp
./axure-forge page list --project demo.rp
```

- Line 1: create a prototype named Demo and save it as `demo.rp`; it defaults to RP9, add `--format-version 11` for RP11.
- Line 2: list the pages inside the file and note the page id (`scope_id`).

**Look up templates and formats:**

```bash
./axure-forge search explore --query input --category template
./axure-forge format list
```

- Line 1: search built-in templates for "input" to see what you can reuse.
- Line 2: list the formats and widget types the tool knows about.

**Add a widget:**

Run `page list` first, then replace `YOUR_SCOPE_ID` below with the page id you got.

```bash
./axure-forge node create --project demo.rp --scope-id YOUR_SCOPE_ID \
  --spec '{"kind":"text","text":"Hello Axure"}' --output edited.rp
```

This adds a text block to that page and saves the result as `edited.rp`.

**Turn a web page into a prototype page:**

```bash
./axure-forge html import --project demo.rp \
  --html '<h1>Hello Axure</h1><p>Editable prototype</p>' \
  --page-name HTML --page-size 1440x900 --output imported.rp
```

The markup becomes a new page named `HTML`: 1440 px wide, at least 900 px tall and growing with the content. The result is saved as `imported.rp`.

**Editing always needs an output path.** Any command that produces a new file takes `--output`.

**Nothing is overwritten by default.** If the target file exists the command stops; add `--force` to overwrite.

## Advanced

<details>
<summary><b>Working directory and evidence</b></summary>

The default working directory is `.forge/` in the current folder; change it with `--work-dir DIR`.
Indexes, layout plans, verification reports and summaries all live there.

`html import` and `batch` write `.forge/summary.json` when they finish. Read that first to get the output file, index and report paths, then dig into details only as needed.

`dump` produces the index; `verify` can check either a prototype or an existing index.
Any write command given `--index` first checks the source file hash and refuses to run if the source has changed.

```bash
./axure-forge dump --project demo.rp --work-dir .forge
./axure-forge verify --index .forge/index
```

The second command reads the index directly and does not parse the prototype again.

</details>

<details>
<summary><b>HTML import: what works, what doesn't</b></summary>

Five layout models are supported: block, inline, flex, table and absolute.

Limits:

- JavaScript is not executed.
- Remote assets are not fetched and external stylesheets are not read.
- CSS grid is not supported.
- Text widths are estimates.
- No GUI rendering is performed.

`--page-size 1440x900` fixes the width at 1440 and uses 900 as the minimum height, growing with content.
`--page-mode fixed` switches to a fixed width and height; `auto` is the default.
When creating a new file, pick the format with `--format-version 9` or `--format-version 11`.

`--plan` reuses a layout that has already been computed:

```bash
./axure-forge html plan ./site --page-size 1440x900 --output plan.json
./axure-forge html import ./site --page-size 1440x900 --plan plan.json --output imported.rp
```

`html plan` only computes layout and writes no prototype. If the input or the actual assets change, the plan goes stale and must be regenerated.

</details>

<details>
<summary><b>Batch and result references</b></summary>

One `batch` call commits several edits at once: either all of them land, or none of them do.
A failure keeps no partial results and produces no target file.

Each operation can take an `as` alias, and later steps reference earlier results with `{"$ref":"alias.field"}`.
For example, right after creating a page you can reference its `scope_id` in the next step instead of looking it up again.

```bash
./axure-forge batch ops.json --project demo.rp --index .forge/index --output batched.rp
```

`ops.json` is the batch request file; the format is documented in [batch and verification](https://github.com/qizhi2design/axure-forge-skill/blob/main/skills/axure-forge/references/batch-and-verify.md) (Chinese).
References may only point at steps that already succeeded; a missing field or a duplicate alias is an error.

</details>

<details>
<summary><b>Formats and strict conversion</b></summary>

RP9 and RP11 can both be read, edited and written, and they convert in either direction under a `strict_lossless` policy.
Preflight first, then convert once nothing blocks it:

```bash
./axure-forge project check-conversion --project demo.rp --target-version 11
./axure-forge project convert --project demo.rp --target-version 11 --output demo11.rp
```

`check-conversion` is read-only and never touches the source file; incompatible or unverified data blocks the conversion.
`convert` writes a separate new file and leaves the source untouched; data it does not recognise is preserved verbatim rather than guessed at.
Converting back works the same way — set `--target-version 9`.
Opening an older file never bumps its version implicitly; switch versions only by an explicit conversion.

</details>

## FAQ

<details>
<summary><b>macOS refused to open it the first time?</b></summary>

The binary is not notarised by Apple. Open System Settings → Privacy & Security and allow it there.
Only allow it after you have confirmed the download source and the `SHA256SUMS` check.

</details>

<details>
<summary><b>It fails to start and complains about a temporary directory?</b></summary>

0.5.0 ships as a directory package. Make sure the whole directory and `_internal` are present, and that the executable is allowed to run.

</details>

<details>
<summary><b>`_internal` is missing, or I copied only the executable?</b></summary>

Extract the archive again and keep the full directory. You cannot run `axure-forge` as a single copied file.

</details>

<details>
<summary><b>Can I use it without Axure installed?</b></summary>

Yes. Creating, reading, editing, HTML import, conversion and verification all work without the editor.
Visual and interaction acceptance still needs Axure open.

</details>

<details>
<summary><b>I am worried about breaking a prototype</b></summary>

Copy the prototype first, edit the copy, and replace the original only after you are happy with the result.

</details>

<details>
<summary><b>Where does the edited file go?</b></summary>

Wherever `--output` points. Without it, no new file is written.

</details>

<details>
<summary><b>Will an existing file be overwritten?</b></summary>

No by default — the command stops and tells you. Add `--force` to confirm overwriting.

</details>

<details>
<summary><b>How do I see what a command does?</b></summary>

Append `--help`, for example:

```bash
./axure-forge --help
./axure-forge node --help
./axure-forge node create --help
```

</details>

## Scope and limits

- Builds are provided for Apple-silicon Mac, Linux x64 (Ubuntu 22.04) and Windows x64.
- Axure RP9 and RP11 can both be read, edited and written, and the two formats convert strictly into each other.
- HTML import only covers the layout rules that are implemented; JavaScript, remote assets, external stylesheets and CSS grid are out of scope.
- Automated checks cover file structure and estimated layout only; they do not replace visual or interaction acceptance.
- The tool performs no GUI rendering — the final look is whatever Axure shows when you open the file.

Exit codes: `0` success, `1` execution or verification failure, `2` invalid arguments or input.

## Updates and versions

The current release is 0.5.0. Check CLI and skill versions and update manually:

```bash
axure-forge update check
axure-forge update all --dry-run
axure-forge update all --yes
axure-forge config set sources.cli.repo qizhi2design/axureforge-cli
```

Offline use remains available. Automatic checks fail silently; manual updates leave the current installation intact when the release source is unreachable. See the [update notes](docs/updates.md) for mirrors, rollback and platform behaviour. Users on 0.3.0 must download the complete 0.5.0 directory package once to obtain the new commands.

## License and compliance

AxureForge is released under the [MIT License](LICENSE).

License texts for bundled third-party components ship with the package; see [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

AxureForge is an independent project and is not affiliated with Axure.
