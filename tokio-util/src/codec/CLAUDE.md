# Tokio: tokio-util/src/codec

## Purpose

Framing and encoding/decoding utilities, including Framed, Encoder, Decoder, lines, bytes, and length-delimited codecs.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- None.

## Key Files

- `any_delimiter_codec.rs`
- `bytes_codec.rs`
- `decoder.rs`
- `encoder.rs`
- `framed.rs`
- `framed_impl.rs`
- `framed_read.rs`
- `framed_write.rs`
- `length_delimited.rs`
- `lines_codec.rs`
- `mod.rs`

## Navigation

- Workspace root: `../../..`
- This directory: `tokio-util/src/codec/`
