# Tokio: tokio/src/sync

## Purpose

Async synchronization primitives: Mutex, RwLock, Semaphore, Notify, Barrier, broadcast/watch/mpsc/oneshot channels, and task coordination helpers.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `mpsc/`
- `rwlock/`
- `task/`
- `tests/`

## Key Files

- `barrier.rs`
- `batch_semaphore.rs`
- `broadcast.rs`
- `mod.rs`
- `mutex.rs`
- `notify.rs`
- `once_cell.rs`
- `oneshot.rs`
- `rwlock.rs`
- `semaphore.rs`
- `set_once.rs`
- `watch.rs`

## Navigation

- Workspace root: `../../..`
- This directory: `tokio/src/sync/`
