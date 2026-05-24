# Tokio: tokio/src/runtime/io

## Purpose

Runtime-owned I/O driver surface and registration types. It connects PollEvented resources to the scheduler through readiness notifications.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `driver/`

## Key Files

- `driver.rs`
- `metrics.rs`
- `mod.rs`
- `registration.rs`
- `registration_set.rs`
- `scheduled_io.rs`

## Navigation

- Workspace root: `../../../..`
- This directory: `tokio/src/runtime/io/`
