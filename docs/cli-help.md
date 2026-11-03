# CLI display copy

Generated from the current argparse declarations. Includes every help page and parameter.
Regenerate with `uv run python scripts/export_cli_help.py`.

## Executable commands

```text
axure-forge update check
axure-forge update cli
axure-forge update skill
axure-forge update all
axure-forge config show
axure-forge config set
axure-forge config reset
axure-forge capabilities
axure-forge dump
axure-forge verify
axure-forge adaptive-view bind-page
axure-forge adaptive-view create
axure-forge adaptive-view delete
axure-forge adaptive-view get-bounds
axure-forge adaptive-view get-style
axure-forge adaptive-view get-visibility
axure-forge adaptive-view list
axure-forge adaptive-view reset-bounds
axure-forge adaptive-view reset-style
axure-forge adaptive-view reset-visible
axure-forge adaptive-view set-bounds
axure-forge adaptive-view set-style
axure-forge adaptive-view set-text
axure-forge adaptive-view set-visible
axure-forge adaptive-view unbind-page
axure-forge adaptive-view update
axure-forge adaptive-view-set create
axure-forge adaptive-view-set delete
axure-forge adaptive-view-set list
axure-forge adaptive-view-set rename
axure-forge choice add
axure-forge choice delete
axure-forge choice move
axure-forge choice options
axure-forge choice select
axure-forge choice set-multiple
axure-forge choice update
axure-forge connector create
axure-forge connector get-path
axure-forge connector set-path
axure-forge expression call
axure-forge expression catalogue
axure-forge folder create
axure-forge folder delete
axure-forge folder get
axure-forge folder list
axure-forge folder move
axure-forge folder rename
axure-forge format get
axure-forge format list
axure-forge frame clear-target
axure-forge frame get-target
axure-forge frame set-page-target
axure-forge frame set-url-target
axure-forge group set-members
axure-forge html import
axure-forge html plan
axure-forge interaction add
axure-forge interaction catalogue
axure-forge interaction clear
axure-forge interaction get
axure-forge interaction set
axure-forge interaction-style clear
axure-forge interaction-style get
axure-forge interaction-style set
axure-forge library instantiate
axure-forge library register
axure-forge master create
axure-forge master delete
axure-forge master get
axure-forge master instances
axure-forge master list
axure-forge master move
axure-forge master rename
axure-forge master-folder create
axure-forge master-folder delete
axure-forge master-folder get
axure-forge master-folder move
axure-forge master-folder rename
axure-forge master-instance clear-text-override
axure-forge master-instance create
axure-forge master-instance delete
axure-forge master-instance detach
axure-forge master-instance get
axure-forge master-instance reset
axure-forge master-instance set-text-override
axure-forge master-instance text-overrides
axure-forge master-instance update
axure-forge master-tree get
axure-forge menu add-item
axure-forge menu create-submenu
axure-forge menu delete-item
axure-forge menu delete-submenu
axure-forge menu get-hierarchy
axure-forge menu get-submenu
axure-forge menu list-items
axure-forge menu move-item
axure-forge menu move-item-to
axure-forge node configure
axure-forge node create
axure-forge node delete
axure-forge node describe
axure-forge node get
axure-forge node group
axure-forge node list
axure-forge node move
axure-forge node properties
axure-forge node replace-image
axure-forge node set-reference-page
axure-forge node set-text-runs
axure-forge node style-text-span
axure-forge node ungroup
axure-forge node update
axure-forge page add-event
axure-forge page clear-events
axure-forge page create
axure-forge page delete
axure-forge page get
axure-forge page get-events
axure-forge page list
axure-forge page move
axure-forge page rename
axure-forge page select
axure-forge page set-events
axure-forge page-tree get
axure-forge panel add-state
axure-forge panel create
axure-forge panel delete
axure-forge panel delete-state
axure-forge panel get
axure-forge panel get-state
axure-forge panel list
axure-forge panel move-state
axure-forge panel rename-state
axure-forge panel set-options
axure-forge project check-conversion
axure-forge project close
axure-forge project convert
axure-forge project create
axure-forge project export
axure-forge project open
axure-forge reference list
axure-forge reference masters
axure-forge reference resolve-master
axure-forge reference resolve-package
axure-forge reference widget-template
axure-forge repeater configure
axure-forge repeater create
axure-forge repeater delete
axure-forge repeater get
axure-forge repeater get-data
axure-forge repeater get-options
axure-forge repeater set-data
axure-forge search context
axure-forge search explore
axure-forge system capabilities
axure-forge table edit-axis
axure-forge table get-cell
axure-forge table get-grid
axure-forge table update-cell
axure-forge tree add-item
axure-forge tree delete-item
axure-forge tree list-items
axure-forge tree move-item
axure-forge tree update-item
axure-forge web capture
axure-forge web import
axure-forge web plan
axure-forge web prepare
axure-forge batch
```

## axure-forge --help

```text
axure-forge 0.5.0
Create, inspect, and edit Axure RP9/RP11 projects.

Usage:
  axure-forge <command> [options]

Project commands:
  project             Create, open, export, and convert projects.
  format              Inspect supported RP file formats.

Import commands:
  html                Plan and import local HTML.
  web                 Prepare and import host-browser captures.

Page and widget commands:
  page                Manage pages and page events.
  page-tree           Inspect the page hierarchy.
  folder              Organize page folders.
  node                Create, inspect, and edit widgets.
  group               Manage widget group membership.
  panel               Manage dynamic panels and their states.
  choice              Edit choice options and selection.
  menu                Manage menus and nested items.
  table               Inspect and edit table cells and axes.
  tree                Manage tree widget items.
  repeater            Manage repeaters, options, and data.
  frame               Set inline frame navigation targets.
  connector           Create connectors and edit their paths.

Interaction commands:
  interaction         Inspect and edit widget interactions.
  interaction-style   Manage widget interaction styles.
  expression          Inspect and construct interaction expressions.

Reuse and adaptive commands:
  master              Manage reusable masters.
  master-folder       Organize master folders.
  master-instance     Manage master instances and overrides.
  master-tree         Inspect the master hierarchy.
  library             Register and instantiate local component templates.
  reference           Inspect and resolve library references.
  adaptive-view       Manage adaptive views and widget overrides.
  adaptive-view-set   Manage adaptive view sets.

Inspection and maintenance commands:
  search              Find widgets and reusable templates.
  dump                Export a reusable project index.
  verify              Check a project or index without the Axure GUI.
  capabilities        Describe CLI commands and supported capabilities as JSON.
  system              Inspect RP capabilities and protocol operations.
  batch               Execute atomic operations from a batch JSON file.
  update              Check for and install CLI or skill updates.
  config              Manage update sources and preferences.

Options:
  -h, --help          Show help and exit.
  --version           Show the installed version and exit.
  --debug             Show diagnostic tracebacks on errors.

Examples:
  axure-forge project create --name Demo -o demo.rp
  axure-forge html import index.html -o demo.rp

Run 'axure-forge <command> --help' for command details.
Exit codes: 0 success; 1 execution/verification failure; 2 invalid input; 130 cancelled.
```

## axure-forge update --help

```text
usage: axure-forge update [-h] [--debug] [--json] [--repo REPO]
                          [--mirror-prefix MIRROR_PREFIX] [--path PATH]
                          [--component {cli,skill,all}]
                          {check,cli,skill,all} ...

Check for and install CLI or skill updates.

positional arguments:
  {check,cli,skill,all}
    check               Check available compatible versions without
                        installing.
    cli                 Update the CLI installation.
    skill               Update a skill installation.
    all                 Update the CLI and skill together.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --json                Protocol-v3 JSON output.
  --repo REPO           One-shot GitHub owner/repo override.
  --mirror-prefix MIRROR_PREFIX
                        One-shot HTTPS mirror prefix.
  --path PATH           Installed skill directory.
  --component {cli,skill,all}
                        Components to check (default: all).
```

## axure-forge update check --help

```text
usage: axure-forge update check [-h] [--debug] [--json] [--repo REPO]
                                [--mirror-prefix MIRROR_PREFIX] [--path PATH]
                                [--component {cli,skill,all}]

Check available compatible versions without installing.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --json                Protocol-v3 JSON output.
  --repo REPO           One-shot GitHub owner/repo override.
  --mirror-prefix MIRROR_PREFIX
                        One-shot HTTPS mirror prefix.
  --path PATH           Installed skill directory.
  --component {cli,skill,all}
                        Components to check (default: all).
```

## axure-forge update cli --help

```text
usage: axure-forge update cli [-h] [--debug] [--json] [--repo REPO]
                              [--mirror-prefix MIRROR_PREFIX] [--path PATH]
                              [--version VERSION] [--yes] [--dry-run]
                              [--force] [--allow-downgrade]

Update the CLI installation.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --json                Protocol-v3 JSON output.
  --repo REPO           One-shot GitHub owner/repo override.
  --mirror-prefix MIRROR_PREFIX
                        One-shot HTTPS mirror prefix.
  --path PATH           Installed skill directory.
  --version VERSION     Explicit stable version (cli or skill only).
  --yes                 Approve the displayed update plan.
  --dry-run             Resolve without installing.
  --force               Back up and replace modified/unknown skill.
  --allow-downgrade     Allow installing an older compatible version.
```

## axure-forge update skill --help

```text
usage: axure-forge update skill [-h] [--debug] [--json] [--repo REPO]
                                [--mirror-prefix MIRROR_PREFIX] [--path PATH]
                                [--version VERSION] [--yes] [--dry-run]
                                [--force] [--allow-downgrade]

Update a skill installation.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --json                Protocol-v3 JSON output.
  --repo REPO           One-shot GitHub owner/repo override.
  --mirror-prefix MIRROR_PREFIX
                        One-shot HTTPS mirror prefix.
  --path PATH           Installed skill directory.
  --version VERSION     Explicit stable version (cli or skill only).
  --yes                 Approve the displayed update plan.
  --dry-run             Resolve without installing.
  --force               Back up and replace modified/unknown skill.
  --allow-downgrade     Allow installing an older compatible version.
```

## axure-forge update all --help

```text
usage: axure-forge update all [-h] [--debug] [--json] [--repo REPO]
                              [--mirror-prefix MIRROR_PREFIX] [--path PATH]
                              [--version VERSION] [--yes] [--dry-run]
                              [--force] [--allow-downgrade]

Update the CLI and skill together.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --json                Protocol-v3 JSON output.
  --repo REPO           One-shot GitHub owner/repo override.
  --mirror-prefix MIRROR_PREFIX
                        One-shot HTTPS mirror prefix.
  --path PATH           Installed skill directory.
  --version VERSION     Explicit stable version (cli or skill only).
  --yes                 Approve the displayed update plan.
  --dry-run             Resolve without installing.
  --force               Back up and replace modified/unknown skill.
  --allow-downgrade     Allow installing an older compatible version.
```

## axure-forge config --help

```text
usage: axure-forge config [-h] [--debug] {show,set,reset} ...

Manage update sources and preferences.

positional arguments:
  {show,set,reset}
    show            Show current update configuration.
    set             Set a configuration key to a value.
    reset           Reset one key or all configuration to defaults.

options:
  -h, --help        Show help and exit.
  --debug           Show diagnostic tracebacks on errors.
```

## axure-forge config show --help

```text
usage: axure-forge config show [-h] [--debug] [--json]

Show current update configuration.

options:
  -h, --help  Show help and exit.
  --debug     Show diagnostic tracebacks on errors.
  --json      Return protocol-v3 JSON.
```

## axure-forge config set --help

```text
usage: axure-forge config set [-h] [--debug] [--json] key value

Set a configuration key to a value.

positional arguments:
  key         Configuration key, such as updates.auto-check.
  value       New configuration value.

options:
  -h, --help  Show help and exit.
  --debug     Show diagnostic tracebacks on errors.
  --json      Return protocol-v3 JSON.
```

## axure-forge config reset --help

```text
usage: axure-forge config reset [-h] [--debug] [--json] [key]

Reset one key or all configuration to defaults.

positional arguments:
  key         Configuration key, such as updates.auto-check.

options:
  -h, --help  Show help and exit.
  --debug     Show diagnostic tracebacks on errors.
  --json      Return protocol-v3 JSON.
```

## axure-forge capabilities --help

```text
usage: axure-forge capabilities [-h] [--debug] [--json]

Describe CLI commands and supported capabilities as JSON.

options:
  -h, --help  Show help and exit.
  --debug     Show diagnostic tracebacks on errors.
  --json      Return machine-readable JSON (also the default).
```

## axure-forge dump --help

```text
usage: axure-forge dump [-h] [--debug] [--project PROJECT] [--force]
                        [--work-dir WORK_DIR] [--evidence-dir EVIDENCE_DIR]
                        [--index INDEX_DIR] [--verify]
                        [--fail-on {error,warn,none}] [--json JSON]
                        [--output OUTPUT] [--check]

Export a reusable project index.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --output OUTPUT       Index directory (default: WORK_DIR/index).
  --check               Only check index integrity and source freshness.
```

## axure-forge verify --help

```text
usage: axure-forge verify [-h] [--debug] [--project PROJECT] [--force]
                          [--work-dir WORK_DIR] [--evidence-dir EVIDENCE_DIR]
                          [--index INDEX_DIR] [--verify]
                          [--fail-on {error,warn,none}] [--json JSON]

Check a project or index without the Axure GUI.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
```

## axure-forge adaptive-view --help

```text
usage: axure-forge adaptive-view [-h] [--debug]
                                 {bind-page,create,delete,get-bounds,get-style,get-visibility,list,reset-bounds,reset-style,reset-visible,set-bounds,set-style,set-text,set-visible,unbind-page,update} ...

Manage adaptive views and widget overrides.

positional arguments:
  {bind-page,create,delete,get-bounds,get-style,get-visibility,list,reset-bounds,reset-style,reset-visible,set-bounds,set-style,set-text,set-visible,unbind-page,update}
    bind-page           Bind a page to an adaptive view set.
    create              Create an adaptive view.
    delete              Delete an adaptive view.
    get-bounds          Inspect widget bounds in an adaptive view.
    get-style           Inspect widget style overrides in an adaptive view.
    get-visibility      Inspect widget visibility in an adaptive view.
    list                List adaptive views.
    reset-bounds        Remove widget bounds overrides from an adaptive view.
    reset-style         Remove widget style overrides from an adaptive view.
    reset-visible       Remove widget visibility overrides from an adaptive
                        view.
    set-bounds          Override widget bounds in an adaptive view.
    set-style           Override widget styles in an adaptive view.
    set-text            Override widget text in an adaptive view.
    set-visible         Override widget visibility in an adaptive view.
    unbind-page         Remove the adaptive view set binding from a page.
    update              Update an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge adaptive-view bind-page --help

```text
usage: axure-forge adaptive-view bind-page [-h] [--debug] [--project PROJECT]
                                           [-o OUTPUT] [--force]
                                           [--work-dir WORK_DIR]
                                           [--evidence-dir EVIDENCE_DIR]
                                           [--index INDEX_DIR] [--verify]
                                           [--fail-on {error,warn,none}]
                                           [--json JSON]
                                           [--library-path LIBRARY_PATH]
                                           [--page-id PAGE_ID]
                                           [--set-id SET_ID]

