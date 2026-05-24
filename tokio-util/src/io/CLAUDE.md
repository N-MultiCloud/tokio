# Tokio: tokio-util/src/io

## Purpose

I/O adapters such as ReaderStream, StreamReader, SyncIoBridge, and inspection/copy helpers.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `copy_to_bytes.rs`
- `inspect.rs`
- `mod.rs`
- `read_arc.rs`
- `read_buf.rs`
- `reader_stream.rs`
- `simplex.rs`
- `sink_writer.rs`
- `stream_reader.rs`
- `sync_bridge.rs`
- `write_all_vectored.rs`

## Navigation

- Workspace root: `../../..`
- This directory: `tokio-util/src/io/`
