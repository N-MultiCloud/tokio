# Tokio: tests-build/tests/fail

## Purpose

Fixtures expected to fail compilation. Each case documents an API misuse, missing feature gate, or diagnostic contract Tokio wants to preserve.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `macros_core_no_default.rs`
- `macros_core_no_default.stderr`
- `macros_dead_code.rs`
- `macros_dead_code.stderr`
- `macros_invalid_input.rs`
- `macros_invalid_input.stderr`
- `macros_join.rs`
- `macros_join.stderr`
- `macros_try_join.rs`
- `macros_try_join.stderr`
- `macros_type_mismatch.rs`
- `macros_type_mismatch.stderr`

## Navigation

- Workspace root: `../../..`
- This directory: `tests-build/tests/fail/`
