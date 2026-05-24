# Tokio: tokio/src/task

## Purpose

Public task API: spawn, spawn_blocking, yield_now, JoinHandle, JoinSet, LocalSet, task locals, cancellation, and cooperative scheduling surface.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `coop/`

## Key Files

- `blocking.rs`
- `builder.rs`
- `join_set.rs`
- `local.rs`
- `mod.rs`
- `spawn.rs`
- `task_local.rs`
- `yield_now.rs`

## Navigation

- Workspace root: `../../..`
- This directory: `tokio/src/task/`
