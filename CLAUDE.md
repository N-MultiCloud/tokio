# Tokio Workspace

## Purpose

Top-level Tokio workspace. This repository hosts the main tokio runtime crate plus companion crates for macros, streams, testing utilities, and protocol-oriented utilities. Start here to understand workspace membership, release policy, feature flags, CI, and how the crates fit together.

## Agent Notes

- Treat this checkout as the N-MultiCloud fork of upstream `tokio-rs/tokio`; keep behavior-preserving documentation changes separate from source changes unless a task explicitly asks for source edits.
- Prefer Rust-aware navigation (`rust-analyzer`, `cargo metadata`, and targeted tests) over broad text guessing when tracing runtime, scheduler, macro, or feature-gated behavior.
- Before changing code in this directory, inspect the nearest `Cargo.toml`, module-level rustdoc, and colocated tests so feature flags and cfg-specific behavior stay intact.

## Direct Subdirectories

- `.github/`
- `benches/`
- `docs/`
- `examples/`
- `stress-test/`
- `target-specs/`
- `tests-build/`
- `tests-integration/`
- `tokio/`
- `tokio-macros/`
- `tokio-stream/`
- `tokio-test/`
- `tokio-util/`

## Key Files

- `.gitignore`
- `CODE_OF_CONDUCT.md`
- `CONTRIBUTING.md`
- `Cargo.toml`
- `Cross.toml`
- `LICENSE`
- `README.md`
- `SECURITY.md`
- `deny.toml`
- `netlify.toml`
- `spellcheck.dic`
- `spellcheck.toml`

## Navigation

- Workspace root: `.`
- This directory: `.`

## Full Directory Index

