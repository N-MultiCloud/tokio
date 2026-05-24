# Tokio: tokio/src/sync/tests

## Purpose

Unit tests for synchronization primitives and channel behavior.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `atomic_waker.rs`
- `loom_atomic_waker.rs`
- `loom_broadcast.rs`
- `loom_list.rs`
- `loom_mpsc.rs`
- `loom_notify.rs`
- `loom_oneshot.rs`
- `loom_rwlock.rs`
- `loom_semaphore_batch.rs`
- `loom_set_once.rs`
- `loom_watch.rs`
- `mod.rs`
- `notify.rs`
- `semaphore_batch.rs`

## Navigation

- Workspace root: `../../../..`
- This directory: `tokio/src/sync/tests/`
