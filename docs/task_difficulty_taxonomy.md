# Task Difficulty Taxonomy

Difficulty in this release is descriptive, not absolute.

Two concepts are separated:

## Design Complexity

Design complexity describes what the task was intended to require.

- `simple`: narrow implementation or extraction surface.
- `medium`: multiple rules, files, UI states, or interaction paths.
- `hard`: larger integration surface, longer context, or more complex behavior.

## Observed Difficulty

Observed difficulty describes how this model set behaved under this benchmark protocol.

- `easy`: most tested models completed it.
- `medium`: mixed results.
- `hard`: few models completed it.
- `separator`: useful for distinguishing stronger workflows.
- `unsolved`: no listed model completed it under the tested protocol.
- `insufficient_data`: not enough runs to interpret.

Observed difficulty depends on this model set, hardware, validators, repair protocol, and runtime settings. It should not be treated as a universal property of the task.
