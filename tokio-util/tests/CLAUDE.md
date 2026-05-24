# Tokio: tokio-util/tests

## Purpose

tokio-util integration tests for codecs, sync, io, net, task, and time helpers.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `_require_full.rs`
- `abort_on_drop.rs`
- `codecs.rs`
- `compat.rs`
- `context.rs`
- `framed.rs`
- `framed_read.rs`
- `framed_stream.rs`
- `framed_write.rs`
- `future.rs`
- `io_inspect.rs`
- `io_reader_stream.rs`
- `io_simplex.rs`
- `io_sink_writer.rs`
- `io_stream_reader.rs`
- `io_sync_bridge.rs`
- `io_write_all_vectored.rs`
- `length_delimited.rs`
- `... plus 11 more tracked files`

## Navigation

- Workspace root: `../..`
- This directory: `tokio-util/tests/`
