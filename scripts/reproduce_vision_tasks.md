# Reproduce Vision Tasks

## Scope

This benchmark separates:

- Vision extraction: read synthetic screenshots and extract structured information.
- Screenshot-to-web: generate a browser-openable web page from a screenshot.

These are not the same capability and should not be merged into one score.

## Required Inputs

- A local multimodal model setup with its required projection file when applicable.
- Synthetic screenshot inputs.
- Expected structured outputs or validation rubric.
- Browser Runtime Audit for screenshot-to-web artifacts.

## Suggested Procedure

1. Start the model with multimodal support enabled.
2. Run each screenshot extraction task.
3. Validate extracted fields against the expected answer.
4. For screenshot-to-web, inspect the generated browser artifact separately.
5. Repeat selected vision tasks three times when repeatability evidence is needed.

## Interpretation

A model may extract screenshot content well and still fail to generate a usable web implementation. Treat these as separate workflow routes.

