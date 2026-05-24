# Tokio: tokio-stream/src

## Purpose

Source root for stream wrappers and StreamExt utilities.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `stream_ext/`
- `wrappers/`

## Key Files

- `empty.rs`
- `iter.rs`
- `lib.rs`
- `macros.rs`
- `once.rs`
- `pending.rs`
- `stream_close.rs`
- `stream_ext.rs`
- `stream_map.rs`
- `wrappers.rs`

## Navigation

- Workspace root: `../..`
- This directory: `tokio-stream/src/`
