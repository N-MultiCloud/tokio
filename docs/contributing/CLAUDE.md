# Tokio: docs/contributing

## Purpose

Contributor guide source. It explains Tokio project process, tests, unstable features, commit expectations, and how to run specialized checks.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `README.md`
- `contributing-in-issues.md`
- `how-to-specify-crates-dependencies-versions.md`
- `keeping-track-of-issues-and-prs.md`
- `pull-requests.md`
- `reviewing-pull-requests.md`

## Navigation

- Workspace root: `../..`
- This directory: `docs/contributing/`
