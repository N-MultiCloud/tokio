# Tokio: tokio-stream/tests

## Purpose

tokio-stream integration tests.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `support/`

## Key Files

- `async_send_sync.rs`
- `chunks_timeout.rs`
- `mpsc_bounded_stream.rs`
- `mpsc_unbounded_stream.rs`
- `stream_chain.rs`
- `stream_chunks_timeout.rs`
- `stream_close.rs`
- `stream_collect.rs`
- `stream_empty.rs`
- `stream_fuse.rs`
- `stream_fused.rs`
- `stream_iter.rs`
- `stream_merge.rs`
- `stream_once.rs`
- `stream_panic.rs`
- `stream_pending.rs`
- `stream_stream_map.rs`
- `stream_timeout.rs`
- `... plus 2 more tracked files`

## Navigation

- Workspace root: `../..`
- This directory: `tokio-stream/tests/`
