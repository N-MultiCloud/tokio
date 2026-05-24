# Tokio: tokio/src/runtime/time

## Purpose

Primary timer driver, sleep/interval/timeout plumbing, timer entries, and wheel integration.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `tests/`
- `wheel/`

## Key Files

- `entry.rs`
- `handle.rs`
- `mod.rs`
- `source.rs`

## Navigation

- Workspace root: `../../../..`
- This directory: `tokio/src/runtime/time/`
