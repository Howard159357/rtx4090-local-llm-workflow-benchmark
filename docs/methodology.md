# Methodology

This benchmark is a practical RTX 4090 local workflow study. It measures how local GGUF models behave across coding, repair-loop coding, browser runtime QA, vision extraction, screenshot-to-web attempts, and context/VRAM scaling.

## Hardware And Runtime

- GPU class: RTX 4090 workstation.
- Runtime: local llama.cpp-based GGUF workflow.
- Guardrail: 23 GiB VRAM guard for comparable runs unless a result is explicitly marked as no-guard supplemental.
- Model format: GGUF, with quantization noted in the model name or model metadata table.

Exact hardware and runtime metadata are summarized in the reproducibility and provenance documents when recorded.

## Task Construction

Tasks are custom synthetic tasks created for this benchmark. They are not imported from HumanEval, MBPP, LiveCodeBench, or another public coding leaderboard. The task catalog documents each task's public name, family, input/output shape, validator type, and provenance notes.

ChatGPT assisted task and rubric drafting. It was not scored as a local solver and was not the judge.

## Evaluation Layers

### B1 First Pass

B1 means one first-pass attempt with no repair. It measures first-answer task completion under the chosen runtime and context setting.

### B2 Repair Loop

B2 means one repair round using validation feedback. It measures recovery after feedback, not pure first-answer quality.

### n=3 Repeatability

n=3 is practical repeatability evidence. It is not a statistical significance claim. Equal aggregate counts do not prove identical task-level outcomes.

### Browser Runtime Audit

Browser Runtime Audit checks completed browser-openable web/game artifacts in a real browser. It complements static validators because a task can pass a validator and still render poorly, throw console errors, or fail interaction checks.

Bridge note: earlier internal files may refer to this layer as Browser Audit v2. Public-facing materials call it Browser Runtime Audit.

### Vision Extraction

Vision extraction tasks ask a model to interpret synthetic UI screenshots into structured information. This is separate from generating a working website from a screenshot.

### Screenshot-To-Web

Screenshot-to-web tasks ask a model to generate a browser-openable artifact from a screenshot. One-off passes are treated as capability signals, not reliability claims unless repeated evidence supports them.

### Context Sweep

Context length is treated as an engineering budget. Standard plotted points are completed comparable configurations under the 23 GiB guard. No-guard supplemental attempts are documented separately.

## Scoring

Most coding tasks use deterministic validators. Browser Runtime Audit can include manual runtime review because browser usability cannot be fully captured by static test pass alone. Validation details are in `validation_ledger.md`.

## Limitations

The results are specific to this task set, local runtime, quantization choices, repair protocol, and hardware. They should be used as engineering evidence, not as universal model rankings.
