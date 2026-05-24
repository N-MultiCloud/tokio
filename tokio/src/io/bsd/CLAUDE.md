# Tokio: tokio/src/io/bsd

## Purpose

BSD-specific asynchronous I/O support. Check target cfgs here before changing kqueue or FreeBSD behavior.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `poll_aio.rs`

## Navigation

- Workspace root: `../../../..`
- This directory: `tokio/src/io/bsd/`
