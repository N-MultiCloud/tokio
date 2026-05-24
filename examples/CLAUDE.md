# Tokio: examples

## Purpose

Runnable example crate showing typical Tokio usage patterns, including TCP/UDP, task spawning, streams, channels, cancellation, and runtime setup.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `Cargo.toml`
- `README.md`
- `chat.rs`
- `connect-tcp.rs`
- `connect-udp.rs`
- `custom-executor-tokio-context.rs`
- `custom-executor.rs`
- `dump.rs`
- `echo-tcp.rs`
- `echo-udp.rs`
- `graceful-shutdown.rs`
- `hello_world.rs`
- `named-pipe-multi-client.rs`
- `named-pipe-ready.rs`
- `named-pipe.rs`
- `prewarm-fd-table.rs`
- `print_each_packet.rs`
- `proxy.rs`
- `... plus 4 more tracked files`

## Navigation

- Workspace root: `..`
- This directory: `examples/`
