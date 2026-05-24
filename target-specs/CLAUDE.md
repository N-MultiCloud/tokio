# Tokio: target-specs

## Purpose

Custom Rust target specification files and notes used for platform coverage. Check here before assuming a target's cfg or atomics support.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `README.md`
- `i686-unknown-linux-gnu.json`

## Navigation

- Workspace root: `..`
- This directory: `target-specs/`