Bind a page to an adaptive view set.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --set-id SET_ID       Adaptive view set ID. (required unless provided by
                        file context)

Required inputs: --page-id, --set-id. Project context is supplied by --project
when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view create --help

```text
usage: axure-forge adaptive-view create [-h] [--debug] [--project PROJECT]
                                        [-o OUTPUT] [--force]
                                        [--work-dir WORK_DIR]
                                        [--evidence-dir EVIDENCE_DIR]
                                        [--index INDEX_DIR] [--verify]
                                        [--fail-on {error,warn,none}]
                                        [--json JSON]
                                        [--library-path LIBRARY_PATH]
                                        [--set-id SET_ID] [--name NAME]
                                        [--width WIDTH] [--height HEIGHT]
                                        [--base-id BASE_ID]

Create an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --set-id SET_ID       Adaptive view set ID. (required unless provided by
                        file context)
  --name NAME           Display name. (required unless provided by file
                        context)
  --width WIDTH         Width in pixels. (required unless provided by file
                        context)
  --height HEIGHT       Height in pixels. (required unless provided by file
                        context)
  --base-id BASE_ID     Base adaptive view ID.

Required inputs: --set-id, --name, --width, --height. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge adaptive-view delete --help

```text
usage: axure-forge adaptive-view delete [-h] [--debug] [--project PROJECT]
                                        [-o OUTPUT] [--force]
                                        [--work-dir WORK_DIR]
                                        [--evidence-dir EVIDENCE_DIR]
                                        [--index INDEX_DIR] [--verify]
                                        [--fail-on {error,warn,none}]
                                        [--json JSON]
                                        [--library-path LIBRARY_PATH]
                                        [--set-id SET_ID] [--view-id VIEW_ID]

Delete an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --set-id SET_ID       Adaptive view set ID. (required unless provided by
                        file context)
  --view-id VIEW_ID     Adaptive view ID. (required unless provided by file
                        context)

Required inputs: --set-id, --view-id. Project context is supplied by --project
when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view get-bounds --help

```text
usage: axure-forge adaptive-view get-bounds [-h] [--debug] [--project PROJECT]
                                            [-o OUTPUT] [--force]
                                            [--work-dir WORK_DIR]
                                            [--evidence-dir EVIDENCE_DIR]
                                            [--index INDEX_DIR] [--verify]
                                            [--fail-on {error,warn,none}]
                                            [--json JSON]
                                            [--library-path LIBRARY_PATH]
                                            [--page-id PAGE_ID]
                                            [--view-id VIEW_ID]
                                            [--node-id NODE_ID]

Inspect widget bounds in an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --view-id VIEW_ID     Adaptive view ID. (required unless provided by file
                        context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --page-id, --view-id, --node-id. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view get-style --help

```text
usage: axure-forge adaptive-view get-style [-h] [--debug] [--project PROJECT]
                                           [-o OUTPUT] [--force]
                                           [--work-dir WORK_DIR]
                                           [--evidence-dir EVIDENCE_DIR]
                                           [--index INDEX_DIR] [--verify]
                                           [--fail-on {error,warn,none}]
                                           [--json JSON]
                                           [--library-path LIBRARY_PATH]
                                           [--page-id PAGE_ID]
                                           [--view-id VIEW_ID]
                                           [--node-id NODE_ID]

