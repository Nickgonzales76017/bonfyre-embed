<p align="center"><img src="https://github.com/user-attachments/assets/7785a8d6-6e28-4892-8958-3daf85414f05" width="80" alt="Bonfÿre knight" /></p>

# Bonfÿre Embed

**Local text embeddings and source-linked search tools.**

For an example of what a developer or customer can do with local search, start with the [Aurekai document workspace](https://aurekai-work-samples.pages.dev/documents/) or [local-first application guide](https://docs.aurekai.work/local-first-applications).

## What this source contains

This repository preserves an **April 2026 extraction** of the embedding interface, with `cmd/bonfyre-embed/`, temporary vendored library dependencies and extraction notes. It is useful for reading and extending the original native implementation, but is not a separately versioned or supported package release.

The canonical integrated source lives at [Bonfÿre / cmd/BonfyreEmbed](https://github.com/Nickgonzales76017/bonfyre/tree/main/cmd/BonfyreEmbed). Development after the public snapshot is moving through its own source and privacy review; this older extraction does not automatically reflect those changes.

Native embedding requires compatible model files, representation/dimension choices, and actual installed dependencies (including ONNX Runtime where used). Source paths and model requirements should be checked for the exact version being built. An embedding is not, on its own, a verified answer or a license to inspect another owner's data.

## Related uses

- [Search a local document collection](https://aurekai-work-samples.pages.dev/documents/) — paragraphs and cited notes
- [Bonfÿre native implementation](https://github.com/Nickgonzales76017/bonfyre) — embedding, vector storage, CMS, work and evidence owners
- [Integration and migration guide](https://docs.aurekai.work/integration-and-migration) — moving results into an existing customer application
- [Aurekai service examples](https://aurekai-work-samples.pages.dev/) — working browser applications

This extraction retains its original notices; the current Bonfÿre repository and independent components have their own licensing terms.
