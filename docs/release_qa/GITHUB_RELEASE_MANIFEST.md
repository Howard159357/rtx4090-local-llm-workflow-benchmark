# GitHub Release Manifest

This staging package is prepared for a public GitHub release of the RTX 4090 Local LLM Workflow Benchmark.

- Repository name: `rtx4090-local-llm-workflow-benchmark`.
- Release version: `v0.1.0`.
- Author display name: Howard Liu (Chuan-Hao Liu).
- Formal citation author: Chuan-Hao Liu.
- Affiliation: Independent engineering project.

## Public Positioning

This is a practical local AI engineering stack study on a single RTX 4090 workstation. It is not a universal model leaderboard.

The evidence supports workflow-level decisions:

- Which local model was useful for first-pass coding.
- Which local model improved after one repair round.
- Why browser runtime validation is needed for web/game artifacts.
- Why vision extraction and screenshot-to-web generation should be treated separately.
- How context length and VRAM pressure shaped deployment choices.

## Included Top-Level Structure

- `README.md`: public project overview and reading guide.
- `docs/`: methodology, limitations, charts, processed table descriptions, and a lightweight HTML report.
- `docs/assets/charts/`: final public PNG/SVG charts.
- `docs/assets/tables/`: processed CSV evidence tables used by the docs.
- `data/processed/`: clean public CSV tables.
- `scripts/`: reproduction notes for rerunning the benchmark.
- `THIRD_PARTY_MODELS.md`: model-source and licensing caution notes.
- `LICENSE`: MIT License for code and scripts.
- `CONTENT_LICENSE.md`: CC BY 4.0 content and processed data license.
- `CITATION_DRAFT.cff`: draft citation metadata pending final repository URL.
- `docs/release_qa/RELEASE_NOTES.md`: public release notes.

## Included Evidence Tables

- `coding_leaderboard.csv`
- `b1_repeat_summary.csv`
- `b2_repair_summary.csv`
- `browser_runtime_audit_summary.csv`
- `vision_extraction_summary.csv`
- `vision_to_web_summary.csv`
- `context_sweep_summary.csv`
- `context_attempt_matrix.csv`
- `model_hashes.csv`
- `task_catalog.csv`
- `task_length_summary.csv`
- `validation_ledger.csv`

## Included Public Charts

- `01_experiment_map_nvidia_accent_final`
- `02_coding_vs_browser_nvidia_accent_final`
- `03_first_pass_repair_repeatability_nvidia_accent_final`
- `04_completion_vs_vram_nvidia_accent_final`
- `05_vision_extraction_vs_generation_nvidia_accent_final`
- `06_role_based_decision_matrix_nvidia_accent_final`

Both PNG and SVG are included for the six main charts.

## Licensing

- Code and scripts: MIT License.
- Documentation, charts, processed benchmark summaries, task catalog, validation ledger, report materials, public figures, and processed CSV summaries: CC BY 4.0.
- Third-party model weights: not included and not licensed by this repository.

## Not Included

This package intentionally excludes model weights, raw giant logs, local caches, private machine paths, intermediate drafts, rejected chart variants, internal review contact sheets, LinkedIn drafts, and unpublished internal prompts.

See `EXCLUDED_FILES.md` for the explicit exclusion rationale.

## Source Paths

This release is staged from the local public patch package and final benchmark evidence pack. Public evidence is included only as curated documentation, final charts, and processed CSV summaries. The package is not the entire local working directory.

## Known Limitations

- One RTX 4090 workstation.
- One local llama.cpp based GGUF harness.
- Custom synthetic task set.
- n=3 repeatability evidence is practical evidence, not statistical significance.
- Browser Runtime Audit samples are small and unequal.
- Screenshot-to-web one-off passes are capability signals, not reliability claims.

## Release Readiness

Status: ready for review.

Public release notes are listed in `docs/release_qa/RELEASE_NOTES.md`.
