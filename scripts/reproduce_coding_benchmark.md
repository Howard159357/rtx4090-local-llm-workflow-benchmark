# Reproduce The Coding Benchmark

## Scope

This guide covers:

- B1 first-pass coding: one attempt, no repair.
- B2 repair loop: one repair round using validation feedback.
- n=3 repeatability: three runs used as practical stability evidence.

## Required Inputs

- Local GGUF model files.
- llama.cpp server or equivalent local inference endpoint.
- The synthetic coding task prompts and validators from your local benchmark workspace.
- A fixed generation configuration per model and context setting.

Model weights are not included in this package. Use `../docs/model_cards_and_hashes.md` and `../data/processed/model_hashes.csv` to identify tested local files and hashes.

## Suggested Procedure

1. Start the local inference server for one model and one context length.
2. Run every B1 task once with no repair feedback.
3. Record pass/fail, runtime notes, peak VRAM, and output artifact paths.
4. For B2, provide the validation feedback from the failed or incomplete first attempt and allow exactly one repair attempt.
5. Repeat the B1/B2 schedule three times for n=3 evidence.
6. Aggregate by task count, not by token count or subjective preference.

## Interpretation

B1 and B2 are different engineering signals:

- B1 measures first-pass execution quality.
- B2 measures whether the model can use validation feedback once.

Equal aggregate counts across repeated runs do not prove identical task-level outcomes.

