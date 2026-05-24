# Tokio: tokio/src/runtime/scheduler

## Purpose

Task schedulers. This directory owns current-thread, multi-thread, inject queues, run queues, worker logic, and scheduling utilities.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `current_thread/`
- `inject/`
- `multi_thread/`
- `util/`

## Key Files

- `block_in_place.rs`
- `defer.rs`
- `inject.rs`
- `lock.rs`
- `mod.rs`

## Navigation

- Workspace root: `../../../..`
- This directory: `tokio/src/runtime/scheduler/`
