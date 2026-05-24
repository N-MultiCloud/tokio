# Tokio: tokio-stream/src/wrappers

## Purpose

Wrappers that expose Tokio resources such as channels, listeners, signals, and intervals as Streams.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `broadcast.rs`
- `interval.rs`
- `lines.rs`
- `mpsc_bounded.rs`
- `mpsc_unbounded.rs`
- `read_dir.rs`
- `signal_unix.rs`
- `signal_windows.rs`
- `split.rs`
- `tcp_listener.rs`
- `unix_listener.rs`
- `watch.rs`

## Navigation

- Workspace root: `../../..`
- This directory: `tokio-stream/src/wrappers/`
