# Migration Batch 1

This is the first extraction batch for `bonfyre-embed`.

## Goal

Move the live `BonfyreEmbed` binary into its own public-facing repo while keeping both its core and system-level dependencies explicit.

## Batch Contents

### 1. `BonfyreEmbed`

Current source:

- `/Users/nickgonzales/Projects/bonfyre-oss/cmd/BonfyreEmbed`

Target:

- `cmd/bonfyre-embed/`

### 2. `libbonfyre` dependency slice

Current source:

- `/Users/nickgonzales/Projects/bonfyre-core/lib/libbonfyre`

Target:

- `vendor/bonfyre-core/lib/libbonfyre/`

## Acceptance Criteria

1. the embed binary builds from its extracted path
2. the local vendored `libbonfyre` builds
3. the Homebrew dependency note is preserved in repo docs
4. the repo can serve as a clean backlink target from the live Bonfyre page

## Progress

- imported:
  - `BonfyreEmbed`
  - vendored `libbonfyre` dependency slice
- verification:
  - vendored `libbonfyre` builds locally
  - `bonfyre-embed` builds from the extracted path
  - usage surface runs from the extracted binary
