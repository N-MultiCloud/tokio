# Tokio: .github

## Purpose

GitHub automation and community metadata for the upstream Tokio project. It owns issue templates, workflow definitions, and Buildomat configuration used by CI and release validation.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `ISSUE_TEMPLATE/`
- `buildomat/`
- `workflows/`

## Key Files

- `FUNDING.yml`
- `PULL_REQUEST_TEMPLATE.md`
- `dependabot.yml`
- `labeler.yml`

## Navigation

- Workspace root: `..`
- This directory: `.github/`
