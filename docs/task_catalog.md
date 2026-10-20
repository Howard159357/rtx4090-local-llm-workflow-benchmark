# Task Catalog

The public task catalog is available as a CSV table:

- [docs/assets/tables/task_catalog.csv](assets/tables/task_catalog.csv)
- [data/processed/task_catalog.csv](../data/processed/task_catalog.csv)

The table includes all public tasks used for this release package. It documents task identity, public name, task family, tested capability, input/output shape, prompt length, validator type, provenance, and caveats.

If a field could not be verified from the available public evidence, it is marked `unknown / not recorded`.

Some catalog fields remain partial in v1 because original run metadata was not recorded at that granularity.

## Task IDs And Names

Each row has a short `task_id` and a readable `public_task_name`. The charts and documents use the readable names; for example, `web_005_vision_checkout_recreation` is the screenshot-to-web task.

## Provenance

Tasks are custom synthetic benchmark tasks. They were not imported from HumanEval, MBPP, LiveCodeBench, or another public coding leaderboard. The task archetypes may be common, but task prompts, tests, screenshots, and edge cases are project-specific.
