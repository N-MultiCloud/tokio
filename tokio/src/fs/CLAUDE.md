# Tokio: tokio/src/fs

## Purpose

Asynchronous filesystem facade. Tokio implements most fs operations by moving blocking std::fs work onto the blocking pool while preserving async APIs.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `file/`
- `open_options/`

## Key Files

- `canonicalize.rs`
- `copy.rs`
- `create_dir.rs`
- `create_dir_all.rs`
- `dir_builder.rs`
- `file.rs`
- `hard_link.rs`
- `metadata.rs`
- `mocks.rs`
- `mod.rs`
- `open_options.rs`
- `read.rs`
- `read_dir.rs`
- `read_link.rs`
- `read_to_string.rs`
- `read_uring.rs`
- `remove_dir.rs`
- `remove_dir_all.rs`
- `... plus 9 more tracked files`

## Navigation

- Workspace root: `../../..`
- This directory: `tokio/src/fs/`
