# bonfyre-embed

Semantic vector search and embedding entry repo for Bonfyre.

This repo is a public entry vector for the embedding surface:

- text embeddings
- ONNX Runtime inference
- SQLite-backed vector persistence
- local semantic search workflows

## Why This Exists

The live `BonfyreEmbed` runtime currently lives in:

- `/Users/nickgonzales/Projects/bonfyre-oss/cmd/BonfyreEmbed`

This repo gives that surface its own clear entry point so the Bonfyre page can link to it directly.

## Current Layout

- `cmd/bonfyre-embed/`
  - extracted embedding binary source
- `vendor/bonfyre-core/lib/libbonfyre/`
  - temporary local dependency slice for extraction validation
- `docs/`
  - extraction notes

## Dependency Note

This repo currently vendors only the minimum `bonfyre-core` dependency surface needed to build locally:

- `lib/libbonfyre`

`bonfyre-embed` also depends on local system libraries from Homebrew:

- `onnxruntime`
- `sqlite`

That makes this a slightly heavier entry repo than `bonfyre-core` or `bonfyre-intake`, but still a clean standalone entry vector.
