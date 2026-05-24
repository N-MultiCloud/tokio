# Tokio: tokio/src/runtime/tests

## Purpose

Runtime unit tests and support modules colocated with runtime internals.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `loom_current_thread/`
- `loom_multi_thread/`

## Key Files

- `inject.rs`
- `loom_blocking.rs`
- `loom_current_thread.rs`
- `loom_join_set.rs`
- `loom_local.rs`
- `loom_multi_thread.rs`
- `loom_oneshot.rs`
- `mod.rs`
- `queue.rs`
- `task.rs`
- `task_combinations.rs`

## Navigation

- Workspace root: `../../../..`
- This directory: `tokio/src/runtime/tests/`
