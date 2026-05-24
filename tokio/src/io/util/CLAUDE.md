# Tokio: tokio/src/io/util

## Purpose

AsyncReadExt/AsyncWriteExt combinators and utility futures such as read_exact, write_all, copy, split, and buffering helpers.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `async_buf_read_ext.rs`
- `async_read_ext.rs`
- `async_seek_ext.rs`
- `async_write_ext.rs`
- `buf_reader.rs`
- `buf_stream.rs`
- `buf_writer.rs`
- `chain.rs`
- `copy.rs`
- `copy_bidirectional.rs`
- `copy_buf.rs`
- `empty.rs`
- `fill_buf.rs`
- `flush.rs`
- `lines.rs`
- `mem.rs`
- `mod.rs`
- `read.rs`
- `... plus 19 more tracked files`

## Navigation

- Workspace root: `../../../..`
- This directory: `tokio/src/io/util/`
