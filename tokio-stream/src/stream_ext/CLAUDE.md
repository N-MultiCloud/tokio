# Tokio: tokio-stream/src/stream_ext

## Purpose

Extension traits and combinators for streams.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `all.rs`
- `any.rs`
- `chain.rs`
- `chunks_timeout.rs`
- `collect.rs`
- `filter.rs`
- `filter_map.rs`
- `fold.rs`
- `fuse.rs`
- `map.rs`
- `map_while.rs`
- `merge.rs`
- `next.rs`
- `peekable.rs`
- `skip.rs`
- `skip_while.rs`
- `take.rs`
- `take_while.rs`
- `... plus 5 more tracked files`

## Navigation

- Workspace root: `../../..`
- This directory: `tokio-stream/src/stream_ext/`
