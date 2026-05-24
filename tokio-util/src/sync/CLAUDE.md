# Tokio: tokio-util/src/sync

## Purpose

Synchronization utilities such as CancellationToken, PollSender, reusable boxes, and mpsc helpers.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `cancellation_token/`
- `tests/`

## Key Files

- `cancellation_token.rs`
- `mod.rs`
- `mpsc.rs`
- `poll_semaphore.rs`
- `reusable_box.rs`

## Navigation

- Workspace root: `../../..`
- This directory: `tokio-util/src/sync/`
