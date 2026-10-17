# Reproduction Notes

This folder currently contains reproduction notes, not a fully automated benchmark runner.

The original benchmark was run on a local Windows RTX 4090 workstation using a llama.cpp GGUF workflow. Model weights, local batch files, private paths, raw giant logs, screenshots from rejected drafts, and local caches are intentionally excluded from this public package.

Use these notes to rebuild the setup in your own environment:

- `reproduce_coding_benchmark.md`: B1 first-pass and B2 repair-loop coding runs.
- `reproduce_browser_runtime_audit.md`: browser runtime QA for completed web/game artifacts.
- `reproduce_vision_tasks.md`: vision extraction and screenshot-to-web checks.
- `reproduce_context_sweep.md`: context length and VRAM sweep.

The included CSV files are processed evidence tables. They are suitable for review, plotting, and methodology inspection, but they are not a substitute for running the models again on your own machine.
