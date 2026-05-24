# Tokio: tokio/tests

## Purpose

Main tokio crate integration tests. These cover public behavior across runtime, net, io, sync, time, process, fs, and feature combinations.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `support/`

## Key Files

- `_require_full.rs`
- `async_send_sync.rs`
- `buffered.rs`
- `coop_budget.rs`
- `dump.rs`
- `duplex_stream.rs`
- `fs.rs`
- `fs_canonicalize_dir.rs`
- `fs_copy.rs`
- `fs_dir.rs`
- `fs_file.rs`
- `fs_link.rs`
- `fs_open_options.rs`
- `fs_open_options_windows.rs`
- `fs_remove_dir_all.rs`
- `fs_remove_file.rs`
- `fs_rename.rs`
- `fs_symlink_dir_windows.rs`
- `... plus 151 more tracked files`

## Navigation

- Workspace root: `../..`
- This directory: `tokio/tests/`
