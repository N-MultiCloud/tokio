# Tokio: benches

## Purpose

Cargo workspace crate containing benchmarks for runtime, sync, I/O, scheduler, channel, and utility performance. Use it for performance-sensitive changes after functional tests are green.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `Cargo.toml`
- `copy.rs`
- `fs.rs`
- `remote_spawn.rs`
- `rt_current_thread.rs`
- `rt_multi_threaded.rs`
- `signal.rs`
- `spawn.rs`
- `spawn_blocking.rs`
- `sync_broadcast.rs`
- `sync_mpsc.rs`
- `sync_mpsc_oneshot.rs`
- `sync_notify.rs`
- `sync_rwlock.rs`
- `sync_semaphore.rs`
- `sync_watch.rs`
- `time_now.rs`
- `time_timeout.rs`

## Navigation

- Workspace root: `..`
- This directory: `benches/`
