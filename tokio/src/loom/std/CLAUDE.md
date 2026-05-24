# Tokio: tokio/src/loom/std

## Purpose

Loom-compatible stand-ins for standard synchronization, atomics, and threading primitives.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `atomic_u16.rs`
- `atomic_u32.rs`
- `atomic_u64.rs`
- `atomic_u64_as_mutex.rs`
- `atomic_u64_native.rs`
- `atomic_u64_static_const_new.rs`
- `atomic_u64_static_once_cell.rs`
- `atomic_usize.rs`
- `barrier.rs`
- `mod.rs`
- `mutex.rs`
- `parking_lot.rs`
- `rwlock.rs`
- `unsafe_cell.rs`

## Navigation

- Workspace root: `../../../..`
- This directory: `tokio/src/loom/std/`
