# Tokio: tokio/src/runtime/scheduler/multi_thread

## Purpose

Work-stealing multi-thread scheduler. This is the default runtime flavor for most applications.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `handle/`
- `worker/`

## Key Files

- `counters.rs`
- `handle.rs`
- `idle.rs`
- `mod.rs`
- `overflow.rs`
- `park.rs`
- `queue.rs`
- `stats.rs`
- `trace.rs`
- `trace_mock.rs`
- `worker.rs`

## Navigation

- Workspace root: `../../../../..`
- This directory: `tokio/src/runtime/scheduler/multi_thread/`
