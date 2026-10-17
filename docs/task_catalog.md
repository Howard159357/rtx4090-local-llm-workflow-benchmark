# Task Catalog

The public task catalog is available as a CSV table:

- [docs/assets/tables/task_catalog.csv](assets/tables/task_catalog.csv)
- [data/processed/task_catalog.csv](../data/processed/task_catalog.csv)

The table includes all public tasks used for this release package. It documents task identity, public name, task family, tested capability, input/output shape, prompt length, validator type, provenance, and caveats.

If a field could not be verified from the available public evidence, it is marked `unknown / not recorded`.

Some catalog fields remain partial in v1 because original run metadata was not recorded at that granularity.

## Internal And Public Names

Some task IDs are internal identifiers. For public writing, use `public_task_name`.

The internal task ID `web005` may appear in the catalog as an internal identifier. In public narrative, refer to it as a screenshot-to-web UI generation task.

## Provenance

Tasks are custom synthetic benchmark tasks. They were not imported from HumanEval, MBPP, LiveCodeBench, or another public coding leaderboard. The task archetypes may be common, but task prompts, tests, screenshots, and edge cases are project-specific.
