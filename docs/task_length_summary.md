# Task Length Summary

Task length data is available as:

- [docs/assets/tables/task_length_summary.csv](assets/tables/task_length_summary.csv)
- [data/processed/task_length_summary.csv](../data/processed/task_length_summary.csv)

The table includes prompt characters, prompt words, and approximate prompt token counts for each task where recorded.

Token counts are approximate and tokenizer-dependent. They should be used for relative prompt-length inspection, not exact billing or capacity estimates.

## Summary Statistics

- Task count: 30.
- Prompt characters: min 379, median 617.5, max 2330.
- Approximate prompt tokens: min 95, median 154.5, max 583.

## Longest Tasks By Prompt Characters

- Multi-page ordering website task.
- Screenshot-to-web UI generation task.
- Kitchen admin dashboard task.
- Tetris-style browser game task.
- Checkout form task.

## Shortest Tasks By Prompt Characters

- Refund policy repository task.
- Burger customization vision extraction task.
- Empty cart and delivery error vision extraction task.
- Desktop menu grid vision extraction task.
- Bowl customization vision extraction task.

## How To Use This Table

- Compare short function tasks with longer repo, web, game, and vision tasks.
- Identify long-context tasks that may stress memory or retrieval behavior.
- Interpret context sweep results alongside task length rather than treating context size as a model badge.

## Caveats

Prompt length is not the full runtime context. Some tasks also include starter files, images, or repository content. Approximate token counts are rough estimates and should not be interpreted as tokenizer-exact counts.
