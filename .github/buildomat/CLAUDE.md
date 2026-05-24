# Tokio: .github/buildomat

## Purpose

Buildomat job definitions used by Tokio CI for selected platform and test jobs. Read this together with workflow YAML before changing CI coverage.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `README.md`
- `config.toml`

## Navigation

- Workspace root: `../..`
- This directory: `.github/buildomat/`