Inspect widget style overrides in an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --view-id VIEW_ID     Adaptive view ID. (required unless provided by file
                        context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --page-id, --view-id, --node-id. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view get-visibility --help

```text
usage: axure-forge adaptive-view get-visibility [-h] [--debug]
                                                [--project PROJECT]
                                                [-o OUTPUT] [--force]
                                                [--work-dir WORK_DIR]
                                                [--evidence-dir EVIDENCE_DIR]
                                                [--index INDEX_DIR] [--verify]
                                                [--fail-on {error,warn,none}]
                                                [--json JSON]
                                                [--library-path LIBRARY_PATH]
                                                [--page-id PAGE_ID]
                                                [--view-id VIEW_ID]
                                                [--node-id NODE_ID]

Inspect widget visibility in an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --view-id VIEW_ID     Adaptive view ID. (required unless provided by file
                        context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --page-id, --view-id, --node-id. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view list --help

```text
usage: axure-forge adaptive-view list [-h] [--debug] [--project PROJECT]
                                      [-o OUTPUT] [--force]
                                      [--work-dir WORK_DIR]
                                      [--evidence-dir EVIDENCE_DIR]
                                      [--index INDEX_DIR] [--verify]
                                      [--fail-on {error,warn,none}]
                                      [--json JSON]
                                      [--library-path LIBRARY_PATH]
                                      [--set-id SET_ID]

List adaptive views.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --set-id SET_ID       Adaptive view set ID. (required unless provided by
                        file context)

Required inputs: --set-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view reset-bounds --help

```text
usage: axure-forge adaptive-view reset-bounds [-h] [--debug]
                                              [--project PROJECT] [-o OUTPUT]
                                              [--force] [--work-dir WORK_DIR]
                                              [--evidence-dir EVIDENCE_DIR]
                                              [--index INDEX_DIR] [--verify]
                                              [--fail-on {error,warn,none}]
                                              [--json JSON]
                                              [--library-path LIBRARY_PATH]
                                              [--page-id PAGE_ID]
                                              [--view-id VIEW_ID]
                                              [--node-id NODE_ID]

Remove widget bounds overrides from an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --view-id VIEW_ID     Adaptive view ID. (required unless provided by file
                        context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --page-id, --view-id, --node-id. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view reset-style --help

```text
usage: axure-forge adaptive-view reset-style [-h] [--debug]
                                             [--project PROJECT] [-o OUTPUT]
                                             [--force] [--work-dir WORK_DIR]
                                             [--evidence-dir EVIDENCE_DIR]
                                             [--index INDEX_DIR] [--verify]
                                             [--fail-on {error,warn,none}]
                                             [--json JSON]
                                             [--library-path LIBRARY_PATH]
                                             [--page-id PAGE_ID]
                                             [--view-id VIEW_ID]
                                             [--node-id NODE_ID]

Remove widget style overrides from an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --view-id VIEW_ID     Adaptive view ID. (required unless provided by file
                        context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --page-id, --view-id, --node-id. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view reset-visible --help

```text
usage: axure-forge adaptive-view reset-visible [-h] [--debug]
                                               [--project PROJECT] [-o OUTPUT]
                                               [--force] [--work-dir WORK_DIR]
                                               [--evidence-dir EVIDENCE_DIR]
                                               [--index INDEX_DIR] [--verify]
                                               [--fail-on {error,warn,none}]
                                               [--json JSON]
                                               [--library-path LIBRARY_PATH]
                                               [--page-id PAGE_ID]
                                               [--view-id VIEW_ID]
                                               [--node-id NODE_ID]

Remove widget visibility overrides from an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --view-id VIEW_ID     Adaptive view ID. (required unless provided by file
                        context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --page-id, --view-id, --node-id. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view set-bounds --help

```text
usage: axure-forge adaptive-view set-bounds [-h] [--debug] [--project PROJECT]
                                            [-o OUTPUT] [--force]
                                            [--work-dir WORK_DIR]
                                            [--evidence-dir EVIDENCE_DIR]
                                            [--index INDEX_DIR] [--verify]
                                            [--fail-on {error,warn,none}]
                                            [--json JSON]
                                            [--library-path LIBRARY_PATH]
                                            [--page-id PAGE_ID]
                                            [--view-id VIEW_ID]
                                            [--node-id NODE_ID]
                                            [--bounds BOUNDS]

Override widget bounds in an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --view-id VIEW_ID     Adaptive view ID. (required unless provided by file
                        context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --bounds BOUNDS       Widget geometry as a JSON object. (required unless
                        provided by file context)

Required inputs: --page-id, --view-id, --node-id, --bounds. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge adaptive-view set-style --help

```text
usage: axure-forge adaptive-view set-style [-h] [--debug] [--project PROJECT]
                                           [-o OUTPUT] [--force]
                                           [--work-dir WORK_DIR]
                                           [--evidence-dir EVIDENCE_DIR]
                                           [--index INDEX_DIR] [--verify]
                                           [--fail-on {error,warn,none}]
                                           [--json JSON]
                                           [--library-path LIBRARY_PATH]
                                           [--page-id PAGE_ID]
                                           [--view-id VIEW_ID]
                                           [--node-id NODE_ID] [--style STYLE]

Override widget styles in an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --view-id VIEW_ID     Adaptive view ID. (required unless provided by file
                        context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --style STYLE         Style patch: fill, border, radius, opacity, font_size,
                        font_weight, color, text, padding or shadow. (required
                        unless provided by file context)

Required inputs: --page-id, --view-id, --node-id, --style. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge adaptive-view set-text --help

```text
usage: axure-forge adaptive-view set-text [-h] [--debug] [--project PROJECT]
                                          [-o OUTPUT] [--force]
                                          [--work-dir WORK_DIR]
                                          [--evidence-dir EVIDENCE_DIR]
                                          [--index INDEX_DIR] [--verify]
                                          [--fail-on {error,warn,none}]
                                          [--json JSON]
                                          [--library-path LIBRARY_PATH]
                                          [--page-id PAGE_ID]
                                          [--view-id VIEW_ID]
                                          [--node-id NODE_ID] [--text TEXT]

Override widget text in an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --view-id VIEW_ID     Adaptive view ID. (required unless provided by file
                        context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --text TEXT           Text content. (required unless provided by file
                        context)

Required inputs: --page-id, --view-id, --node-id, --text. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge adaptive-view set-visible --help

```text
usage: axure-forge adaptive-view set-visible [-h] [--debug]
                                             [--project PROJECT] [-o OUTPUT]
                                             [--force] [--work-dir WORK_DIR]
                                             [--evidence-dir EVIDENCE_DIR]
                                             [--index INDEX_DIR] [--verify]
                                             [--fail-on {error,warn,none}]
                                             [--json JSON]
                                             [--library-path LIBRARY_PATH]
                                             [--page-id PAGE_ID]
                                             [--view-id VIEW_ID]
                                             [--node-id NODE_ID]
                                             [--visible VISIBLE]

Override widget visibility in an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --view-id VIEW_ID     Adaptive view ID. (required unless provided by file
                        context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --visible VISIBLE     Whether the widget is visible (JSON boolean).
                        (required unless provided by file context)

Required inputs: --page-id, --view-id, --node-id, --visible. Project context
is supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge adaptive-view unbind-page --help

```text
usage: axure-forge adaptive-view unbind-page [-h] [--debug]
                                             [--project PROJECT] [-o OUTPUT]
                                             [--force] [--work-dir WORK_DIR]
                                             [--evidence-dir EVIDENCE_DIR]
                                             [--index INDEX_DIR] [--verify]
                                             [--fail-on {error,warn,none}]
                                             [--json JSON]
                                             [--library-path LIBRARY_PATH]
                                             [--page-id PAGE_ID]
                                             [--clear-overrides CLEAR_OVERRIDES]

Remove the adaptive view set binding from a page.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --clear-overrides CLEAR_OVERRIDES
                        Whether to clear existing overrides (JSON boolean).

Required inputs: --page-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view update --help

```text
usage: axure-forge adaptive-view update [-h] [--debug] [--project PROJECT]
                                        [-o OUTPUT] [--force]
                                        [--work-dir WORK_DIR]
                                        [--evidence-dir EVIDENCE_DIR]
                                        [--index INDEX_DIR] [--verify]
                                        [--fail-on {error,warn,none}]
                                        [--json JSON]
                                        [--library-path LIBRARY_PATH]
                                        [--set-id SET_ID] [--view-id VIEW_ID]
                                        [--name NAME] [--width WIDTH]
                                        [--height HEIGHT] [--base-id BASE_ID]

Update an adaptive view.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --set-id SET_ID       Adaptive view set ID. (required unless provided by
                        file context)
  --view-id VIEW_ID     Adaptive view ID. (required unless provided by file
                        context)
  --name NAME           Display name.
  --width WIDTH         Width in pixels.
  --height HEIGHT       Height in pixels.
  --base-id BASE_ID     Base adaptive view ID.

Required inputs: --set-id, --view-id. Project context is supplied by --project
when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view-set --help

```text
usage: axure-forge adaptive-view-set [-h] [--debug]
                                     {create,delete,list,rename} ...

Manage adaptive view sets.

positional arguments:
  {create,delete,list,rename}
    create              Create an adaptive view set.
    delete              Delete an adaptive view set.
    list                List adaptive view sets.
    rename              Rename an adaptive view set.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge adaptive-view-set create --help

```text
usage: axure-forge adaptive-view-set create [-h] [--debug] [--project PROJECT]
                                            [-o OUTPUT] [--force]
                                            [--work-dir WORK_DIR]
                                            [--evidence-dir EVIDENCE_DIR]
                                            [--index INDEX_DIR] [--verify]
                                            [--fail-on {error,warn,none}]
                                            [--json JSON]
                                            [--library-path LIBRARY_PATH]
                                            [--name NAME] [--width WIDTH]
                                            [--height HEIGHT]

Create an adaptive view set.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --name NAME           Display name. (required unless provided by file
                        context)
  --width WIDTH         Width in pixels.
  --height HEIGHT       Height in pixels.

Required inputs: --name. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view-set delete --help

```text
usage: axure-forge adaptive-view-set delete [-h] [--debug] [--project PROJECT]
                                            [-o OUTPUT] [--force]
                                            [--work-dir WORK_DIR]
                                            [--evidence-dir EVIDENCE_DIR]
                                            [--index INDEX_DIR] [--verify]
                                            [--fail-on {error,warn,none}]
                                            [--json JSON]
                                            [--library-path LIBRARY_PATH]
                                            [--set-id SET_ID]

Delete an adaptive view set.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --set-id SET_ID       Adaptive view set ID. (required unless provided by
                        file context)

Required inputs: --set-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view-set list --help

```text
usage: axure-forge adaptive-view-set list [-h] [--debug] [--project PROJECT]
                                          [-o OUTPUT] [--force]
                                          [--work-dir WORK_DIR]
                                          [--evidence-dir EVIDENCE_DIR]
                                          [--index INDEX_DIR] [--verify]
                                          [--fail-on {error,warn,none}]
                                          [--json JSON]
                                          [--library-path LIBRARY_PATH]

List adaptive view sets.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge adaptive-view-set rename --help

```text
usage: axure-forge adaptive-view-set rename [-h] [--debug] [--project PROJECT]
                                            [-o OUTPUT] [--force]
                                            [--work-dir WORK_DIR]
                                            [--evidence-dir EVIDENCE_DIR]
                                            [--index INDEX_DIR] [--verify]
                                            [--fail-on {error,warn,none}]
                                            [--json JSON]
                                            [--library-path LIBRARY_PATH]
                                            [--set-id SET_ID] [--name NAME]

Rename an adaptive view set.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --set-id SET_ID       Adaptive view set ID. (required unless provided by
                        file context)
  --name NAME           Display name. (required unless provided by file
                        context)

Required inputs: --set-id, --name. Project context is supplied by --project
when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge choice --help

```text
usage: axure-forge choice [-h] [--debug]
                          {add,delete,move,options,select,set-multiple,update} ...

Edit choice options and selection.

positional arguments:
  {add,delete,move,options,select,set-multiple,update}
    add                 Add an option to a choice widget.
    delete              Delete an option from a choice widget.
    move                Reorder an option in a choice widget.
    options             List the options of a choice widget.
    select              Set the selected options of a choice widget.
    set-multiple        Enable or disable multiple selection for a choice
                        widget.
    update              Update a choice option.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge choice add --help

```text
usage: axure-forge choice add [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                              [--force] [--work-dir WORK_DIR]
                              [--evidence-dir EVIDENCE_DIR]
                              [--project-index INDEX_DIR] [--verify]
                              [--fail-on {error,warn,none}] [--json JSON]
                              [--library-path LIBRARY_PATH]
                              [--scope-id SCOPE_ID] [--node-id NODE_ID]
                              [--text TEXT] [--selected SELECTED]
                              [--index INDEX]

Add an option to a choice widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --text TEXT           Text content. (required unless provided by file
                        context)
  --selected SELECTED   Whether the option is selected (JSON boolean).
  --index INDEX         Position in the ordered collection.

Required inputs: --scope-id, --node-id, --text. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge choice delete --help

```text
usage: axure-forge choice delete [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH]
                                 [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                 [--option-id OPTION_ID]

Delete an option from a choice widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --option-id OPTION_ID
                        Choice option ID. (required unless provided by file
                        context)

Required inputs: --scope-id, --node-id, --option-id. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge choice move --help

```text
usage: axure-forge choice move [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--project-index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH]
                               [--scope-id SCOPE_ID] [--node-id NODE_ID]
                               [--option-id OPTION_ID] [--index INDEX]

Reorder an option in a choice widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --option-id OPTION_ID
                        Choice option ID. (required unless provided by file
                        context)
  --index INDEX         Position in the ordered collection. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --option-id, --index. Project context
is supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge choice options --help

```text
usage: axure-forge choice options [-h] [--debug] [--project PROJECT]
                                  [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                  [--evidence-dir EVIDENCE_DIR]
                                  [--index INDEX_DIR] [--verify]
                                  [--fail-on {error,warn,none}] [--json JSON]
                                  [--library-path LIBRARY_PATH]
                                  [--scope-id SCOPE_ID] [--node-id NODE_ID]

List the options of a choice widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge choice select --help

```text
usage: axure-forge choice select [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH]
                                 [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                 [--option-ids OPTION_IDS]

Set the selected options of a choice widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --option-ids OPTION_IDS
                        Choice option IDs as a JSON array. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --option-ids. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge choice set-multiple --help

```text
usage: axure-forge choice set-multiple [-h] [--debug] [--project PROJECT]
                                       [-o OUTPUT] [--force]
                                       [--work-dir WORK_DIR]
                                       [--evidence-dir EVIDENCE_DIR]
                                       [--index INDEX_DIR] [--verify]
                                       [--fail-on {error,warn,none}]
                                       [--json JSON]
                                       [--library-path LIBRARY_PATH]
                                       [--scope-id SCOPE_ID]
                                       [--node-id NODE_ID]
                                       [--multiple MULTIPLE]

Enable or disable multiple selection for a choice widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --multiple MULTIPLE   Whether to allow multiple selection (JSON boolean).
                        (required unless provided by file context)

Required inputs: --scope-id, --node-id, --multiple. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge choice update --help

```text
usage: axure-forge choice update [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH]
                                 [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                 [--option-id OPTION_ID] [--text TEXT]
                                 [--selected SELECTED]

Update a choice option.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --option-id OPTION_ID
                        Choice option ID. (required unless provided by file
                        context)
  --text TEXT           Text content.
  --selected SELECTED   Whether the option is selected (JSON boolean).

Required inputs: --scope-id, --node-id, --option-id. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge connector --help

```text
usage: axure-forge connector [-h] [--debug] {create,get-path,set-path} ...

Create connectors and edit their paths.

positional arguments:
  {create,get-path,set-path}
    create              Create a connector.
    get-path            Inspect connector path points and endpoints.
    set-path            Set connector path points and endpoints.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge connector create --help

```text
usage: axure-forge connector create [-h] [--debug] [--project PROJECT]
                                    [-o OUTPUT] [--force]
                                    [--work-dir WORK_DIR]
                                    [--evidence-dir EVIDENCE_DIR]
                                    [--index INDEX_DIR] [--verify]
                                    [--fail-on {error,warn,none}]
                                    [--json JSON]
                                    [--library-path LIBRARY_PATH]
                                    [--scope-id SCOPE_ID] [--points POINTS]
                                    [--start-node-id START_NODE_ID]
                                    [--end-node-id END_NODE_ID]
                                    [--start-direction START_DIRECTION]
                                    [--end-direction END_DIRECTION]
                                    [--auto-reflow AUTO_REFLOW] [--name NAME]

Create a connector.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --points POINTS       Connector path points as a JSON array. (required
                        unless provided by file context)
  --start-node-id START_NODE_ID
                        Connector start widget ID.
  --end-node-id END_NODE_ID
                        Connector end widget ID.
  --start-direction START_DIRECTION
                        Connector start direction.; choices: [1, 2, 4, 8]
  --end-direction END_DIRECTION
                        Connector end direction.; choices: [1, 2, 4, 8]
  --auto-reflow AUTO_REFLOW
                        Whether layout changes trigger automatic reflow (JSON
                        boolean).
  --name NAME           Display name.

Required inputs: --scope-id, --points. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge connector get-path --help

```text
usage: axure-forge connector get-path [-h] [--debug] [--project PROJECT]
                                      [-o OUTPUT] [--force]
                                      [--work-dir WORK_DIR]
                                      [--evidence-dir EVIDENCE_DIR]
                                      [--index INDEX_DIR] [--verify]
                                      [--fail-on {error,warn,none}]
                                      [--json JSON]
                                      [--library-path LIBRARY_PATH]
                                      [--scope-id SCOPE_ID]
                                      [--node-id NODE_ID]

Inspect connector path points and endpoints.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge connector set-path --help

```text
usage: axure-forge connector set-path [-h] [--debug] [--project PROJECT]
                                      [-o OUTPUT] [--force]
                                      [--work-dir WORK_DIR]
                                      [--evidence-dir EVIDENCE_DIR]
                                      [--index INDEX_DIR] [--verify]
                                      [--fail-on {error,warn,none}]
                                      [--json JSON]
                                      [--library-path LIBRARY_PATH]
                                      [--scope-id SCOPE_ID]
                                      [--node-id NODE_ID] [--points POINTS]
                                      [--start-node-id START_NODE_ID]
                                      [--end-node-id END_NODE_ID]
                                      [--start-direction START_DIRECTION]
                                      [--end-direction END_DIRECTION]
                                      [--auto-reflow AUTO_REFLOW]

Set connector path points and endpoints.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --points POINTS       Connector path points as a JSON array. (required
                        unless provided by file context)
  --start-node-id START_NODE_ID
                        Connector start widget ID.
  --end-node-id END_NODE_ID
                        Connector end widget ID.
  --start-direction START_DIRECTION
                        Connector start direction.; choices: [1, 2, 4, 8]
  --end-direction END_DIRECTION
                        Connector end direction.; choices: [1, 2, 4, 8]
  --auto-reflow AUTO_REFLOW
                        Whether layout changes trigger automatic reflow (JSON
                        boolean).

Required inputs: --scope-id, --node-id, --points. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge expression --help

```text
usage: axure-forge expression [-h] [--debug] {call,catalogue} ...

Inspect and construct interaction expressions.

positional arguments:
  {call,catalogue}
    call            Construct a function-call expression.
    catalogue       List supported expression functions and signatures.

options:
  -h, --help        Show help and exit.
  --debug           Show diagnostic tracebacks on errors.
```

## axure-forge expression call --help

```text
usage: axure-forge expression call [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--function FUNCTION] [--args ARGS]

Construct a function-call expression.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --function FUNCTION   Expression function name. (required unless provided by
                        file context)
  --args ARGS           Function arguments as a JSON array.

Required inputs: --function. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge expression catalogue --help

```text
usage: axure-forge expression catalogue [-h] [--debug] [--project PROJECT]
                                        [-o OUTPUT] [--force]
                                        [--work-dir WORK_DIR]
                                        [--evidence-dir EVIDENCE_DIR]
                                        [--index INDEX_DIR] [--verify]
                                        [--fail-on {error,warn,none}]
                                        [--json JSON]
                                        [--library-path LIBRARY_PATH]

List supported expression functions and signatures.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge folder --help

```text
usage: axure-forge folder [-h] [--debug]
                          {create,delete,get,list,move,rename} ...

Organize page folders.

positional arguments:
  {create,delete,get,list,move,rename}
    create              Create a folder.
    delete              Delete a folder.
    get                 Get a folder.
    list                List folders.
    move                Move a folder.
    rename              Rename a folder.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge folder create --help

```text
usage: axure-forge folder create [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--project-index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH] [--name NAME]
                                 [--parent-id PARENT_ID] [--index INDEX]

Create a folder.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --name NAME           Display name. (required unless provided by file
                        context)
  --parent-id PARENT_ID
                        Parent item or folder ID.
  --index INDEX         Position in the ordered collection.

Required inputs: --name. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge folder delete --help

```text
usage: axure-forge folder delete [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH]
                                 [--folder-id FOLDER_ID]
                                 [--recursive RECURSIVE]

Delete a folder.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --folder-id FOLDER_ID
                        Folder ID. (required unless provided by file context)
  --recursive RECURSIVE
                        Whether to include descendants (JSON boolean).

Required inputs: --folder-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge folder get --help

```text
usage: axure-forge folder get [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                              [--force] [--work-dir WORK_DIR]
                              [--evidence-dir EVIDENCE_DIR]
                              [--index INDEX_DIR] [--verify]
                              [--fail-on {error,warn,none}] [--json JSON]
                              [--library-path LIBRARY_PATH]
                              [--folder-id FOLDER_ID]

Get a folder.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --folder-id FOLDER_ID
                        Folder ID. (required unless provided by file context)

Required inputs: --folder-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge folder list --help

```text
usage: axure-forge folder list [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH]

List folders.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge folder move --help

```text
usage: axure-forge folder move [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--project-index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH]
                               [--folder-id FOLDER_ID] [--parent-id PARENT_ID]
                               [--index INDEX]

Move a folder.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --folder-id FOLDER_ID
                        Folder ID. (required unless provided by file context)
  --parent-id PARENT_ID
                        Parent item or folder ID.
  --index INDEX         Position in the ordered collection.

Required inputs: --folder-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge folder rename --help

```text
usage: axure-forge folder rename [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH]
                                 [--folder-id FOLDER_ID] [--name NAME]

Rename a folder.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --folder-id FOLDER_ID
                        Folder ID. (required unless provided by file context)
  --name NAME           Display name. (required unless provided by file
                        context)

Required inputs: --folder-id, --name. Project context is supplied by --project
when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge format --help

```text
usage: axure-forge format [-h] [--debug] {get,list} ...

Inspect supported RP file formats.

positional arguments:
  {get,list}
    get       Get a RP format.
    list      List RP formats.

options:
  -h, --help  Show help and exit.
  --debug     Show diagnostic tracebacks on errors.
```

## axure-forge format get --help

```text
usage: axure-forge format get [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                              [--force] [--work-dir WORK_DIR]
                              [--evidence-dir EVIDENCE_DIR]
                              [--index INDEX_DIR] [--verify]
                              [--fail-on {error,warn,none}] [--json JSON]
                              [--library-path LIBRARY_PATH] [--tag TAG]

Get a RP format.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --tag TAG             Search tag filter. (required unless provided by file
                        context)

Required inputs: --tag. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge format list --help

```text
usage: axure-forge format list [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH] [--family FAMILY]

List RP formats.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --family FAMILY       Widget family filter.

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge frame --help

```text
usage: axure-forge frame [-h] [--debug]
                         {clear-target,get-target,set-page-target,set-url-target} ...

Set inline frame navigation targets.

positional arguments:
  {clear-target,get-target,set-page-target,set-url-target}
    clear-target        Clear the navigation target of an inline frame.
    get-target          Inspect the navigation target of an inline frame.
    set-page-target     Point an inline frame to a project page.
    set-url-target      Point an inline frame to a URL.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge frame clear-target --help

```text
usage: axure-forge frame clear-target [-h] [--debug] [--project PROJECT]
                                      [-o OUTPUT] [--force]
                                      [--work-dir WORK_DIR]
                                      [--evidence-dir EVIDENCE_DIR]
                                      [--index INDEX_DIR] [--verify]
                                      [--fail-on {error,warn,none}]
                                      [--json JSON]
                                      [--library-path LIBRARY_PATH]
                                      [--scope-id SCOPE_ID]
                                      [--node-id NODE_ID]

Clear the navigation target of an inline frame.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge frame get-target --help

```text
usage: axure-forge frame get-target [-h] [--debug] [--project PROJECT]
                                    [-o OUTPUT] [--force]
                                    [--work-dir WORK_DIR]
                                    [--evidence-dir EVIDENCE_DIR]
                                    [--index INDEX_DIR] [--verify]
                                    [--fail-on {error,warn,none}]
                                    [--json JSON]
                                    [--library-path LIBRARY_PATH]
                                    [--scope-id SCOPE_ID] [--node-id NODE_ID]

Inspect the navigation target of an inline frame.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge frame set-page-target --help

```text
usage: axure-forge frame set-page-target [-h] [--debug] [--project PROJECT]
                                         [-o OUTPUT] [--force]
                                         [--work-dir WORK_DIR]
                                         [--evidence-dir EVIDENCE_DIR]
                                         [--index INDEX_DIR] [--verify]
                                         [--fail-on {error,warn,none}]
                                         [--json JSON]
                                         [--library-path LIBRARY_PATH]
                                         [--scope-id SCOPE_ID]
                                         [--node-id NODE_ID]
                                         [--page-id PAGE_ID]

Point an inline frame to a project page.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --page-id PAGE_ID     Page ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id, --page-id. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge frame set-url-target --help

```text
usage: axure-forge frame set-url-target [-h] [--debug] [--project PROJECT]
                                        [-o OUTPUT] [--force]
                                        [--work-dir WORK_DIR]
                                        [--evidence-dir EVIDENCE_DIR]
                                        [--index INDEX_DIR] [--verify]
                                        [--fail-on {error,warn,none}]
                                        [--json JSON]
                                        [--library-path LIBRARY_PATH]
                                        [--scope-id SCOPE_ID]
                                        [--node-id NODE_ID] [--url URL]

Point an inline frame to a URL.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --url URL             Navigation URL. (required unless provided by file
                        context)

Required inputs: --scope-id, --node-id, --url. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge group --help

```text
usage: axure-forge group [-h] [--debug] {set-members} ...

Manage widget group membership.

positional arguments:
  {set-members}
    set-members  Replace the ordered members of a widget group.

options:
  -h, --help     Show help and exit.
  --debug        Show diagnostic tracebacks on errors.
```

## axure-forge group set-members --help

```text
usage: axure-forge group set-members [-h] [--debug] [--project PROJECT]
                                     [-o OUTPUT] [--force]
                                     [--work-dir WORK_DIR]
                                     [--evidence-dir EVIDENCE_DIR]
                                     [--index INDEX_DIR] [--verify]
                                     [--fail-on {error,warn,none}]
                                     [--json JSON]
                                     [--library-path LIBRARY_PATH]
                                     [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                     [--node-ids NODE_IDS]

Replace the ordered members of a widget group.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --node-ids NODE_IDS   Ordered widget IDs as a JSON array. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --node-ids. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge html --help

```text
usage: axure-forge html [-h] [--debug] {import,plan} ...

Plan and import local HTML.

positional arguments:
  {import,plan}
    import       Import local HTML as editable native widgets.
    plan         Compute a reusable HTML layout without writing an RP file.

options:
  -h, --help     Show help and exit.
  --debug        Show diagnostic tracebacks on errors.
```

## axure-forge html import --help

```text
usage: axure-forge html import [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH]
                               [--page-size PAGE_SIZE]
                               [--format-version {9,11}] [--html HTML]
                               [--page-name PAGE_NAME] [--base-path BASE_PATH]
                               [--viewport VIEWPORT] [--mapping MAPPING]
                               [--plan PLAN] [--text-metrics TEXT_METRICS]
                               [--page-mode PAGE_MODE]
                               [input]

Import local HTML as editable native widgets.

positional arguments:
  input                 HTML file or directory with index.html.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-size PAGE_SIZE
                        WIDTHxHEIGHT; fixed width and minimum height, e.g.
                        1440x900.
  --format-version {9,11}
                        Format for a new project (default: 9); existing
                        projects keep their version.
  --html HTML           HTML source text. (required unless provided by file
                        context)
  --page-name PAGE_NAME
                        Name of the imported page.
  --base-path BASE_PATH
                        Local base directory for resolving HTML assets.
  --viewport VIEWPORT   Canvas dimensions as a JSON array [width, height].
  --mapping MAPPING     HTML-to-widget mappings as a JSON object.
  --plan PLAN           Import plan as JSON or a JSON file path.
  --text-metrics TEXT_METRICS
                        Text measurement configuration as a JSON object.
  --page-mode PAGE_MODE
                        HTML page import mode.; choices: ['auto', 'fixed']

Required inputs: --html. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge html plan --help

```text
usage: axure-forge html plan [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                             [--force] [--work-dir WORK_DIR]
                             [--evidence-dir EVIDENCE_DIR] [--index INDEX_DIR]
                             [--verify] [--fail-on {error,warn,none}]
                             [--json JSON] [--library-path LIBRARY_PATH]
                             [--page-size PAGE_SIZE] [--html HTML]
                             [--base-path BASE_PATH] [--viewport VIEWPORT]
                             [--mapping MAPPING] [--text-metrics TEXT_METRICS]
                             [--page-mode PAGE_MODE]
                             [input]

Compute a reusable HTML layout without writing an RP file.

positional arguments:
  input                 HTML file or directory with index.html.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-size PAGE_SIZE
                        WIDTHxHEIGHT; fixed width and minimum height, e.g.
                        1440x900.
  --html HTML           HTML source text. (required unless provided by file
                        context)
  --base-path BASE_PATH
                        Local base directory for resolving HTML assets.
  --viewport VIEWPORT   Canvas dimensions as a JSON array [width, height].
  --mapping MAPPING     HTML-to-widget mappings as a JSON object.
  --text-metrics TEXT_METRICS
                        Text measurement configuration as a JSON object.
  --page-mode PAGE_MODE
                        HTML page import mode.; choices: ['auto', 'fixed']

Required inputs: --html. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge interaction --help

```text
usage: axure-forge interaction [-h] [--debug]
                               {add,catalogue,clear,get,set} ...

Inspect and edit widget interactions.

positional arguments:
  {add,catalogue,clear,get,set}
    add                 Add an event interaction to a widget.
    catalogue           List supported events and interaction actions.
    clear               Clear widget event interactions.
    get                 Inspect widget event interactions.
    set                 Replace widget event interactions.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge interaction add --help

```text
usage: axure-forge interaction add [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                   [--event EVENT]

Add an event interaction to a widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --event EVENT         Event name. (required unless provided by file context)

Required inputs: --scope-id, --node-id, --event. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge interaction catalogue --help

```text
usage: axure-forge interaction catalogue [-h] [--debug] [--project PROJECT]
                                         [-o OUTPUT] [--force]
                                         [--work-dir WORK_DIR]
                                         [--evidence-dir EVIDENCE_DIR]
                                         [--index INDEX_DIR] [--verify]
                                         [--fail-on {error,warn,none}]
                                         [--json JSON]
                                         [--library-path LIBRARY_PATH]

List supported events and interaction actions.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge interaction clear --help

```text
usage: axure-forge interaction clear [-h] [--debug] [--project PROJECT]
                                     [-o OUTPUT] [--force]
                                     [--work-dir WORK_DIR]
                                     [--evidence-dir EVIDENCE_DIR]
                                     [--index INDEX_DIR] [--verify]
                                     [--fail-on {error,warn,none}]
                                     [--json JSON]
                                     [--library-path LIBRARY_PATH]
                                     [--scope-id SCOPE_ID] [--node-id NODE_ID]

Clear widget event interactions.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge interaction get --help

```text
usage: axure-forge interaction get [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--scope-id SCOPE_ID] [--node-id NODE_ID]

Inspect widget event interactions.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge interaction set --help

```text
usage: axure-forge interaction set [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                   [--events EVENTS]

Replace widget event interactions.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --events EVENTS       Event interactions as a JSON object. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --events. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge interaction-style --help

```text
usage: axure-forge interaction-style [-h] [--debug] {clear,get,set} ...

Manage widget interaction styles.

positional arguments:
  {clear,get,set}
    clear          Clear interaction style overrides for a widget.
    get            Inspect interaction style overrides for a widget.
    set            Set interaction style overrides for a widget.

options:
  -h, --help       Show help and exit.
  --debug          Show diagnostic tracebacks on errors.
```

## axure-forge interaction-style clear --help

```text
usage: axure-forge interaction-style clear [-h] [--debug] [--project PROJECT]
                                           [-o OUTPUT] [--force]
                                           [--work-dir WORK_DIR]
                                           [--evidence-dir EVIDENCE_DIR]
                                           [--index INDEX_DIR] [--verify]
                                           [--fail-on {error,warn,none}]
                                           [--json JSON]
                                           [--library-path LIBRARY_PATH]
                                           [--scope-id SCOPE_ID]
                                           [--node-id NODE_ID] [--state STATE]

Clear interaction style overrides for a widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --state STATE         Interaction state name. (required unless provided by
                        file context)

Required inputs: --scope-id, --node-id, --state. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge interaction-style get --help

```text
usage: axure-forge interaction-style get [-h] [--debug] [--project PROJECT]
                                         [-o OUTPUT] [--force]
                                         [--work-dir WORK_DIR]
                                         [--evidence-dir EVIDENCE_DIR]
                                         [--index INDEX_DIR] [--verify]
                                         [--fail-on {error,warn,none}]
                                         [--json JSON]
                                         [--library-path LIBRARY_PATH]
                                         [--scope-id SCOPE_ID]
                                         [--node-id NODE_ID]

Inspect interaction style overrides for a widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge interaction-style set --help

```text
usage: axure-forge interaction-style set [-h] [--debug] [--project PROJECT]
                                         [-o OUTPUT] [--force]
                                         [--work-dir WORK_DIR]
                                         [--evidence-dir EVIDENCE_DIR]
                                         [--index INDEX_DIR] [--verify]
                                         [--fail-on {error,warn,none}]
                                         [--json JSON]
                                         [--library-path LIBRARY_PATH]
                                         [--scope-id SCOPE_ID]
                                         [--node-id NODE_ID] [--state STATE]
                                         [--style STYLE]

Set interaction style overrides for a widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --state STATE         Interaction state name. (required unless provided by
                        file context)
  --style STYLE         Style properties as a JSON object. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --state, --style. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge library --help

```text
usage: axure-forge library [-h] [--debug] {instantiate,register} ...

Register and instantiate local component templates.

positional arguments:
  {instantiate,register}
    instantiate         Create a template in a scope with supported overrides
                        applied atomically.
    register            Validate and register a local JSON template library
                        for this session.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge library instantiate --help

```text
usage: axure-forge library instantiate [-h] [--debug] [--project PROJECT]
                                       [-o OUTPUT] [--force]
                                       [--work-dir WORK_DIR]
                                       [--evidence-dir EVIDENCE_DIR]
                                       [--index INDEX_DIR] [--verify]
                                       [--fail-on {error,warn,none}]
                                       [--json JSON]
                                       [--library-path LIBRARY_PATH]
                                       [--scope-id SCOPE_ID]
                                       [--template-id TEMPLATE_ID]
                                       [--spec SPEC]

Create a template in a scope with supported overrides applied atomically.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --template-id TEMPLATE_ID
                        Registered component template ID. (required unless
                        provided by file context)
  --spec SPEC           Widget specification as a JSON object.

Required inputs: --scope-id, --template-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge library register --help

```text
usage: axure-forge library register [-h] [--debug] [--project PROJECT]
                                    [-o OUTPUT] [--force]
                                    [--work-dir WORK_DIR]
                                    [--evidence-dir EVIDENCE_DIR]
                                    [--index INDEX_DIR] [--verify]
                                    [--fail-on {error,warn,none}]
                                    [--json JSON]
                                    [--library-path LIBRARY_PATH]
                                    [--path PATH]

Validate and register a local JSON template library for this session.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --path PATH           Local file path. (required unless provided by file
                        context)

Required inputs: --path. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge master --help

```text
usage: axure-forge master [-h] [--debug]
                          {create,delete,get,instances,list,move,rename} ...

Manage reusable masters.

positional arguments:
  {create,delete,get,instances,list,move,rename}
    create              Create a master.
    delete              Delete a master.
    get                 Get a master.
    instances           List instances that reference a master.
    list                List masters.
    move                Move a master.
    rename              Rename a master.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge master create --help

```text
usage: axure-forge master create [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--project-index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH] [--name NAME]
                                 [--parent-id PARENT_ID] [--index INDEX]

Create a master.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --name NAME           Display name. (required unless provided by file
                        context)
  --parent-id PARENT_ID
                        Parent item or folder ID.
  --index INDEX         Position in the ordered collection.

Required inputs: --name. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge master delete --help

```text
usage: axure-forge master delete [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH]
                                 [--master-id MASTER_ID]

Delete a master.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --master-id MASTER_ID
                        Master ID. (required unless provided by file context)

Required inputs: --master-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master get --help

```text
usage: axure-forge master get [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                              [--force] [--work-dir WORK_DIR]
                              [--evidence-dir EVIDENCE_DIR]
                              [--index INDEX_DIR] [--verify]
                              [--fail-on {error,warn,none}] [--json JSON]
                              [--library-path LIBRARY_PATH]
                              [--master-id MASTER_ID]

Get a master.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --master-id MASTER_ID
                        Master ID. (required unless provided by file context)

Required inputs: --master-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master instances --help

```text
usage: axure-forge master instances [-h] [--debug] [--project PROJECT]
                                    [-o OUTPUT] [--force]
                                    [--work-dir WORK_DIR]
                                    [--evidence-dir EVIDENCE_DIR]
                                    [--index INDEX_DIR] [--verify]
                                    [--fail-on {error,warn,none}]
                                    [--json JSON]
                                    [--library-path LIBRARY_PATH]
                                    [--master-id MASTER_ID]

List instances that reference a master.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --master-id MASTER_ID
                        Master ID.

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge master list --help

```text
usage: axure-forge master list [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH]

List masters.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge master move --help

```text
usage: axure-forge master move [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--project-index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH]
                               [--master-id MASTER_ID] [--parent-id PARENT_ID]
                               [--index INDEX]

Move a master.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --master-id MASTER_ID
                        Master ID. (required unless provided by file context)
  --parent-id PARENT_ID
                        Parent item or folder ID.
  --index INDEX         Position in the ordered collection.

Required inputs: --master-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master rename --help

```text
usage: axure-forge master rename [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH]
                                 [--master-id MASTER_ID] [--name NAME]

Rename a master.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --master-id MASTER_ID
                        Master ID. (required unless provided by file context)
  --name NAME           Display name. (required unless provided by file
                        context)

Required inputs: --master-id, --name. Project context is supplied by --project
when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master-folder --help

```text
usage: axure-forge master-folder [-h] [--debug]
                                 {create,delete,get,move,rename} ...

Organize master folders.

positional arguments:
  {create,delete,get,move,rename}
    create              Create a master folder.
    delete              Delete a master folder.
    get                 Get a master folder.
    move                Move a master folder.
    rename              Rename a master folder.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge master-folder create --help

```text
usage: axure-forge master-folder create [-h] [--debug] [--project PROJECT]
                                        [-o OUTPUT] [--force]
                                        [--work-dir WORK_DIR]
                                        [--evidence-dir EVIDENCE_DIR]
                                        [--project-index INDEX_DIR] [--verify]
                                        [--fail-on {error,warn,none}]
                                        [--json JSON]
                                        [--library-path LIBRARY_PATH]
                                        [--name NAME] [--parent-id PARENT_ID]
                                        [--index INDEX]

Create a master folder.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --name NAME           Display name. (required unless provided by file
                        context)
  --parent-id PARENT_ID
                        Parent item or folder ID.
  --index INDEX         Position in the ordered collection.

Required inputs: --name. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge master-folder delete --help

```text
usage: axure-forge master-folder delete [-h] [--debug] [--project PROJECT]
                                        [-o OUTPUT] [--force]
                                        [--work-dir WORK_DIR]
                                        [--evidence-dir EVIDENCE_DIR]
                                        [--index INDEX_DIR] [--verify]
                                        [--fail-on {error,warn,none}]
                                        [--json JSON]
                                        [--library-path LIBRARY_PATH]
                                        [--folder-id FOLDER_ID]

Delete a master folder.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --folder-id FOLDER_ID
                        Folder ID. (required unless provided by file context)

Required inputs: --folder-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master-folder get --help

```text
usage: axure-forge master-folder get [-h] [--debug] [--project PROJECT]
                                     [-o OUTPUT] [--force]
                                     [--work-dir WORK_DIR]
                                     [--evidence-dir EVIDENCE_DIR]
                                     [--index INDEX_DIR] [--verify]
                                     [--fail-on {error,warn,none}]
                                     [--json JSON]
                                     [--library-path LIBRARY_PATH]
                                     [--folder-id FOLDER_ID]

Get a master folder.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --folder-id FOLDER_ID
                        Folder ID. (required unless provided by file context)

Required inputs: --folder-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master-folder move --help

```text
usage: axure-forge master-folder move [-h] [--debug] [--project PROJECT]
                                      [-o OUTPUT] [--force]
                                      [--work-dir WORK_DIR]
                                      [--evidence-dir EVIDENCE_DIR]
                                      [--project-index INDEX_DIR] [--verify]
                                      [--fail-on {error,warn,none}]
                                      [--json JSON]
                                      [--library-path LIBRARY_PATH]
                                      [--folder-id FOLDER_ID]
                                      [--parent-id PARENT_ID] [--index INDEX]

Move a master folder.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --folder-id FOLDER_ID
                        Folder ID. (required unless provided by file context)
  --parent-id PARENT_ID
                        Parent item or folder ID.
  --index INDEX         Position in the ordered collection.

Required inputs: --folder-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master-folder rename --help

```text
usage: axure-forge master-folder rename [-h] [--debug] [--project PROJECT]
                                        [-o OUTPUT] [--force]
                                        [--work-dir WORK_DIR]
                                        [--evidence-dir EVIDENCE_DIR]
                                        [--index INDEX_DIR] [--verify]
                                        [--fail-on {error,warn,none}]
                                        [--json JSON]
                                        [--library-path LIBRARY_PATH]
                                        [--folder-id FOLDER_ID] [--name NAME]

Rename a master folder.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --folder-id FOLDER_ID
                        Folder ID. (required unless provided by file context)
  --name NAME           Display name. (required unless provided by file
                        context)

Required inputs: --folder-id, --name. Project context is supplied by --project
when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master-instance --help

```text
usage: axure-forge master-instance [-h] [--debug]
                                   {clear-text-override,create,delete,detach,get,reset,set-text-override,text-overrides,update} ...

Manage master instances and overrides.

positional arguments:
  {clear-text-override,create,delete,detach,get,reset,set-text-override,text-overrides,update}
    clear-text-override
                        Remove the text override for a widget in a master
                        instance.
    create              Create a master instance.
    delete              Delete a master instance.
    detach              Replace a master instance with independent widgets.
    get                 Get a master instance.
    reset               Reset overrides on a master instance.
    set-text-override   Override widget text in a master instance.
    text-overrides      List text overrides on a master instance.
    update              Update a master instance.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge master-instance clear-text-override --help

```text
usage: axure-forge master-instance clear-text-override [-h] [--debug]
                                                       [--project PROJECT]
                                                       [-o OUTPUT] [--force]
                                                       [--work-dir WORK_DIR]
                                                       [--evidence-dir EVIDENCE_DIR]
                                                       [--index INDEX_DIR]
                                                       [--verify]
                                                       [--fail-on {error,warn,none}]
                                                       [--json JSON]
                                                       [--library-path LIBRARY_PATH]
                                                       [--scope-id SCOPE_ID]
                                                       [--node-id NODE_ID]
                                                       [--target-id TARGET_ID]
                                                       [--view-id VIEW_ID]

Remove the text override for a widget in a master instance.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --target-id TARGET_ID
                        Target widget ID. (required unless provided by file
                        context)
  --view-id VIEW_ID     Adaptive view ID.

Required inputs: --scope-id, --node-id, --target-id. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge master-instance create --help

```text
usage: axure-forge master-instance create [-h] [--debug] [--project PROJECT]
                                          [-o OUTPUT] [--force]
                                          [--work-dir WORK_DIR]
                                          [--evidence-dir EVIDENCE_DIR]
                                          [--index INDEX_DIR] [--verify]
                                          [--fail-on {error,warn,none}]
                                          [--json JSON]
                                          [--library-path LIBRARY_PATH]
                                          [--scope-id SCOPE_ID]
                                          [--master-id MASTER_ID]
                                          [--bounds BOUNDS] [--name NAME]
                                          [--options OPTIONS]

Create a master instance.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --master-id MASTER_ID
                        Master ID. (required unless provided by file context)
  --bounds BOUNDS       Widget geometry as a JSON object.
  --name NAME           Display name.
  --options OPTIONS     Behavior options as a JSON object.

Required inputs: --scope-id, --master-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master-instance delete --help

```text
usage: axure-forge master-instance delete [-h] [--debug] [--project PROJECT]
                                          [-o OUTPUT] [--force]
                                          [--work-dir WORK_DIR]
                                          [--evidence-dir EVIDENCE_DIR]
                                          [--index INDEX_DIR] [--verify]
                                          [--fail-on {error,warn,none}]
                                          [--json JSON]
                                          [--library-path LIBRARY_PATH]
                                          [--scope-id SCOPE_ID]
                                          [--node-id NODE_ID]

Delete a master instance.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master-instance detach --help

```text
usage: axure-forge master-instance detach [-h] [--debug] [--project PROJECT]
                                          [-o OUTPUT] [--force]
                                          [--work-dir WORK_DIR]
                                          [--evidence-dir EVIDENCE_DIR]
                                          [--index INDEX_DIR] [--verify]
                                          [--fail-on {error,warn,none}]
                                          [--json JSON]
                                          [--library-path LIBRARY_PATH]
                                          [--scope-id SCOPE_ID]
                                          [--node-id NODE_ID]

Replace a master instance with independent widgets.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master-instance get --help

```text
usage: axure-forge master-instance get [-h] [--debug] [--project PROJECT]
                                       [-o OUTPUT] [--force]
                                       [--work-dir WORK_DIR]
                                       [--evidence-dir EVIDENCE_DIR]
                                       [--index INDEX_DIR] [--verify]
                                       [--fail-on {error,warn,none}]
                                       [--json JSON]
                                       [--library-path LIBRARY_PATH]
                                       [--scope-id SCOPE_ID]
                                       [--node-id NODE_ID]

Get a master instance.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master-instance reset --help

```text
usage: axure-forge master-instance reset [-h] [--debug] [--project PROJECT]
                                         [-o OUTPUT] [--force]
                                         [--work-dir WORK_DIR]
                                         [--evidence-dir EVIDENCE_DIR]
                                         [--index INDEX_DIR] [--verify]
                                         [--fail-on {error,warn,none}]
                                         [--json JSON]
                                         [--library-path LIBRARY_PATH]
                                         [--scope-id SCOPE_ID]
                                         [--node-id NODE_ID]

Reset overrides on a master instance.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master-instance set-text-override --help

```text
usage: axure-forge master-instance set-text-override [-h] [--debug]
                                                     [--project PROJECT]
                                                     [-o OUTPUT] [--force]
                                                     [--work-dir WORK_DIR]
                                                     [--evidence-dir EVIDENCE_DIR]
                                                     [--index INDEX_DIR]
                                                     [--verify]
                                                     [--fail-on {error,warn,none}]
                                                     [--json JSON]
                                                     [--library-path LIBRARY_PATH]
                                                     [--scope-id SCOPE_ID]
                                                     [--node-id NODE_ID]
                                                     [--target-id TARGET_ID]
                                                     [--view-id VIEW_ID]
                                                     [--text TEXT]

Override widget text in a master instance.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --target-id TARGET_ID
                        Target widget ID. (required unless provided by file
                        context)
  --view-id VIEW_ID     Adaptive view ID.
  --text TEXT           Text content. (required unless provided by file
                        context)

Required inputs: --scope-id, --node-id, --target-id, --text. Project context
is supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge master-instance text-overrides --help

```text
usage: axure-forge master-instance text-overrides [-h] [--debug]
                                                  [--project PROJECT]
                                                  [-o OUTPUT] [--force]
                                                  [--work-dir WORK_DIR]
                                                  [--evidence-dir EVIDENCE_DIR]
                                                  [--index INDEX_DIR]
                                                  [--verify]
                                                  [--fail-on {error,warn,none}]
                                                  [--json JSON]
                                                  [--library-path LIBRARY_PATH]
                                                  [--scope-id SCOPE_ID]
                                                  [--node-id NODE_ID]

List text overrides on a master instance.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master-instance update --help

```text
usage: axure-forge master-instance update [-h] [--debug] [--project PROJECT]
                                          [-o OUTPUT] [--force]
                                          [--work-dir WORK_DIR]
                                          [--evidence-dir EVIDENCE_DIR]
                                          [--index INDEX_DIR] [--verify]
                                          [--fail-on {error,warn,none}]
                                          [--json JSON]
                                          [--library-path LIBRARY_PATH]
                                          [--scope-id SCOPE_ID]
                                          [--node-id NODE_ID]
                                          [--master-id MASTER_ID]
                                          [--bounds BOUNDS]
                                          [--options OPTIONS]

Update a master instance.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --master-id MASTER_ID
                        Master ID.
  --bounds BOUNDS       Widget geometry as a JSON object.
  --options OPTIONS     Behavior options as a JSON object.

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge master-tree --help

```text
usage: axure-forge master-tree [-h] [--debug] {get} ...

Inspect the master hierarchy.

positional arguments:
  {get}
    get       Inspect the master and master folder hierarchy.

options:
  -h, --help  Show help and exit.
  --debug     Show diagnostic tracebacks on errors.
```

## axure-forge master-tree get --help

```text
usage: axure-forge master-tree get [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]

Inspect the master and master folder hierarchy.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge menu --help

```text
usage: axure-forge menu [-h] [--debug]
                        {add-item,create-submenu,delete-item,delete-submenu,get-hierarchy,get-submenu,list-items,move-item,move-item-to} ...

Manage menus and nested items.

positional arguments:
  {add-item,create-submenu,delete-item,delete-submenu,get-hierarchy,get-submenu,list-items,move-item,move-item-to}
    add-item            Add an item to a menu.
    create-submenu      Create a submenu for a menu item.
    delete-item         Delete a menu item.
    delete-submenu      Delete the submenu of a menu item.
    get-hierarchy       Inspect the complete menu hierarchy.
    get-submenu         Inspect the submenu of a menu item.
    list-items          List items in a menu.
    move-item           Reorder a menu item.
    move-item-to        Move a menu item to another menu.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge menu add-item --help

```text
usage: axure-forge menu add-item [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--project-index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH]
                                 [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                 [--text TEXT] [--index INDEX]

Add an item to a menu.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --text TEXT           Text content. (required unless provided by file
                        context)
  --index INDEX         Position in the ordered collection.

Required inputs: --scope-id, --node-id, --text. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge menu create-submenu --help

```text
usage: axure-forge menu create-submenu [-h] [--debug] [--project PROJECT]
                                       [-o OUTPUT] [--force]
                                       [--work-dir WORK_DIR]
                                       [--evidence-dir EVIDENCE_DIR]
                                       [--index INDEX_DIR] [--verify]
                                       [--fail-on {error,warn,none}]
                                       [--json JSON]
                                       [--library-path LIBRARY_PATH]
                                       [--scope-id SCOPE_ID]
                                       [--node-id NODE_ID] [--item-id ITEM_ID]
                                       [--name NAME]

Create a submenu for a menu item.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --item-id ITEM_ID     Menu or tree item ID. (required unless provided by
                        file context)
  --name NAME           Display name.

Required inputs: --scope-id, --node-id, --item-id. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge menu delete-item --help

```text
usage: axure-forge menu delete-item [-h] [--debug] [--project PROJECT]
                                    [-o OUTPUT] [--force]
                                    [--work-dir WORK_DIR]
                                    [--evidence-dir EVIDENCE_DIR]
                                    [--project-index INDEX_DIR] [--verify]
                                    [--fail-on {error,warn,none}]
                                    [--json JSON]
                                    [--library-path LIBRARY_PATH]
                                    [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                    [--index INDEX] [--recursive RECURSIVE]

Delete a menu item.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --index INDEX         Position in the ordered collection. (required unless
                        provided by file context)
  --recursive RECURSIVE
                        Whether to include descendants (JSON boolean).

Required inputs: --scope-id, --node-id, --index. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge menu delete-submenu --help

```text
usage: axure-forge menu delete-submenu [-h] [--debug] [--project PROJECT]
                                       [-o OUTPUT] [--force]
                                       [--work-dir WORK_DIR]
                                       [--evidence-dir EVIDENCE_DIR]
                                       [--index INDEX_DIR] [--verify]
                                       [--fail-on {error,warn,none}]
                                       [--json JSON]
                                       [--library-path LIBRARY_PATH]
                                       [--scope-id SCOPE_ID]
                                       [--node-id NODE_ID] [--item-id ITEM_ID]

Delete the submenu of a menu item.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --item-id ITEM_ID     Menu or tree item ID. (required unless provided by
                        file context)

Required inputs: --scope-id, --node-id, --item-id. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge menu get-hierarchy --help

```text
usage: axure-forge menu get-hierarchy [-h] [--debug] [--project PROJECT]
                                      [-o OUTPUT] [--force]
                                      [--work-dir WORK_DIR]
                                      [--evidence-dir EVIDENCE_DIR]
                                      [--index INDEX_DIR] [--verify]
                                      [--fail-on {error,warn,none}]
                                      [--json JSON]
                                      [--library-path LIBRARY_PATH]
                                      [--scope-id SCOPE_ID]
                                      [--node-id NODE_ID]

Inspect the complete menu hierarchy.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge menu get-submenu --help

```text
usage: axure-forge menu get-submenu [-h] [--debug] [--project PROJECT]
                                    [-o OUTPUT] [--force]
                                    [--work-dir WORK_DIR]
                                    [--evidence-dir EVIDENCE_DIR]
                                    [--index INDEX_DIR] [--verify]
                                    [--fail-on {error,warn,none}]
                                    [--json JSON]
                                    [--library-path LIBRARY_PATH]
                                    [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                    [--item-id ITEM_ID]

Inspect the submenu of a menu item.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --item-id ITEM_ID     Menu or tree item ID. (required unless provided by
                        file context)

Required inputs: --scope-id, --node-id, --item-id. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge menu list-items --help

```text
usage: axure-forge menu list-items [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--scope-id SCOPE_ID] [--node-id NODE_ID]

List items in a menu.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge menu move-item --help

```text
usage: axure-forge menu move-item [-h] [--debug] [--project PROJECT]
                                  [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                  [--evidence-dir EVIDENCE_DIR]
                                  [--project-index INDEX_DIR] [--verify]
                                  [--fail-on {error,warn,none}] [--json JSON]
                                  [--library-path LIBRARY_PATH]
                                  [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                  [--index INDEX] [--to-index TO_INDEX]

Reorder a menu item.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --index INDEX         Position in the ordered collection. (required unless
                        provided by file context)
  --to-index TO_INDEX   Destination index. (required unless provided by file
                        context)

Required inputs: --scope-id, --node-id, --index, --to-index. Project context
is supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge menu move-item-to --help

```text
usage: axure-forge menu move-item-to [-h] [--debug] [--project PROJECT]
                                     [-o OUTPUT] [--force]
                                     [--work-dir WORK_DIR]
                                     [--evidence-dir EVIDENCE_DIR]
                                     [--project-index INDEX_DIR] [--verify]
                                     [--fail-on {error,warn,none}]
                                     [--json JSON]
                                     [--library-path LIBRARY_PATH]
                                     [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                     [--item-id ITEM_ID]
                                     [--target-menu-id TARGET_MENU_ID]
                                     [--index INDEX]

Move a menu item to another menu.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --item-id ITEM_ID     Menu or tree item ID. (required unless provided by
                        file context)
  --target-menu-id TARGET_MENU_ID
                        Destination menu ID. (required unless provided by file
                        context)
  --index INDEX         Position in the ordered collection.

Required inputs: --scope-id, --node-id, --item-id, --target-menu-id. Project
context is supplied by --project when needed. JSON values accept inline JSON
or a JSON file path.
```

## axure-forge node --help

```text
usage: axure-forge node [-h] [--debug]
                        {configure,create,delete,describe,get,group,list,move,properties,replace-image,set-reference-page,set-text-runs,style-text-span,ungroup,update} ...

Create, inspect, and edit widgets.

positional arguments:
  {configure,create,delete,describe,get,group,list,move,properties,replace-image,set-reference-page,set-text-runs,style-text-span,ungroup,update}
    configure           Configure widget properties and options.
    create              Create a widget.
    delete              Delete a widget.
    describe            Describe the widget schema for a supported kind.
    get                 Get a widget.
    group               Combine widgets into a group.
    list                List widgets.
    move                Move a widget.
    properties          Inspect widget property definitions.
    replace-image       Replace the image content of a widget.
    set-reference-page  Set the page referenced by a widget.
    set-text-runs       Replace widget text with formatted text runs.
    style-text-span     Apply text styling to a span of widget text.
    ungroup             Release the members of a widget group.
    update              Update a widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge node configure --help

```text
usage: axure-forge node configure [-h] [--debug] [--project PROJECT]
                                  [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                  [--evidence-dir EVIDENCE_DIR]
                                  [--index INDEX_DIR] [--verify]
                                  [--fail-on {error,warn,none}] [--json JSON]
                                  [--library-path LIBRARY_PATH]
                                  [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                  [--properties PROPERTIES]

Configure widget properties and options.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --properties PROPERTIES
                        Widget properties as a JSON object. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --properties. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge node create --help

```text
usage: axure-forge node create [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH]
                               [--scope-id SCOPE_ID] [--spec SPEC]

Create a widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --spec SPEC           Widget specification as a JSON object. (required
                        unless provided by file context)

Required inputs: --scope-id, --spec. Project context is supplied by --project
when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge node delete --help

```text
usage: axure-forge node delete [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH]
                               [--scope-id SCOPE_ID] [--node-id NODE_ID]

Delete a widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge node describe --help

```text
usage: axure-forge node describe [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH]
                                 [--scope-id SCOPE_ID] [--node-id NODE_ID]

Describe the widget schema for a supported kind.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge node get --help

```text
usage: axure-forge node get [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                            [--force] [--work-dir WORK_DIR]
                            [--evidence-dir EVIDENCE_DIR] [--index INDEX_DIR]
                            [--verify] [--fail-on {error,warn,none}]
                            [--json JSON] [--library-path LIBRARY_PATH]
                            [--scope-id SCOPE_ID] [--node-id NODE_ID]

Get a widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge node group --help

```text
usage: axure-forge node group [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                              [--force] [--work-dir WORK_DIR]
                              [--evidence-dir EVIDENCE_DIR]
                              [--index INDEX_DIR] [--verify]
                              [--fail-on {error,warn,none}] [--json JSON]
                              [--library-path LIBRARY_PATH]
                              [--scope-id SCOPE_ID] [--node-ids NODE_IDS]
                              [--name NAME]

Combine widgets into a group.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-ids NODE_IDS   Ordered widget IDs as a JSON array. (required unless
                        provided by file context)
  --name NAME           Display name.

Required inputs: --scope-id, --node-ids. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge node list --help

```text
usage: axure-forge node list [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                             [--force] [--work-dir WORK_DIR]
                             [--evidence-dir EVIDENCE_DIR] [--index INDEX_DIR]
                             [--verify] [--fail-on {error,warn,none}]
                             [--json JSON] [--library-path LIBRARY_PATH]
                             [--scope-id SCOPE_ID]

List widgets.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)

Required inputs: --scope-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge node move --help

```text
usage: axure-forge node move [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                             [--force] [--work-dir WORK_DIR]
                             [--evidence-dir EVIDENCE_DIR] [--index INDEX_DIR]
                             [--verify] [--fail-on {error,warn,none}]
                             [--json JSON] [--library-path LIBRARY_PATH]
                             [--scope-id SCOPE_ID] [--node-id NODE_ID]
                             [--position POSITION]

Move a widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --position POSITION   Insertion position. (required unless provided by file
                        context)

Required inputs: --scope-id, --node-id, --position. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge node properties --help

```text
usage: axure-forge node properties [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--scope-id SCOPE_ID] [--node-id NODE_ID]

Inspect widget property definitions.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge node replace-image --help

```text
usage: axure-forge node replace-image [-h] [--debug] [--project PROJECT]
                                      [-o OUTPUT] [--force]
                                      [--work-dir WORK_DIR]
                                      [--evidence-dir EVIDENCE_DIR]
                                      [--index INDEX_DIR] [--verify]
                                      [--fail-on {error,warn,none}]
                                      [--json JSON]
                                      [--library-path LIBRARY_PATH]
                                      [--scope-id SCOPE_ID]
                                      [--node-id NODE_ID] [--image IMAGE]

Replace the image content of a widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --image IMAGE         Image specification as a JSON object. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --image. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge node set-reference-page --help

```text
usage: axure-forge node set-reference-page [-h] [--debug] [--project PROJECT]
                                           [-o OUTPUT] [--force]
                                           [--work-dir WORK_DIR]
                                           [--evidence-dir EVIDENCE_DIR]
                                           [--index INDEX_DIR] [--verify]
                                           [--fail-on {error,warn,none}]
                                           [--json JSON]
                                           [--library-path LIBRARY_PATH]
                                           [--scope-id SCOPE_ID]
                                           [--node-id NODE_ID]
                                           [--page-id PAGE_ID]

Set the page referenced by a widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --page-id PAGE_ID     Page ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id, --page-id. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge node set-text-runs --help

```text
usage: axure-forge node set-text-runs [-h] [--debug] [--project PROJECT]
                                      [-o OUTPUT] [--force]
                                      [--work-dir WORK_DIR]
                                      [--evidence-dir EVIDENCE_DIR]
                                      [--index INDEX_DIR] [--verify]
                                      [--fail-on {error,warn,none}]
                                      [--json JSON]
                                      [--library-path LIBRARY_PATH]
                                      [--scope-id SCOPE_ID]
                                      [--node-id NODE_ID] [--runs RUNS]

Replace widget text with formatted text runs.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --runs RUNS           Formatted text runs as a JSON array. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --runs. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge node style-text-span --help

```text
usage: axure-forge node style-text-span [-h] [--debug] [--project PROJECT]
                                        [-o OUTPUT] [--force]
                                        [--work-dir WORK_DIR]
                                        [--evidence-dir EVIDENCE_DIR]
                                        [--index INDEX_DIR] [--verify]
                                        [--fail-on {error,warn,none}]
                                        [--json JSON]
                                        [--library-path LIBRARY_PATH]
                                        [--scope-id SCOPE_ID]
                                        [--node-id NODE_ID] [--span SPAN]
                                        [--style STYLE]

Apply text styling to a span of widget text.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --span SPAN           Text span definition as a JSON object.
  --style STYLE         Style properties as a JSON object. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --style. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge node ungroup --help

```text
usage: axure-forge node ungroup [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                                [--force] [--work-dir WORK_DIR]
                                [--evidence-dir EVIDENCE_DIR]
                                [--index INDEX_DIR] [--verify]
                                [--fail-on {error,warn,none}] [--json JSON]
                                [--library-path LIBRARY_PATH]
                                [--scope-id SCOPE_ID] [--node-id NODE_ID]

Release the members of a widget group.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge node update --help

```text
usage: axure-forge node update [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH]
                               [--scope-id SCOPE_ID] [--node-id NODE_ID]
                               [--changes CHANGES]

Update a widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --changes CHANGES     Property changes as a JSON object. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --changes. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge page --help

```text
usage: axure-forge page [-h] [--debug]
                        {add-event,clear-events,create,delete,get,get-events,list,move,rename,select,set-events} ...

Manage pages and page events.

positional arguments:
  {add-event,clear-events,create,delete,get,get-events,list,move,rename,select,set-events}
    add-event           Add a page event interaction.
    clear-events        Clear page event interactions.
    create              Create a page.
    delete              Delete a page.
    get                 Get a page.
    get-events          Inspect page event interactions.
    list                List pages.
    move                Move a page.
    rename              Rename a page.
    select              Select the current page in a project.
    set-events          Replace page event interactions.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge page add-event --help

```text
usage: axure-forge page add-event [-h] [--debug] [--project PROJECT]
                                  [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                  [--evidence-dir EVIDENCE_DIR]
                                  [--index INDEX_DIR] [--verify]
                                  [--fail-on {error,warn,none}] [--json JSON]
                                  [--library-path LIBRARY_PATH]
                                  [--page-id PAGE_ID] [--event EVENT]

Add a page event interaction.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --event EVENT         Event name. (required unless provided by file context)

Required inputs: --page-id, --event. Project context is supplied by --project
when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge page clear-events --help

```text
usage: axure-forge page clear-events [-h] [--debug] [--project PROJECT]
                                     [-o OUTPUT] [--force]
                                     [--work-dir WORK_DIR]
                                     [--evidence-dir EVIDENCE_DIR]
                                     [--index INDEX_DIR] [--verify]
                                     [--fail-on {error,warn,none}]
                                     [--json JSON]
                                     [--library-path LIBRARY_PATH]
                                     [--page-id PAGE_ID]

Clear page event interactions.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)

Required inputs: --page-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge page create --help

```text
usage: axure-forge page create [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--project-index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH] [--name NAME]
                               [--index INDEX] [--parent-id PARENT_ID]

Create a page.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --name NAME           Display name. (required unless provided by file
                        context)
  --index INDEX         Position in the ordered collection.
  --parent-id PARENT_ID
                        Parent item or folder ID.

Required inputs: --name. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge page delete --help

```text
usage: axure-forge page delete [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH]
                               [--page-id PAGE_ID] [--recursive RECURSIVE]

Delete a page.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --recursive RECURSIVE
                        Whether to include descendants (JSON boolean).

Required inputs: --page-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge page get --help

```text
usage: axure-forge page get [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                            [--force] [--work-dir WORK_DIR]
                            [--evidence-dir EVIDENCE_DIR] [--index INDEX_DIR]
                            [--verify] [--fail-on {error,warn,none}]
                            [--json JSON] [--library-path LIBRARY_PATH]
                            [--page-id PAGE_ID]

Get a page.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)

Required inputs: --page-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge page get-events --help

```text
usage: axure-forge page get-events [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--page-id PAGE_ID]

Inspect page event interactions.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)

Required inputs: --page-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge page list --help

```text
usage: axure-forge page list [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                             [--force] [--work-dir WORK_DIR]
                             [--evidence-dir EVIDENCE_DIR] [--index INDEX_DIR]
                             [--verify] [--fail-on {error,warn,none}]
                             [--json JSON] [--library-path LIBRARY_PATH]

List pages.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge page move --help

```text
usage: axure-forge page move [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                             [--force] [--work-dir WORK_DIR]
                             [--evidence-dir EVIDENCE_DIR]
                             [--project-index INDEX_DIR] [--verify]
                             [--fail-on {error,warn,none}] [--json JSON]
                             [--library-path LIBRARY_PATH] [--page-id PAGE_ID]
                             [--parent-id PARENT_ID] [--index INDEX]

Move a page.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --parent-id PARENT_ID
                        Parent item or folder ID.
  --index INDEX         Position in the ordered collection.

Required inputs: --page-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge page rename --help

```text
usage: axure-forge page rename [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH]
                               [--page-id PAGE_ID] [--name NAME]

Rename a page.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --name NAME           Display name. (required unless provided by file
                        context)

Required inputs: --page-id, --name. Project context is supplied by --project
when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge page select --help

```text
usage: axure-forge page select [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH]
                               [--page-id PAGE_ID]

Select the current page in a project.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)

Required inputs: --page-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge page set-events --help

```text
usage: axure-forge page set-events [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--page-id PAGE_ID] [--events EVENTS]

Replace page event interactions.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)
  --events EVENTS       Event interactions as a JSON object. (required unless
                        provided by file context)

Required inputs: --page-id, --events. Project context is supplied by --project
when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge page-tree --help

```text
usage: axure-forge page-tree [-h] [--debug] {get} ...

Inspect the page hierarchy.

positional arguments:
  {get}
    get       Inspect the page and folder hierarchy.

options:
  -h, --help  Show help and exit.
  --debug     Show diagnostic tracebacks on errors.
```

## axure-forge page-tree get --help

```text
usage: axure-forge page-tree get [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH]

Inspect the page and folder hierarchy.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge panel --help

```text
usage: axure-forge panel [-h] [--debug]
                         {add-state,create,delete,delete-state,get,get-state,list,move-state,rename-state,set-options} ...

Manage dynamic panels and their states.

positional arguments:
  {add-state,create,delete,delete-state,get,get-state,list,move-state,rename-state,set-options}
    add-state           Add a state to a dynamic panel.
    create              Create a panel.
    delete              Delete a panel.
    delete-state        Delete a dynamic panel state.
    get                 Get a panel.
    get-state           Inspect a dynamic panel state.
    list                List panels.
    move-state          Reorder a dynamic panel state.
    rename-state        Rename a dynamic panel state.
    set-options         Set dynamic panel behavior options.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge panel add-state --help

```text
usage: axure-forge panel add-state [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--project-index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                   [--name NAME] [--index INDEX]

Add a state to a dynamic panel.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --name NAME           Display name. (required unless provided by file
                        context)
  --index INDEX         Position in the ordered collection.

Required inputs: --scope-id, --node-id, --name. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge panel create --help

```text
usage: axure-forge panel create [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                                [--force] [--work-dir WORK_DIR]
                                [--evidence-dir EVIDENCE_DIR]
                                [--index INDEX_DIR] [--verify]
                                [--fail-on {error,warn,none}] [--json JSON]
                                [--library-path LIBRARY_PATH]
                                [--scope-id SCOPE_ID] [--bounds BOUNDS]
                                [--states STATES] [--options OPTIONS]
                                [--name NAME]

Create a panel.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --bounds BOUNDS       Widget geometry as a JSON object. (required unless
                        provided by file context)
  --states STATES       Dynamic panel state definitions as a JSON array.
                        (required unless provided by file context)
  --options OPTIONS     Behavior options as a JSON object.
  --name NAME           Display name.

Required inputs: --scope-id, --bounds, --states. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge panel delete --help

```text
usage: axure-forge panel delete [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                                [--force] [--work-dir WORK_DIR]
                                [--evidence-dir EVIDENCE_DIR]
                                [--index INDEX_DIR] [--verify]
                                [--fail-on {error,warn,none}] [--json JSON]
                                [--library-path LIBRARY_PATH]
                                [--scope-id SCOPE_ID] [--node-id NODE_ID]

Delete a panel.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge panel delete-state --help

```text
usage: axure-forge panel delete-state [-h] [--debug] [--project PROJECT]
                                      [-o OUTPUT] [--force]
                                      [--work-dir WORK_DIR]
                                      [--evidence-dir EVIDENCE_DIR]
                                      [--index INDEX_DIR] [--verify]
                                      [--fail-on {error,warn,none}]
                                      [--json JSON]
                                      [--library-path LIBRARY_PATH]
                                      [--scope-id SCOPE_ID]
                                      [--node-id NODE_ID]
                                      [--state-id STATE_ID]

Delete a dynamic panel state.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --state-id STATE_ID   Dynamic panel state ID. (required unless provided by
                        file context)

Required inputs: --scope-id, --node-id, --state-id. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge panel get --help

```text
usage: axure-forge panel get [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                             [--force] [--work-dir WORK_DIR]
                             [--evidence-dir EVIDENCE_DIR] [--index INDEX_DIR]
                             [--verify] [--fail-on {error,warn,none}]
                             [--json JSON] [--library-path LIBRARY_PATH]
                             [--scope-id SCOPE_ID] [--node-id NODE_ID]

Get a panel.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge panel get-state --help

```text
usage: axure-forge panel get-state [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                   [--state-id STATE_ID]

Inspect a dynamic panel state.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --state-id STATE_ID   Dynamic panel state ID. (required unless provided by
                        file context)

Required inputs: --scope-id, --node-id, --state-id. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge panel list --help

```text
usage: axure-forge panel list [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                              [--force] [--work-dir WORK_DIR]
                              [--evidence-dir EVIDENCE_DIR]
                              [--index INDEX_DIR] [--verify]
                              [--fail-on {error,warn,none}] [--json JSON]
                              [--library-path LIBRARY_PATH]
                              [--scope-id SCOPE_ID]

List panels.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)

Required inputs: --scope-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge panel move-state --help

```text
usage: axure-forge panel move-state [-h] [--debug] [--project PROJECT]
                                    [-o OUTPUT] [--force]
                                    [--work-dir WORK_DIR]
                                    [--evidence-dir EVIDENCE_DIR]
                                    [--project-index INDEX_DIR] [--verify]
                                    [--fail-on {error,warn,none}]
                                    [--json JSON]
                                    [--library-path LIBRARY_PATH]
                                    [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                    [--state-id STATE_ID] [--index INDEX]

Reorder a dynamic panel state.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --state-id STATE_ID   Dynamic panel state ID. (required unless provided by
                        file context)
  --index INDEX         Position in the ordered collection. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --state-id, --index. Project context
is supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge panel rename-state --help

```text
usage: axure-forge panel rename-state [-h] [--debug] [--project PROJECT]
                                      [-o OUTPUT] [--force]
                                      [--work-dir WORK_DIR]
                                      [--evidence-dir EVIDENCE_DIR]
                                      [--index INDEX_DIR] [--verify]
                                      [--fail-on {error,warn,none}]
                                      [--json JSON]
                                      [--library-path LIBRARY_PATH]
                                      [--scope-id SCOPE_ID]
                                      [--node-id NODE_ID]
                                      [--state-id STATE_ID] [--name NAME]

Rename a dynamic panel state.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --state-id STATE_ID   Dynamic panel state ID. (required unless provided by
                        file context)
  --name NAME           Display name. (required unless provided by file
                        context)

Required inputs: --scope-id, --node-id, --state-id, --name. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge panel set-options --help

```text
usage: axure-forge panel set-options [-h] [--debug] [--project PROJECT]
                                     [-o OUTPUT] [--force]
                                     [--work-dir WORK_DIR]
                                     [--evidence-dir EVIDENCE_DIR]
                                     [--index INDEX_DIR] [--verify]
                                     [--fail-on {error,warn,none}]
                                     [--json JSON]
                                     [--library-path LIBRARY_PATH]
                                     [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                     [--options OPTIONS]

Set dynamic panel behavior options.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --options OPTIONS     Behavior options as a JSON object. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --options. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge project --help

```text
usage: axure-forge project [-h] [--debug]
                           {check-conversion,close,convert,create,export,open} ...

Create, open, export, and convert projects.

positional arguments:
  {check-conversion,close,convert,create,export,open}
    check-conversion    Check strict lossless conversion and report blockers
                        without editing.
    close               Close a project.
    convert             Create a separate converted project; reject
                        incompatible or unverified data.
    create              Create a project.
    export              Export a project.
    open                Open a project.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge project check-conversion --help

```text
usage: axure-forge project check-conversion [-h] [--debug] [--project PROJECT]
                                            [-o OUTPUT] [--force]
                                            [--work-dir WORK_DIR]
                                            [--evidence-dir EVIDENCE_DIR]
                                            [--index INDEX_DIR] [--verify]
                                            [--fail-on {error,warn,none}]
                                            [--json JSON]
                                            [--library-path LIBRARY_PATH]
                                            [--target-version TARGET_VERSION]

Check strict lossless conversion and report blockers without editing.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --target-version TARGET_VERSION
                        Destination RP format version. (required unless
                        provided by file context); choices: [9, 11]

Required inputs: --target-version. Project context is supplied by --project
when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge project close --help

```text
usage: axure-forge project close [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH]

Close a project.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge project convert --help

```text
usage: axure-forge project convert [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--target-version TARGET_VERSION]

Create a separate converted project; reject incompatible or unverified data.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --target-version TARGET_VERSION
                        Destination RP format version. (required unless
                        provided by file context); choices: [9, 11]

Required inputs: --target-version. Project context is supplied by --project
when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge project create --help

```text
usage: axure-forge project create [-h] [--debug] [--project PROJECT]
                                  [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                  [--evidence-dir EVIDENCE_DIR]
                                  [--index INDEX_DIR] [--verify]
                                  [--fail-on {error,warn,none}] [--json JSON]
                                  [--library-path LIBRARY_PATH] [--name NAME]
                                  [--first-page FIRST_PAGE]
                                  [--format-version FORMAT_VERSION]

Create a project.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --name NAME           Display name.
  --first-page FIRST_PAGE
                        Initial page name.
  --format-version FORMAT_VERSION
                        RP format version.; choices: [9, 11]

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge project export --help

```text
usage: axure-forge project export [-h] [--debug] [--project PROJECT]
                                  [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                  [--evidence-dir EVIDENCE_DIR]
                                  [--index INDEX_DIR] [--verify]
                                  [--fail-on {error,warn,none}] [--json JSON]
                                  [--library-path LIBRARY_PATH] [--path PATH]
                                  [--overwrite OVERWRITE]

Export a project.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --path PATH           Local file path. (required unless provided by file
                        context)
  --overwrite OVERWRITE
                        Whether export may overwrite its target (JSON
                        boolean).

Required inputs: --path. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge project open --help

```text
usage: axure-forge project open [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                                [--force] [--work-dir WORK_DIR]
                                [--evidence-dir EVIDENCE_DIR]
                                [--index INDEX_DIR] [--verify]
                                [--fail-on {error,warn,none}] [--json JSON]
                                [--library-path LIBRARY_PATH] [--path PATH]

Open a project.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --path PATH           Local file path. (required unless provided by file
                        context)

Required inputs: --path. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge reference --help

```text
usage: axure-forge reference [-h] [--debug]
                             {list,masters,resolve-master,resolve-package,widget-template} ...

Inspect and resolve library references.

positional arguments:
  {list,masters,resolve-master,resolve-package,widget-template}
    list                List references.
    masters             List masters available through library references.
    resolve-master      Resolve a referenced master.
    resolve-package     Resolve a referenced library package.
    widget-template     Read a reusable widget template from a reference.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge reference list --help

```text
usage: axure-forge reference list [-h] [--debug] [--project PROJECT]
                                  [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                  [--evidence-dir EVIDENCE_DIR]
                                  [--index INDEX_DIR] [--verify]
                                  [--fail-on {error,warn,none}] [--json JSON]
                                  [--library-path LIBRARY_PATH]
                                  [--page-id PAGE_ID]

List references.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --page-id PAGE_ID     Page ID. (required unless provided by file context)

Required inputs: --page-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge reference masters --help

```text
usage: axure-forge reference masters [-h] [--debug] [--project PROJECT]
                                     [-o OUTPUT] [--force]
                                     [--work-dir WORK_DIR]
                                     [--evidence-dir EVIDENCE_DIR]
                                     [--index INDEX_DIR] [--verify]
                                     [--fail-on {error,warn,none}]
                                     [--json JSON]
                                     [--library-path LIBRARY_PATH]

List masters available through library references.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge reference resolve-master --help

```text
usage: axure-forge reference resolve-master [-h] [--debug] [--project PROJECT]
                                            [-o OUTPUT] [--force]
                                            [--work-dir WORK_DIR]
                                            [--evidence-dir EVIDENCE_DIR]
                                            [--index INDEX_DIR] [--verify]
                                            [--fail-on {error,warn,none}]
                                            [--json JSON]
                                            [--library-path LIBRARY_PATH]
                                            [--master MASTER]

Resolve a referenced master.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --master MASTER       Master definition or reference as a JSON object.
                        (required unless provided by file context)

Required inputs: --master. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge reference resolve-package --help

```text
usage: axure-forge reference resolve-package [-h] [--debug]
                                             [--project PROJECT] [-o OUTPUT]
                                             [--force] [--work-dir WORK_DIR]
                                             [--evidence-dir EVIDENCE_DIR]
                                             [--index INDEX_DIR] [--verify]
                                             [--fail-on {error,warn,none}]
                                             [--json JSON]
                                             [--library-path LIBRARY_PATH]
                                             [--package-id PACKAGE_ID]

Resolve a referenced library package.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --package-id PACKAGE_ID
                        Master or library package ID. (required unless
                        provided by file context)

Required inputs: --package-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge reference widget-template --help

```text
usage: axure-forge reference widget-template [-h] [--debug]
                                             [--project PROJECT] [-o OUTPUT]
                                             [--force] [--work-dir WORK_DIR]
                                             [--evidence-dir EVIDENCE_DIR]
                                             [--index INDEX_DIR] [--verify]
                                             [--fail-on {error,warn,none}]
                                             [--json JSON]
                                             [--library-path LIBRARY_PATH]
                                             [--scope-id SCOPE_ID]
                                             [--node-id NODE_ID]

Read a reusable widget template from a reference.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge repeater --help

```text
usage: axure-forge repeater [-h] [--debug]
                            {configure,create,delete,get,get-data,get-options,set-data} ...

Manage repeaters, options, and data.

positional arguments:
  {configure,create,delete,get,get-data,get-options,set-data}
    configure           Configure repeater layout and behavior.
    create              Create a repeater.
    delete              Delete a repeater.
    get                 Get a repeater.
    get-data            Read repeater columns and rows.
    get-options         Inspect repeater layout and behavior options.
    set-data            Replace repeater columns and rows.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge repeater configure --help

```text
usage: axure-forge repeater configure [-h] [--debug] [--project PROJECT]
                                      [-o OUTPUT] [--force]
                                      [--work-dir WORK_DIR]
                                      [--evidence-dir EVIDENCE_DIR]
                                      [--index INDEX_DIR] [--verify]
                                      [--fail-on {error,warn,none}]
                                      [--json JSON]
                                      [--library-path LIBRARY_PATH]
                                      [--scope-id SCOPE_ID]
                                      [--node-id NODE_ID] [--options OPTIONS]

Configure repeater layout and behavior.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --options OPTIONS     Behavior options as a JSON object. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --options. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge repeater create --help

```text
usage: axure-forge repeater create [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--scope-id SCOPE_ID] [--bounds BOUNDS]
                                   [--columns COLUMNS] [--rows ROWS]
                                   [--name NAME] [--options OPTIONS]

Create a repeater.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --bounds BOUNDS       Widget geometry as a JSON object. (required unless
                        provided by file context)
  --columns COLUMNS     Repeater column definitions as a JSON array.
  --rows ROWS           Repeater data rows as a JSON array.
  --name NAME           Display name.
  --options OPTIONS     Behavior options as a JSON object.

Required inputs: --scope-id, --bounds. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge repeater delete --help

```text
usage: axure-forge repeater delete [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--scope-id SCOPE_ID] [--node-id NODE_ID]

Delete a repeater.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge repeater get --help

```text
usage: axure-forge repeater get [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                                [--force] [--work-dir WORK_DIR]
                                [--evidence-dir EVIDENCE_DIR]
                                [--index INDEX_DIR] [--verify]
                                [--fail-on {error,warn,none}] [--json JSON]
                                [--library-path LIBRARY_PATH]
                                [--scope-id SCOPE_ID] [--node-id NODE_ID]

Get a repeater.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge repeater get-data --help

```text
usage: axure-forge repeater get-data [-h] [--debug] [--project PROJECT]
                                     [-o OUTPUT] [--force]
                                     [--work-dir WORK_DIR]
                                     [--evidence-dir EVIDENCE_DIR]
                                     [--index INDEX_DIR] [--verify]
                                     [--fail-on {error,warn,none}]
                                     [--json JSON]
                                     [--library-path LIBRARY_PATH]
                                     [--scope-id SCOPE_ID] [--node-id NODE_ID]

Read repeater columns and rows.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge repeater get-options --help

```text
usage: axure-forge repeater get-options [-h] [--debug] [--project PROJECT]
                                        [-o OUTPUT] [--force]
                                        [--work-dir WORK_DIR]
                                        [--evidence-dir EVIDENCE_DIR]
                                        [--index INDEX_DIR] [--verify]
                                        [--fail-on {error,warn,none}]
                                        [--json JSON]
                                        [--library-path LIBRARY_PATH]
                                        [--scope-id SCOPE_ID]
                                        [--node-id NODE_ID]

Inspect repeater layout and behavior options.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge repeater set-data --help

```text
usage: axure-forge repeater set-data [-h] [--debug] [--project PROJECT]
                                     [-o OUTPUT] [--force]
                                     [--work-dir WORK_DIR]
                                     [--evidence-dir EVIDENCE_DIR]
                                     [--index INDEX_DIR] [--verify]
                                     [--fail-on {error,warn,none}]
                                     [--json JSON]
                                     [--library-path LIBRARY_PATH]
                                     [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                     [--columns COLUMNS] [--rows ROWS]

Replace repeater columns and rows.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --columns COLUMNS     Repeater column definitions as a JSON array. (required
                        unless provided by file context)
  --rows ROWS           Repeater data rows as a JSON array. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --columns, --rows. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge search --help

```text
usage: axure-forge search [-h] [--debug] {context,explore} ...

Find widgets and reusable templates.

positional arguments:
  {context,explore}
    context          Inspect a search result, its path, and directly related
                     items.
    explore          Find widgets or templates by name, text, and kind; return
                     scoped IDs and evidence.

options:
  -h, --help         Show help and exit.
  --debug            Show diagnostic tracebacks on errors.
```

## axure-forge search context --help

```text
usage: axure-forge search context [-h] [--debug] [--project PROJECT]
                                  [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                  [--evidence-dir EVIDENCE_DIR]
                                  [--index INDEX_DIR] [--verify]
                                  [--fail-on {error,warn,none}] [--json JSON]
                                  [--library-path LIBRARY_PATH]
                                  [--result-id RESULT_ID]
                                  [--relation-limit RELATION_LIMIT]

Inspect a search result, its path, and directly related items.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --result-id RESULT_ID
                        Search result ID returned by search explore. (required
                        unless provided by file context)
  --relation-limit RELATION_LIMIT
                        Maximum number of related search items.

Required inputs: --result-id. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge search explore --help

```text
usage: axure-forge search explore [-h] [--debug] [--project PROJECT]
                                  [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                  [--evidence-dir EVIDENCE_DIR]
                                  [--index INDEX_DIR] [--verify]
                                  [--fail-on {error,warn,none}] [--json JSON]
                                  [--library-path LIBRARY_PATH]
                                  [--query QUERY] [--category CATEGORY]
                                  [--kind KIND] [--limit LIMIT]

Find widgets or templates by name, text, and kind; return scoped IDs and
evidence.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --query QUERY         Search keywords. (required unless provided by file
                        context)
  --category CATEGORY   Search category filter.; choices: ['all', 'instance',
                        'template']
  --kind KIND           Widget kind.
  --limit LIMIT         Maximum number of search results.

Required inputs: --query. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge system --help

```text
usage: axure-forge system [-h] [--debug] {capabilities} ...

Inspect RP capabilities and protocol operations.

positional arguments:
  {capabilities}
    capabilities  Describe RP9/RP11 read/edit/write/conversion capabilities
                  and v3 operations.

options:
  -h, --help      Show help and exit.
  --debug         Show diagnostic tracebacks on errors.
```

## axure-forge system capabilities --help

```text
usage: axure-forge system capabilities [-h] [--debug] [--project PROJECT]
                                       [-o OUTPUT] [--force]
                                       [--work-dir WORK_DIR]
                                       [--evidence-dir EVIDENCE_DIR]
                                       [--index INDEX_DIR] [--verify]
                                       [--fail-on {error,warn,none}]
                                       [--json JSON]
                                       [--library-path LIBRARY_PATH]

Describe RP9/RP11 read/edit/write/conversion capabilities and v3 operations.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.

Required inputs: none. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge table --help

```text
usage: axure-forge table [-h] [--debug]
                         {edit-axis,get-cell,get-grid,update-cell} ...

Inspect and edit table cells and axes.

positional arguments:
  {edit-axis,get-cell,get-grid,update-cell}
    edit-axis           Insert, remove, or resize table rows or columns.
    get-cell            Inspect a table cell.
    get-grid            Inspect table rows, columns, and cells.
    update-cell         Update a table cell.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge table edit-axis --help

```text
usage: axure-forge table edit-axis [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--project-index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                   [--axis AXIS] [--mode MODE] [--index INDEX]
                                   [--to-index TO_INDEX] [--size SIZE]

Insert, remove, or resize table rows or columns.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --axis AXIS           Table axis to edit. (required unless provided by file
                        context); choices: ['row', 'column']
  --mode MODE           Operation mode. (required unless provided by file
                        context); choices: ['insert', 'delete', 'move',
                        'resize']
  --index INDEX         Position in the ordered collection. (required unless
                        provided by file context)
  --to-index TO_INDEX   Destination index.
  --size SIZE           Row or column size in pixels.

Required inputs: --scope-id, --node-id, --axis, --mode, --index. Project
context is supplied by --project when needed. JSON values accept inline JSON
or a JSON file path.
```

## axure-forge table get-cell --help

```text
usage: axure-forge table get-cell [-h] [--debug] [--project PROJECT]
                                  [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                  [--evidence-dir EVIDENCE_DIR]
                                  [--index INDEX_DIR] [--verify]
                                  [--fail-on {error,warn,none}] [--json JSON]
                                  [--library-path LIBRARY_PATH]
                                  [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                  [--row ROW] [--column COLUMN]

Inspect a table cell.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --row ROW             Table row index. (required unless provided by file
                        context)
  --column COLUMN       Table column index. (required unless provided by file
                        context)

Required inputs: --scope-id, --node-id, --row, --column. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge table get-grid --help

```text
usage: axure-forge table get-grid [-h] [--debug] [--project PROJECT]
                                  [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                  [--evidence-dir EVIDENCE_DIR]
                                  [--index INDEX_DIR] [--verify]
                                  [--fail-on {error,warn,none}] [--json JSON]
                                  [--library-path LIBRARY_PATH]
                                  [--scope-id SCOPE_ID] [--node-id NODE_ID]

Inspect table rows, columns, and cells.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge table update-cell --help

```text
usage: axure-forge table update-cell [-h] [--debug] [--project PROJECT]
                                     [-o OUTPUT] [--force]
                                     [--work-dir WORK_DIR]
                                     [--evidence-dir EVIDENCE_DIR]
                                     [--index INDEX_DIR] [--verify]
                                     [--fail-on {error,warn,none}]
                                     [--json JSON]
                                     [--library-path LIBRARY_PATH]
                                     [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                     [--row ROW] [--column COLUMN]
                                     [--changes CHANGES]

Update a table cell.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --row ROW             Table row index. (required unless provided by file
                        context)
  --column COLUMN       Table column index. (required unless provided by file
                        context)
  --changes CHANGES     Property changes as a JSON object. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --row, --column, --changes. Project
context is supplied by --project when needed. JSON values accept inline JSON
or a JSON file path.
```

## axure-forge tree --help

```text
usage: axure-forge tree [-h] [--debug]
                        {add-item,delete-item,list-items,move-item,update-item} ...

Manage tree widget items.

positional arguments:
  {add-item,delete-item,list-items,move-item,update-item}
    add-item            Add an item to a tree widget.
    delete-item         Delete an item from a tree widget.
    list-items          List the items of a tree widget.
    move-item           Move or reorder a tree item.
    update-item         Update a tree item.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge tree add-item --help

```text
usage: axure-forge tree add-item [-h] [--debug] [--project PROJECT]
                                 [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                 [--evidence-dir EVIDENCE_DIR]
                                 [--project-index INDEX_DIR] [--verify]
                                 [--fail-on {error,warn,none}] [--json JSON]
                                 [--library-path LIBRARY_PATH]
                                 [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                 [--text TEXT] [--parent-id PARENT_ID]
                                 [--index INDEX]

Add an item to a tree widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --text TEXT           Text content. (required unless provided by file
                        context)
  --parent-id PARENT_ID
                        Parent item or folder ID.
  --index INDEX         Position in the ordered collection.

Required inputs: --scope-id, --node-id, --text. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge tree delete-item --help

```text
usage: axure-forge tree delete-item [-h] [--debug] [--project PROJECT]
                                    [-o OUTPUT] [--force]
                                    [--work-dir WORK_DIR]
                                    [--evidence-dir EVIDENCE_DIR]
                                    [--index INDEX_DIR] [--verify]
                                    [--fail-on {error,warn,none}]
                                    [--json JSON]
                                    [--library-path LIBRARY_PATH]
                                    [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                    [--item-id ITEM_ID]
                                    [--recursive RECURSIVE]

Delete an item from a tree widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --item-id ITEM_ID     Menu or tree item ID. (required unless provided by
                        file context)
  --recursive RECURSIVE
                        Whether to include descendants (JSON boolean).

Required inputs: --scope-id, --node-id, --item-id. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge tree list-items --help

```text
usage: axure-forge tree list-items [-h] [--debug] [--project PROJECT]
                                   [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                   [--evidence-dir EVIDENCE_DIR]
                                   [--index INDEX_DIR] [--verify]
                                   [--fail-on {error,warn,none}] [--json JSON]
                                   [--library-path LIBRARY_PATH]
                                   [--scope-id SCOPE_ID] [--node-id NODE_ID]

List the items of a tree widget.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)

Required inputs: --scope-id, --node-id. Project context is supplied by
--project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge tree move-item --help

```text
usage: axure-forge tree move-item [-h] [--debug] [--project PROJECT]
                                  [-o OUTPUT] [--force] [--work-dir WORK_DIR]
                                  [--evidence-dir EVIDENCE_DIR]
                                  [--project-index INDEX_DIR] [--verify]
                                  [--fail-on {error,warn,none}] [--json JSON]
                                  [--library-path LIBRARY_PATH]
                                  [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                  [--item-id ITEM_ID] [--parent-id PARENT_ID]
                                  [--index INDEX]

Move or reorder a tree item.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --project-index INDEX_DIR
                        Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --item-id ITEM_ID     Menu or tree item ID. (required unless provided by
                        file context)
  --parent-id PARENT_ID
                        Parent item or folder ID.
  --index INDEX         Position in the ordered collection. (required unless
                        provided by file context)

Required inputs: --scope-id, --node-id, --item-id, --index. Project context is
supplied by --project when needed. JSON values accept inline JSON or a JSON
file path.
```

## axure-forge tree update-item --help

```text
usage: axure-forge tree update-item [-h] [--debug] [--project PROJECT]
                                    [-o OUTPUT] [--force]
                                    [--work-dir WORK_DIR]
                                    [--evidence-dir EVIDENCE_DIR]
                                    [--index INDEX_DIR] [--verify]
                                    [--fail-on {error,warn,none}]
                                    [--json JSON]
                                    [--library-path LIBRARY_PATH]
                                    [--scope-id SCOPE_ID] [--node-id NODE_ID]
                                    [--item-id ITEM_ID] [--text TEXT]
                                    [--expanded EXPANDED]

Update a tree item.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --scope-id SCOPE_ID   Page, master, or panel-state scope ID. (required
                        unless provided by file context)
  --node-id NODE_ID     Widget ID. (required unless provided by file context)
  --item-id ITEM_ID     Menu or tree item ID. (required unless provided by
                        file context)
  --text TEXT           Text content.
  --expanded EXPANDED   Whether the tree item is expanded (JSON boolean).

Required inputs: --scope-id, --node-id, --item-id. Project context is supplied
by --project when needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge web --help

```text
usage: axure-forge web [-h] [--debug] {capture,import,plan,prepare} ...

Prepare and import host-browser captures.

positional arguments:
  {capture,import,plan,prepare}
    capture             Assemble a host-browser result directory into a
                        validated portable snapshot, offline.
    import              Import an offline web plan as native pages, panels and
                        interactions, atomically.
    plan                Project a browser snapshot into editable nodes and
                        explicit region states, offline.
    prepare             Prepare scripts and tasks for an existing logged-in
                        host browser; no browser connection.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
```

## axure-forge web capture --help

```text
usage: axure-forge web capture [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH] [--input INPUT]

Assemble a host-browser result directory into a validated portable snapshot,
offline.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   Output snapshot/plan JSON or RP file.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --input INPUT         Host-browser capture directory. (required unless
                        provided by file context)

Required inputs: --input. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge web import --help

```text
usage: axure-forge web import [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                              [--force] [--work-dir WORK_DIR]
                              [--evidence-dir EVIDENCE_DIR]
                              [--index INDEX_DIR] [--verify]
                              [--fail-on {error,warn,none}] [--json JSON]
                              [--library-path LIBRARY_PATH]
                              [--format-version {9,11}] [--plan PLAN]

Import an offline web plan as native pages, panels and interactions,
atomically.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   Output snapshot/plan JSON or RP file.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --format-version {9,11}
                        Format for a new project (default: 9); existing
                        projects keep their version.
  --plan PLAN           Import plan as JSON or a JSON file path. (required
                        unless provided by file context)

Required inputs: --plan. Project context is supplied by --project when needed.
JSON values accept inline JSON or a JSON file path.
```

## axure-forge web plan --help

```text
usage: axure-forge web plan [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                            [--force] [--work-dir WORK_DIR]
                            [--evidence-dir EVIDENCE_DIR] [--index INDEX_DIR]
                            [--verify] [--fail-on {error,warn,none}]
                            [--json JSON] [--library-path LIBRARY_PATH]
                            [--snapshot SNAPSHOT]

Project a browser snapshot into editable nodes and explicit region states,
offline.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   Output snapshot/plan JSON or RP file.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --snapshot SNAPSHOT   Browser snapshot as JSON or a JSON file path.
                        (required unless provided by file context)

Required inputs: --snapshot. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge web prepare --help

```text
usage: axure-forge web prepare [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                               [--force] [--work-dir WORK_DIR]
                               [--evidence-dir EVIDENCE_DIR]
                               [--index INDEX_DIR] [--verify]
                               [--fail-on {error,warn,none}] [--json JSON]
                               [--library-path LIBRARY_PATH] [--config CONFIG]

Prepare scripts and tasks for an existing logged-in host browser; no browser
connection.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New preparation directory; existing directories are
                        never overwritten.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Optional local component library.
  --config CONFIG       Browser preparation configuration as JSON or a JSON
                        file path. (required unless provided by file context)

Required inputs: --config. Project context is supplied by --project when
needed. JSON values accept inline JSON or a JSON file path.
```

## axure-forge batch --help

```text
usage: axure-forge batch [-h] [--debug] [--project PROJECT] [-o OUTPUT]
                         [--force] [--work-dir WORK_DIR]
                         [--evidence-dir EVIDENCE_DIR] [--index INDEX_DIR]
                         [--verify] [--fail-on {error,warn,none}]
                         [--json JSON] [--library-path LIBRARY_PATH]
                         request

Execute atomic operations from a batch JSON file.

positional arguments:
  request               Protocol-v3 batch JSON file.

options:
  -h, --help            Show help and exit.
  --debug               Show diagnostic tracebacks on errors.
  --project PROJECT     Input RP file; never modified implicitly.
  -o, --output OUTPUT   New RP output path; existing paths require --force.
  --force               Explicitly allow overwriting the output path.
  --work-dir WORK_DIR   Data workspace (default: ./.forge).
  --evidence-dir EVIDENCE_DIR
                        Override the per-output evidence directory.
  --index INDEX_DIR     Read-only index; source SHA256 is checked before
                        editing.
  --verify              Reopen output and check structure/estimated layout in
                        this process.
  --fail-on {error,warn,none}
                        Verification gate (default: error).
  --json JSON           Write full response here and print a small summary.
  --library-path LIBRARY_PATH
                        Local component library; may be repeated.
```
