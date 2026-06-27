# Reproduce Browser Runtime Audit

## Scope

Browser Runtime Audit checks only completed browser-openable web or game artifacts. It does not apply to function-only tasks, text-only outputs, failed web/game outputs, or model runs that did not produce an artifact that can be opened in a browser.

## Required Inputs

- Completed HTML/CSS/JS artifacts from coding runs.
- A browser automation tool such as Playwright.
- Audit rules for:
  - page load success,
  - visible rendering,
  - console errors,
  - basic interaction behavior,
  - mobile layout sanity.

## Suggested Procedure

1. Open each completed web/game artifact in a browser.
2. Capture console errors and runtime exceptions.
3. Check that the primary surface renders visibly.
4. Exercise expected basic interactions.
5. Check at least one mobile viewport.
6. Mark the artifact as pass/fail for runtime usability.

## Interpretation

A validator pass is not the same as browser usability. Browser Runtime Audit is a QA layer after task validation, not a replacement for the benchmark score.

