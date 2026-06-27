# Context And VRAM Attempt Matrix

The context attempt matrix is available as:

- [docs/assets/tables/context_attempt_matrix.csv](assets/tables/context_attempt_matrix.csv)
- [data/processed/context_attempt_matrix.csv](../data/processed/context_attempt_matrix.csv)

It documents context length attempts, whether a configuration completed, peak VRAM when recorded, and whether a point was comparable under the 23 GiB guard or a no-guard supplemental attempt.

## Interpretation Rule

Only completed comparable configurations under the 23 GiB guard are plotted as standard points. Supplemental no-guard attempts are documented separately.

Do not infer that every missing point was out of memory unless the attempt status explicitly supports that.

## Deployment Lesson

In this setup, longer context did not monotonically improve B1 first-pass completion. Context length should be treated as an engineering budget that competes with VRAM, stability, and throughput.
