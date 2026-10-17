# Reproducibility

This public package includes processed evidence and reproduction notes. It does not include model weights, raw temporary logs, private local paths, or complete model outputs.

## Environment

- Hardware class: RTX 4090 workstation.
- GPU: NVIDIA GeForce RTX 4090.
- Recorded driver: 591.86.
- Recorded VRAM: approximately 24,564 MiB.
- Runtime: local llama.cpp-based GGUF workflow.
- llama.cpp build identifier used in public charts: b9145 CUDA.
- Guard: 23 GiB VRAM for comparable runs unless marked no-guard supplemental.
- Model weights: not included.

## What You Can Reproduce From This Package

- Inspect final public charts.
- Inspect processed CSV evidence.
- Recreate the public interpretation from the validation ledger, task catalog, context matrix, and summaries.
- Re-run similar tasks if you recreate the local model environment and task harness.

## What Requires Local Setup

- Downloading GGUF models from original providers or distributors.
- Matching quantization files and, where applicable, multimodal projection files.
- Matching llama.cpp build and runtime flags.
- Running validators and Browser Runtime Audit on generated artifacts.

## Reproduction Sketch

1. Prepare the local GGUF model file and any required multimodal projection file.
2. Start a llama.cpp-compatible local inference endpoint with the selected context length.
3. Run the custom synthetic task prompt through the benchmark harness.
4. Apply the deterministic task validator where available.
5. For completed web/game artifacts, run Browser Runtime Audit.
6. Record peak VRAM and classify the run as guarded comparable or no-guard supplemental.

## Model Hashes

Model file hashes are included where recorded:

- [docs/assets/tables/model_hashes.csv](assets/tables/model_hashes.csv)
- [data/processed/model_hashes.csv](../data/processed/model_hashes.csv)

The hash table identifies local files used during the study. It does not redistribute model weights.

## Task Set And Harness Caveat

The full raw local harness and complete model outputs are not included in this public package. This release is intended to support public review of processed evidence, methodology, charts, and reproducibility constraints.
