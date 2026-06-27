# Validation Ledger

The validation ledger is one of the core evidence files in this release:

- [docs/assets/tables/validation_ledger.csv](assets/tables/validation_ledger.csv)
- [data/processed/validation_ledger.csv](../data/processed/validation_ledger.csv)

It records task-level validation type, validator path, whether deterministic validation was used, whether Browser Runtime Audit applied, and whether human review was required.

## ChatGPT Role

ChatGPT assisted task and rubric drafting. It was not a scored local solver and was not used as the judge in this evidence pack.

## Deterministic And Manual Layers

Coding and many structured tasks use deterministic validators. Browser-openable artifacts may also require runtime QA because passing a validator does not guarantee usable browser behavior.

When a field could not be verified from the available public evidence, it is marked `unknown / not recorded`.
