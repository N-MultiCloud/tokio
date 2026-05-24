# Tokio: tokio/src/runtime

## Purpose

Runtime core: Builder, Runtime, Handle, scheduler selection, blocking pool, I/O and time drivers, task harness, metrics, and context management.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `blocking/`
- `context/`
- `driver/`
- `io/`
- `local_runtime/`
- `metrics/`
- `scheduler/`
- `signal/`
- `task/`
- `tests/`
- `time/`
- `time_alt/`

## Key Files

- `builder.rs`
- `config.rs`
- `context.rs`
- `driver.rs`
- `dump.rs`
- `handle.rs`
- `id.rs`
- `mod.rs`
- `park.rs`
- `process.rs`
- `runtime.rs`
- `task_hooks.rs`
- `thread_id.rs`

## Navigation

- Workspace root: `../../..`
- This directory: `tokio/src/runtime/`
