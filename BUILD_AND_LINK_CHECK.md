# Build And Link Check

Scan date: 2026-06-27

## Package Size Check

At final check before zipping, the final review package contained:

- 69 files
- approximately 0.83 MB

This confirms that model weights, raw giant logs, and heavy review archives were not copied into the release package.

## Local Link Check

Markdown and HTML relative links were checked inside `github_public_release_v1_final_review/`.

Result:

```text
LINK_CHECK_OK
```

## Private Path Check

The package was scanned for local user-profile paths and temporary attachment paths, including Windows user directory patterns, app-data folders, download folders, Codex remote attachment paths, and clipboard-temp paths.

Result: no matches.

## Heavy Artifact Check

The package was scanned for excluded heavy/runtime artifacts:

- `.gguf`
- `.safetensors`
- `.bin`
- `.pt`
- `.pth`
- `.onnx`
- `.zip`
- `.log`

Result: no included files with those extensions.

## HTML Report

The HTML report is included at:

- `docs/index.html`

It references only local assets inside the package.

## Public Patch Checks

Confirmed:

- no broken relative links,
- no Windows absolute paths,
- no model weights,
- no local logs,
- no internal review zips,
- no outdated LinkedIn drafts,
- no obsolete chart variants,
- final six charts included as PNG and SVG,
- task catalog included,
- validation ledger included,
- prompt length summary included,
- context attempt matrix included.

## Duplicate File Check

The only duplicate-content files found are intentional mirror copies of processed CSV tables:

- `data/processed/*.csv`
- `docs/assets/tables/*.csv`

This duplication is intentional so users can read data from the repository-level data folder or from documentation-relative table links.
