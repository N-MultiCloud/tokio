# Tokio: .github/workflows

## Purpose

GitHub Actions workflows for Tokio CI, docs, loom, miri, fuzz, and release-adjacent validation. These are the source of truth for automated checks on the fork.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `audit.yml`
- `ci.yml`
- `labeler.yml`
- `loom.yml`
- `pr-audit.yml`
- `stress-test.yml`
- `uring-kernel-version-test.yml`

## Navigation

- Workspace root: `../..`
- This directory: `.github/workflows/`
