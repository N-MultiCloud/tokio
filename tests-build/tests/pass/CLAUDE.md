# Tokio: tests-build/tests/pass

## Purpose

Fixtures expected to compile. These guard feature combinations, macros, and public examples that must continue to build.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `forward_args_and_output.rs`
- `impl_trait.rs`
- `macros_main_loop.rs`
- `macros_main_return.rs`
- `use_builder_outer.rs`

## Navigation

- Workspace root: `../../..`
- This directory: `tests-build/tests/pass/`
