# Limitations

This benchmark is intentionally practical and local. The limits matter.

## Hardware Scope

The study was run on a single RTX 4090-class workstation. Results may differ on other GPUs, CPU offload settings, driver versions, CUDA builds, llama.cpp versions, or memory policies.

## Model Scope

Only selected local GGUF models were evaluated. Model weights are not included. Quantization choices can materially change behavior.

## Task Scope

The tasks are custom synthetic tasks. They are useful for controlled local workflow evaluation, but they are not a substitute for broad public benchmarks or real production workload evaluation.

## Statistical Scope

n=3 is repeatability evidence, not statistical significance. It can reveal unstable behavior, but it should not be read as a formal confidence interval.

## Browser Runtime Audit Scope

Browser Runtime Audit applies only to completed browser-openable web/game artifacts. Sample sizes are small and unequal, so the browser audit chart is runtime QA evidence, not a definitive web-generation ranking.

## Vision Scope

Vision extraction and screenshot-to-web generation are separate capabilities. Success on six synthetic UI screenshot extraction tasks does not prove broad multimodal UI generation reliability.

## Context Scope

Longer context did not monotonically improve B1 completion in this setup. That does not mean long context is never useful; it means context length should be budgeted against VRAM, stability, and task need.

## OpenClaw Scope

OpenClaw-style end-to-end integration is a future experiment. This release does not contain a completed end-to-end OpenClaw benchmark.
