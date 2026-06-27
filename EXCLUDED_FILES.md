# Excluded Files

This release package is curated. It is not a full workspace archive.

## Excluded By Design

| Category | Reason |
| --- | --- |
| GGUF model weights | Large third-party files with separate licenses and distribution rules. |
| Multimodal projection files | Same reason as model weights; users should download from official model sources. |
| Raw giant logs | Too large, noisy, and may contain local paths or transient runtime details. |
| Local llama.cpp batch files | They contain machine-specific paths and are not portable. |
| Private absolute paths | Public package should not expose local workstation details. |
| Download caches | Not evidence and not reproducible documentation. |
| Temporary screenshots and drafts | Only final public charts are included. |
| LinkedIn drafts | Kept out of the public GitHub package to avoid stale publication copy. |
| Internal chart contact sheets | Review-only wording is not suitable for the public repo. |
| Internal review zips | Superseded by this public staging package. |
| Failed or abandoned visual variants | Not needed for public review. |

## Excluded Source Examples

The original workspace contains many useful working files that are intentionally not copied into this package:

- `*.gguf`
- `*.zip` review bundles
- browser screenshot archives
- raw logs
- local server launch files
- old chart style trials
- old prompt drafts
- LinkedIn publication drafts
- internal visual review contact sheets

## What To Publish Instead

Publish the contents of `github_public_release_v1_final_review/` as the public GitHub repository.

The zip file is only for transfer and review. Do not commit the zip file into the repository.

This keeps the public artifact focused on reproducible evidence, public charts, methodology, and practical interpretation.
