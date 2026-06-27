# Model Cards And Hashes

Public model metadata is available as:

- [docs/assets/tables/model_hashes.csv](assets/tables/model_hashes.csv)
- [data/processed/model_hashes.csv](../data/processed/model_hashes.csv)

The table includes model display identifiers, quantization-visible file names, file sizes, sanitized model-root paths, and hashes where recorded.

## Fields To Inspect

- `artifact_type`: model or multimodal projection artifact.
- `model_ids`: benchmark model identifier.
- `file_name`: local GGUF or projection file name used in this run.
- `bytes`: recorded file size.
- `sha256`: recorded file hash where available.
- `hash_status`: whether the hash was recorded from cache or computed evidence.

Source repositories and license references should be confirmed from the original model cards before reproduction or redistribution. This package does not redistribute model weights or upstream model assets.

## Important Notes

- Model weights are not included.
- Users must follow original model licenses.
- Quantization and runtime settings can change benchmark behavior.
- Hashes are provided for reproducibility of this local run, not as endorsement of a model distribution.

See [../THIRD_PARTY_MODELS.md](../THIRD_PARTY_MODELS.md).
