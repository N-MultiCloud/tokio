# Tokio: tokio/src/net

## Purpose

Async networking types built around mio and Tokio readiness: TcpStream, TcpListener, UdpSocket, Unix sockets, address resolution, and platform shims.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `tcp/`
- `unix/`
- `windows/`

## Key Files

- `addr.rs`
- `lookup_host.rs`
- `mod.rs`
- `udp.rs`

## Navigation

- Workspace root: `../../..`
- This directory: `tokio/src/net/`
