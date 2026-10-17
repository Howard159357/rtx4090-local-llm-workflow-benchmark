# Vision And Screenshot-To-Web

Vision extraction and screenshot-to-web generation are separate capabilities.

## Vision Extraction

The vision extraction layer uses six synthetic UI screenshots. The model is asked to interpret screenshots into structured information.

Observed extraction result:

- Devstral 24B: 6/6 extraction.
- Qwen3VL 8B: 6/6 extraction.
- Qwen3-Omni and Qwen3.6 plus multimodal projection reached 5/6 in the supported evidence.

This is screenshot-to-structured-data behavior, not proof of broad visual reasoning or production UI understanding.

## Screenshot-To-Web

Screenshot-to-web asks a model to generate a browser-openable artifact from a screenshot. Repeated screenshot-to-web did not pass reliably in this evidence pack.

Earlier one-off screenshot-to-web passes should be read as capability signals, not reliability claims.

Use `screenshot-to-web task` in public narrative. Internal task IDs may appear only in task catalog or appendix tables.
