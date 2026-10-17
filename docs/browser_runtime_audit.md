# Browser Runtime Audit

Browser Runtime Audit checks completed browser-openable web/game artifacts in a real browser.

It exists because validator pass is not enough. A generated artifact can pass a static or scripted check while still having layout problems, console errors, broken interactions, missing responsive behavior, or unusable game surfaces.

## When It Applies

Browser Runtime Audit applies only to completed browser-openable artifacts. It does not apply to pure function tasks, repo-edit tasks, failed web/game outputs, or text-only tasks with no browser artifact.

## What It Checks

- Runtime load behavior.
- Visible rendering.
- Console errors.
- Basic interaction changes.
- Mobile layout where relevant.
- Game/web surface usability when applicable.

## Small And Unequal Samples

The audited browser samples are small and unequal. These fractions are runtime QA evidence, not a definitive web-generation ranking:

- Qwen3-Coder: 3/4
- Devstral: 3/5
- Qwen3.6: 3/6
- GLM-4.7-Flash: 1/5

See the browser runtime chart in `docs/assets/charts/02_coding_vs_browser_nvidia_accent_final.png`.
