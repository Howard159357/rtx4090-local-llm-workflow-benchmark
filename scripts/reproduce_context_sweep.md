# Reproduce Context And VRAM Sweep

## Scope

The context sweep tests whether larger context settings improve B1 first-pass coding under one RTX 4090 setup.

Context lengths considered in this project include:

- 32K
- 64K
- 128K
- 256K

## Required Inputs

- Local GGUF model files.
- llama.cpp runtime.
- A fixed task set and fixed scoring method.
- Peak VRAM capture, for example through `nvidia-smi` sampling.

## Suggested Procedure

1. Select one model.
2. Start the runtime at 32K context and run the B1 task set.
3. Record score, failures, peak VRAM, and whether the run completed.
4. Repeat at 64K, 128K, and 256K where the system can load and complete safely.
5. Mark runs that exceed a guard separately from guarded runs.

## Interpretation

Longer context is an engineering budget. In this study, longer context did not monotonically improve B1 completion under the RTX 4090 setup. No-guard supplemental runs should be read separately from guarded runs.

