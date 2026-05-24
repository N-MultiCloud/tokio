# Tokio: tokio/src/net/unix

## Purpose

Unix-domain socket implementation for streams, listeners, datagrams, credentials, and pipe-like local IPC.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `datagram/`

## Key Files

- `listener.rs`
- `mod.rs`
- `pipe.rs`
- `socket.rs`
- `socketaddr.rs`
- `split.rs`
- `split_owned.rs`
- `stream.rs`
- `ucred.rs`

## Navigation

- Workspace root: `../../../..`
- This directory: `tokio/src/net/unix/`
