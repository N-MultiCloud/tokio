# Tokio: tests-integration

## Purpose

Workspace crate for cross-crate integration tests. Use it for behavior that needs multiple Tokio crates or full runtime setup.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `src/`
- `tests/`

## Key Files

- `Cargo.toml`
- `README.md`

## Navigation

- Workspace root: `..`
- This directory: `tests-integration/`
