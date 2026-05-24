# Tokio: tokio/src/io

## Purpose

Async I/O traits, readiness abstractions, PollEvented integration, platform-specific readiness, and io-util extension traits gated behind features.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `bsd/`
- `uring/`
- `util/`

## Key Files

- `async_buf_read.rs`
- `async_fd.rs`
- `async_read.rs`
- `async_seek.rs`
- `async_write.rs`
- `blocking.rs`
- `interest.rs`
- `join.rs`
- `mod.rs`
- `poll_evented.rs`
- `read_buf.rs`
- `ready.rs`
- `seek.rs`
- `split.rs`
- `stderr.rs`
- `stdin.rs`
- `stdio_common.rs`
- `stdout.rs`

## Navigation

- Workspace root: `../../..`
- This directory: `tokio/src/io/`
