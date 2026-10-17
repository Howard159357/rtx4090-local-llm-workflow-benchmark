# Executive Summary

This project evaluates what is practically useful when running local LLM workflows on a single RTX 4090 workstation.

The goal is not to create a universal leaderboard. The goal is to study local model routing for coding, one-round repair, browser runtime validation, vision extraction, screenshot-to-web attempts, and context/VRAM constraints.

## Scope

- Hardware: one RTX 4090-class workstation.
- Runtime: local llama.cpp-based GGUF workflow.
- Task set: custom synthetic tasks designed for this project.
- Solvers: local GGUF models.
- ChatGPT: used for task/rubric drafting support, not scored as a local solver or used as the judge.

## Main Result

Different workflow layers favored different models and validation methods. First-pass coding, repair-loop coding, browser runtime usability, vision extraction, and context scaling should be read as separate engineering signals.

The strongest practical conclusion is not "one model wins." The useful conclusion is that local AI engineering needs routing, validation, and VRAM-aware deployment decisions.

## What Not To Overclaim

- These results do not prove universal model quality.
- Browser Runtime Audit samples are small and unequal.
- n=3 repeatability is not statistical significance.
- Vision extraction does not imply reliable screenshot-to-web generation.
- OpenClaw-style end-to-end benchmarking has not been completed in this evidence pack.
