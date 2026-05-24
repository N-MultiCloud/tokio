# Tokio: tokio/src/macros

## Purpose

Declarative macros and feature-gated macro support used by the main crate. Procedural macros live in tokio-macros.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `addr_of.rs`
- `cfg.rs`
- `join.rs`
- `loom.rs`
- `mod.rs`
- `pin.rs`
- `select.rs`
- `support.rs`
- `thread_local.rs`
- `trace.rs`
- `try_join.rs`

## Navigation

- Workspace root: `../../..`
- This directory: `tokio/src/macros/`
