# Tokio: tokio/src/util

## Purpose

Internal utilities shared by Tokio modules. APIs here are not public contracts unless re-exported elsewhere.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `rand/`

## Key Files

- `as_ref.rs`
- `atomic_cell.rs`
- `bit.rs`
- `blocking_check.rs`
- `cacheline.rs`
- `error.rs`
- `idle_notified_set.rs`
- `linked_list.rs`
- `markers.rs`
- `memchr.rs`
- `metric_atomics.rs`
- `mod.rs`
- `ptr_expose.rs`
- `rand.rs`
- `rc_cell.rs`
- `sharded_list.rs`
- `sync_wrapper.rs`
- `trace.rs`
- `... plus 4 more tracked files`

## Navigation

- Workspace root: `../../..`
- This directory: `tokio/src/util/`
