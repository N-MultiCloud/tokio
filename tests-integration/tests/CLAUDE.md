# Tokio: tests-integration/tests

## Purpose

Integration test cases run as a standalone crate against the workspace crates.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `macros_main.rs`
- `macros_pin.rs`
- `macros_select.rs`
- `process_stdio.rs`
- `rt_yield.rs`

## Navigation

- Workspace root: `../..`
- This directory: `tests-integration/tests/`