- `.` - Top-level Tokio workspace. This repository hosts the main tokio runtime crate plus companion crates for macros, streams, testing utilities, and protocol-oriented utilities. Start here to understand workspace membership, release policy, feature flags, CI, and how the crates fit together.
- `.github/` - GitHub automation and community metadata for the upstream Tokio project. It owns issue templates, workflow definitions, and Buildomat configuration used by CI and release validation.
- `benches/` - Cargo workspace crate containing benchmarks for runtime, sync, I/O, scheduler, channel, and utility performance. Use it for performance-sensitive changes after functional tests are green.
- `docs/` - Directory for documentation under `root`. Use this local index to identify the direct subfolders and key files before editing or reviewing this part of Tokio.
- `examples/` - Runnable example crate showing typical Tokio usage patterns, including TCP/UDP, task spawning, streams, channels, cancellation, and runtime setup.
- `stress-test/` - Internal stress-test crate for exercising runtime and synchronization behavior under heavier load than unit tests. Use it when scheduler, timer, or channel behavior changes.
- `target-specs/` - Custom Rust target specification files and notes used for platform coverage. Check here before assuming a target's cfg or atomics support.
- `tests-build/` - Compile-fail and compile-pass test crate. This validates feature gating, macros, public API shape, and documentation examples at build time.
- `tests-integration/` - Workspace crate for cross-crate integration tests. Use it for behavior that needs multiple Tokio crates or full runtime setup.
- `tokio/` - Main tokio crate. This is the runtime, task scheduler, I/O driver, timers, async fs/process/signal/net APIs, synchronization primitives, and public module surface users depend on.
- `tokio-macros/` - Procedural macro crate for #[tokio::main] and #[tokio::test]. It parses macro arguments and expands them into runtime builder setup.
- `tokio-stream/` - Companion crate for Stream adapters and wrappers around Tokio primitives. It bridges Tokio channels, listeners, signals, and interval types into futures_core::Stream.
- `tokio-test/` - Testing utilities for Tokio-based code, including mock I/O, task assertion helpers, and deterministic runtime support for examples and downstream crates.
- `tokio-util/` - Utilities layered above Tokio: codecs, framed transports, cancellation tokens, sync helpers, UDP framing, IO adapters, task utilities, and timer utilities.
- `.github/ISSUE_TEMPLATE/` - GitHub issue forms for bug reports and feature requests. These files shape contributor intake before maintainers triage runtime, I/O, docs, or ecosystem issues.
- `.github/buildomat/` - Buildomat job definitions used by Tokio CI for selected platform and test jobs. Read this together with workflow YAML before changing CI coverage.
- `.github/workflows/` - GitHub Actions workflows for Tokio CI, docs, loom, miri, fuzz, and release-adjacent validation. These are the source of truth for automated checks on the fork.
- `docs/contributing/` - Contributor guide source. It explains Tokio project process, tests, unstable features, commit expectations, and how to run specialized checks.
- `stress-test/examples/` - Standalone stress-test scenarios. These are entry points for manual or scripted stress runs.
- `tests-build/src/` - Small support library for tests-build. Keep helpers here minimal so compile tests exercise Tokio's public API rather than local abstractions.
- `tests-build/tests/` - Top-level integration tests for build-time behavior. The pass and fail subdirectories hold trybuild-style fixtures.
- `tests-integration/src/` - Support library and shared helpers for integration tests.
- `tests-integration/tests/` - Integration test cases run as a standalone crate against the workspace crates.
- `tokio-macros/src/` - Implementation of Tokio procedural macros, including entry-point parsing, runtime flavor selection, and generated async test/main wrappers.
- `tokio-stream/fuzz/` - Fuzz harness configuration for tokio-stream.
- `tokio-stream/src/` - Source root for stream wrappers and StreamExt utilities.
- `tokio-stream/tests/` - tokio-stream integration tests.
- `tokio-test/src/` - Source for tokio-test helpers such as io mocks, task spawning helpers, and stream mocks.
- `tokio-test/tests/` - Integration tests for tokio-test itself.
- `tokio-util/src/` - Source root for tokio-util feature modules.
- `tokio-util/tests/` - tokio-util integration tests for codecs, sync, io, net, task, and time helpers.
- `tokio/docs/` - Additional crate-level documentation sources for Tokio. Keep these aligned with rustdoc and the tokio.rs guides.
- `tokio/fuzz/` - Fuzzing harness configuration for the main tokio crate. Use it for parser, codec, I/O, or scheduler edge cases where randomized exploration is valuable.
- `tokio/src/` - Source root for the main tokio crate. Public modules are feature-gated from lib.rs and fan out to runtime, task, io, net, sync, time, process, fs, and signal implementations.
- `tokio/tests/` - Main tokio crate integration tests. These cover public behavior across runtime, net, io, sync, time, process, fs, and feature combinations.
- `tests-build/tests/fail/` - Fixtures expected to fail compilation. Each case documents an API misuse, missing feature gate, or diagnostic contract Tokio wants to preserve.
- `tests-build/tests/pass/` - Fixtures expected to compile. These guard feature combinations, macros, and public examples that must continue to build.
- `tests-integration/src/bin/` - Small binaries used by integration tests, often for process, signal, or subprocess behavior.
- `tokio-stream/fuzz/fuzz_targets/` - Concrete fuzz targets for tokio-stream adapters.
- `tokio-stream/src/stream_ext/` - Extension traits and combinators for streams.
- `tokio-stream/src/wrappers/` - Wrappers that expose Tokio resources such as channels, listeners, signals, and intervals as Streams.
- `tokio-stream/tests/support/` - Shared helpers for tokio-stream tests.
- `tokio-util/src/codec/` - Framing and encoding/decoding utilities, including Framed, Encoder, Decoder, lines, bytes, and length-delimited codecs.
- `tokio-util/src/future/` - Future helpers for tokio-util.
- `tokio-util/src/io/` - I/O adapters such as ReaderStream, StreamReader, SyncIoBridge, and inspection/copy helpers.
- `tokio-util/src/net/` - Network utility layer above tokio::net.
- `tokio-util/src/sync/` - Synchronization utilities such as CancellationToken, PollSender, reusable boxes, and mpsc helpers.
- `tokio-util/src/task/` - Task utilities layered above Tokio, such as task trackers and abort-on-drop helpers.
- `tokio-util/src/time/` - Time utilities such as DelayQueue.
- `tokio-util/src/udp/` - UDP framing utilities such as UdpFramed.
- `tokio-util/src/util/` - Internal helpers for tokio-util modules.
- `tokio/fuzz/fuzz_targets/` - Concrete fuzz targets for the main tokio crate.
- `tokio/src/doc/` - Rustdoc-only guide modules and supporting examples. These files shape docs.rs output and user-facing narrative.
- `tokio/src/fs/` - Asynchronous filesystem facade. Tokio implements most fs operations by moving blocking std::fs work onto the blocking pool while preserving async APIs.
- `tokio/src/future/` - Small future utilities exposed by Tokio. These helpers support polling and pending behavior without pulling in larger dependencies.
- `tokio/src/io/` - Async I/O traits, readiness abstractions, PollEvented integration, platform-specific readiness, and io-util extension traits gated behind features.
- `tokio/src/loom/` - Abstraction layer over std and loom primitives. This lets concurrency code run under deterministic loom exploration without changing production code.
- `tokio/src/macros/` - Declarative macros and feature-gated macro support used by the main crate. Procedural macros live in tokio-macros.
- `tokio/src/net/` - Async networking types built around mio and Tokio readiness: TcpStream, TcpListener, UdpSocket, Unix sockets, address resolution, and platform shims.
- `tokio/src/process/` - Async process management. Wraps std::process with nonblocking wait, async pipes, kill-on-drop behavior, and platform-specific child handling.
- `tokio/src/runtime/` - Runtime core: Builder, Runtime, Handle, scheduler selection, blocking pool, I/O and time drivers, task harness, metrics, and context management.
- `tokio/src/signal/` - Public async signal handling APIs. Bridges OS signal mechanisms into futures and streams through the runtime signal driver.
- `tokio/src/sync/` - Async synchronization primitives: Mutex, RwLock, Semaphore, Notify, Barrier, broadcast/watch/mpsc/oneshot channels, and task coordination helpers.
- `tokio/src/task/` - Public task API: spawn, spawn_blocking, yield_now, JoinHandle, JoinSet, LocalSet, task locals, cancellation, and cooperative scheduling surface.
- `tokio/src/time/` - Public time API: sleep, timeout, interval, Instant wrappers, pause/advance test utilities, and clock behavior.
- `tokio/src/util/` - Internal utilities shared by Tokio modules. APIs here are not public contracts unless re-exported elsewhere.
- `tokio/tests/support/` - Shared support helpers for tokio integration tests.
- `tokio-util/src/net/unix/` - Unix-specific network utilities for tokio-util.
- `tokio-util/src/sync/cancellation_token/` - CancellationToken implementation details, waiters, tree nodes, and cancellation propagation.
- `tokio-util/src/sync/tests/` - Tests colocated with tokio-util sync internals.
- `tokio-util/src/time/wheel/` - Timer wheel implementation used by tokio-util DelayQueue.
- `tokio/src/fs/file/` - Implementation details for tokio::fs::File, including async read/write state, blocking-pool handoff, and flush/shutdown behavior.
- `tokio/src/fs/open_options/` - Builder implementation for asynchronous file open options. Mirrors std::fs::OpenOptions while routing open work through Tokio.
- `tokio/src/io/bsd/` - BSD-specific asynchronous I/O support. Check target cfgs here before changing kqueue or FreeBSD behavior.
- `tokio/src/io/uring/` - Unstable Linux io_uring integration. Requires tokio_unstable and Linux-specific feature gates.
- `tokio/src/io/util/` - AsyncReadExt/AsyncWriteExt combinators and utility futures such as read_exact, write_all, copy, split, and buffering helpers.
- `tokio/src/loom/std/` - Loom-compatible stand-ins for standard synchronization, atomics, and threading primitives.
- `tokio/src/net/tcp/` - TCP stream/listener/socket implementation, splitting types, readiness polling, and conversion to/from std sockets.
- `tokio/src/net/unix/` - Unix-domain socket implementation for streams, listeners, datagrams, credentials, and pipe-like local IPC.
- `tokio/src/net/windows/` - Windows networking and named-pipe support modules.
- `tokio/src/process/unix/` - Unix-specific child process, signal, and pipe handling.
- `tokio/src/runtime/blocking/` - Blocking pool implementation for spawn_blocking and async APIs that must delegate blocking OS calls. Tune carefully because this protects core async worker threads.
- `tokio/src/runtime/context/` - Thread-local runtime context. This is how tokio::spawn, Handle::current, drivers, and task-local state find the active runtime.
- `tokio/src/runtime/driver/` - Composite driver wiring for I/O, time, signal, and optional features. Runtime builders enable or disable these drivers here.
- `tokio/src/runtime/io/` - Runtime-owned I/O driver surface and registration types. It connects PollEvented resources to the scheduler through readiness notifications.
- `tokio/src/runtime/local_runtime/` - Local runtime support for !Send futures. This complements current-thread and multi-thread runtimes with local scheduling constraints.
- `tokio/src/runtime/metrics/` - Runtime and scheduler metrics exposed behind stable and unstable APIs. Keep field semantics compatible because users scrape these values.
- `tokio/src/runtime/scheduler/` - Task schedulers. This directory owns current-thread, multi-thread, inject queues, run queues, worker logic, and scheduling utilities.
- `tokio/src/runtime/signal/` - Runtime signal driver internals. Public signal APIs live under tokio/src/signal.
- `tokio/src/runtime/task/` - Task harness internals: raw task allocation, state transitions, wakers, join handles, cancellation, scheduling, and tracing hooks.
- `tokio/src/runtime/tests/` - Runtime unit tests and support modules colocated with runtime internals.
- `tokio/src/runtime/time/` - Primary timer driver, sleep/interval/timeout plumbing, timer entries, and wheel integration.
- `tokio/src/runtime/time_alt/` - Alternative timer implementation under active experimentation or unstable cfgs.
- `tokio/src/signal/windows/` - Windows-specific signal and console-control handling.
- `tokio/src/sync/mpsc/` - Multi-producer single-consumer channel implementation, including bounded/unbounded variants, permits, blocks, and backpressure logic.
- `tokio/src/sync/rwlock/` - Asynchronous RwLock implementation and guards.
- `tokio/src/sync/task/` - Low-level task notification helpers used by synchronization primitives.
- `tokio/src/sync/tests/` - Unit tests for synchronization primitives and channel behavior.
- `tokio/src/task/coop/` - Cooperative scheduling budget implementation. This prevents long-running futures from starving the runtime.
- `tokio/src/util/rand/` - Small random utilities used by scheduling and runtime internals.
- `tokio/src/net/unix/datagram/` - Unix datagram socket implementation and split halves.
- `tokio/src/runtime/io/driver/` - Low-level I/O driver implementation backed by mio's Poll and event registry.
- `tokio/src/runtime/metrics/histogram/` - Histogram types for runtime poll-count metrics and latency-style observations.
- `tokio/src/runtime/scheduler/current_thread/` - Single-threaded scheduler. It runs tasks only while block_on or LocalSet drives the runtime.
- `tokio/src/runtime/scheduler/inject/` - Global injection queue used to hand tasks into a scheduler from external threads or remote handles.
- `tokio/src/runtime/scheduler/multi_thread/` - Work-stealing multi-thread scheduler. This is the default runtime flavor for most applications.
- `tokio/src/runtime/scheduler/util/` - Shared scheduler utilities used by both scheduler flavors.
- `tokio/src/runtime/task/trace/` - Unstable task tracing and taskdump support used for runtime diagnostics.
- `tokio/src/runtime/tests/loom_current_thread/` - Loom tests for the current-thread scheduler and runtime internals.
- `tokio/src/runtime/tests/loom_multi_thread/` - Loom tests for the multi-thread scheduler and cross-thread task behavior.
- `tokio/src/runtime/time/tests/` - Timer-driver tests for scheduling, cancellation, pause/advance, and edge cases.
- `tokio/src/runtime/time/wheel/` - Hierarchical timer wheel implementation used by the primary time driver.
- `tokio/src/runtime/time_alt/cancellation_queue/` - Cancellation queue for the alternative timer implementation.
- `tokio/src/runtime/time_alt/registration_queue/` - Registration queue for the alternative timer implementation.
- `tokio/src/runtime/time_alt/wake_queue/` - Wake queue for the alternative timer implementation.
- `tokio/src/runtime/time_alt/wheel/` - Timer wheel pieces for the alternative timer implementation.
- `tokio/src/runtime/scheduler/multi_thread/handle/` - Handle-side logic for the multi-thread scheduler, including remote spawning and worker coordination hooks.
- `tokio/src/runtime/scheduler/multi_thread/worker/` - Worker thread loop, local queues, stealing, parking, unparking, and task polling for the multi-thread scheduler.

## Primary Crates

- `tokio/` - main runtime, I/O, timer, sync, task, net, fs, process, and signal crate.
- `tokio-macros/` - procedural macros for `#[tokio::main]` and `#[tokio::test]`.
- `tokio-util/` - codecs, cancellation, IO adapters, UDP framing, and task utilities.
- `tokio-stream/` - Stream wrappers and extension helpers for Tokio resources.
- `tokio-test/` - mock I/O and runtime-aware testing helpers.
