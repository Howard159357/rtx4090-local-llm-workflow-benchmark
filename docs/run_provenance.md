# Run Provenance

This release is a curated public package assembled from the final benchmark evidence pack.

## Included Public Evidence

- Final public NVIDIA accent charts.
- Processed B1, B2, browser runtime, vision, and context CSVs.
- Task catalog and validation ledger.
- Context attempt matrix with no-guard supplemental status.
- Model hash metadata where recorded.
- Public methodology and reproduction notes.

## Supplemental Runs

Some 256K context attempts were documented as no-guard supplemental runs. They are not treated as ordinary 23 GiB guarded comparable points.

## Run Dates And Harness Version

The public package records the release assembly date as 2026-06-27. Some individual model file timestamps and run provenance details are available in processed metadata, but full raw local run logs are excluded.

Public charts identify the runtime as llama.cpp b9145 CUDA with GGUF models and a 23 GiB guard unless noted as no-guard supplemental.

## Result Files Used

The public interpretation is based on processed CSV summaries in `data/processed/` and matching copies in `docs/assets/tables/`.

## Not Included

- Model weights.
- Raw temporary logs.
- Complete model outputs for every run.
- Local caches.
- Private local paths.
- Intermediate visual style trials.

This is a public evidence package, not the full working directory.
