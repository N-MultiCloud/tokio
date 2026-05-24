# Tokio: tokio/src/net/tcp

## Purpose

TCP stream/listener/socket implementation, splitting types, readiness polling, and conversion to/from std sockets.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `listener.rs`
- `mod.rs`
- `socket.rs`
- `split.rs`
- `split_owned.rs`
- `stream.rs`

## Navigation

- Workspace root: `../../../..`
- This directory: `tokio/src/net/tcp/`
