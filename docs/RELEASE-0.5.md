# AxureForge CLI v0.5.0

## CLI interface

- Grouped top-level help lists every command with a description and the installed version. Bare invocation and bare command groups display help.
- Help, options, and CLI messages are in English; user-authored content stays unchanged.
- Errors preserve protocol-v3 JSON on stdout with concise stderr diagnostics. Tracebacks are hidden by default; `--debug` enables them at any command level. Ctrl-C exits with code 130.
- Startup, dependency loading, output writing, and cleanup failures use the same error boundary. Optional update notices cannot change a successful command result.

## Breaking command changes

Use `adaptive-view`, `adaptive-view-set`, `interaction-style`, `master-folder`, `master-instance`, `master-tree`, and `page-tree`. Old underscore spellings are rejected with replacement hints. Long options require their complete spelling. Internal operation names and JSON fields, including batch `master_instance.create`, remain unchanged.

## Web import and native widgets

This release also includes the current host-browser capture workflow (`web prepare`, `web capture --input`, `web plan`, `web import`), native composite widgets, and unified widget contracts. Browser capture uses existing host browser tools; the binary does not bundle a browser driver.

## Installation and compatibility

Download the full directory archive for macOS ARM64, Linux x64, or Windows x64 and verify it with `SHA256SUMS`. Keep `_internal` together with the executable. No Python installation is required. Binaries are unsigned and not notarized.

The matching AxureForge skill v0.5.0 requires CLI 0.5.0 or later and protocol v3. Existing release assets are unchanged. Runtime-free installation, offline update behavior, RP9/RP11 creation and conversion, and the optimized editing workflow are validated by the native build jobs; Axure GUI visual and interaction checks are separate.
