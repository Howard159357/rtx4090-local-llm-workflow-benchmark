# Public Wording Scan

Scan date: 2026-06-27

## Result

No blocking public wording issues found.

## Files Scanned

All public Markdown, HTML, CSV, CFF, SVG, and root metadata files in `github_public_release_v1_final_review/` were scanned.

## Checked Categories

The package was scanned for outdated or misleading wording categories including:

- internal repair-aggregation labels,
- overconfident static-validation claims,
- unsupported efficiency metrics,
- global winner language,
- deployment-certification language,
- cloud-replacement language,
- universal-benchmark language,
- completed-OpenClaw-benchmark claims,
- claims that ChatGPT was a scored competitor,
- claims that local models universally completed all coding work.
- private Windows user paths

## Remaining Allowed Bridge Term

`docs/methodology.md` contains one explicit bridge note from the legacy internal browser-audit name to the public term `Browser Runtime Audit`.

This is intentional because public readers may see older internal filenames in evidence trails. The public term used throughout narrative materials is `Browser Runtime Audit`.

## Internal Task ID Occurrences

The legacy screenshot-to-web task identifier still appears in the task catalog, task length table, and validation ledger.

These occurrences are allowed because they are internal task identifiers in appendix-style evidence tables, not public narrative terms. Public-facing text refers to the task as a screenshot-to-web UI generation task.

The screenshot-to-web summary table now uses neutral evidence IDs such as `vtw_001` and does not expose raw run paths.

## ChatGPT Role Check

The package states that ChatGPT assisted task and rubric design. It does not state that ChatGPT was a scored local solver or the judge.

## OpenClaw Role Check

The package states that end-to-end OpenClaw-style integration remains a future experiment. It does not claim that an OpenClaw benchmark was completed.

## Path And Artifact Wording Check

Public CSV evidence paths were sanitized:

- raw run artifact path columns were removed from the screenshot-to-web summary,
- model hash paths use `<MODEL_ROOT>/models/...`,
- task length rows use `prompt_source_id` rather than unavailable prompt file paths,
- context attempt rows use `source_evidence_id` rather than source CSV file paths.

## Replacements Made

- Public terminology uses `Browser Runtime Audit`.
- Public narrative uses `screenshot-to-web task`.
- Public repair wording avoids internal aggregation labels.
- Author display uses Howard Liu (Chuan-Hao Liu).
- Formal citation and license use Chuan-Hao Liu.
