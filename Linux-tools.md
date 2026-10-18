# xSAR Linux Tools

[← Back to the xSAR repository map](README.md)

Linux-specific utilities and supporting frameworks for systems work, service
integration, storage and inter-process communication.

## Message Queue Framework

**Status:** Planned

A reusable Linux message-queue framework for communication between services,
sensor-acquisition processes, analysis tools and supporting applications.

The design direction is expected to cover:

- clear message schemas and versioning;
- bounded queues and back-pressure behaviour;
- process and service integration;
- failure recovery and observable queue state;
- Rust interfaces suitable for Linux applications and services.

## Warm Drive Cache

**Status:** Active  
**Latest version:** 0.2.0

Rust VFS cache warmer for rclone FUSE mounts. It walks the mounted sync
directories to pre-populate listings, metadata and size-gated file contents,
BLAKE3-verifies warmed content against the local VFS cache by default, and only
ever deletes from the separate rclone cache directory, never the live mount.

- [Open the Warm Drive Cache repository](https://github.com/xSAR-research/warm-drive-cache)

## QMP QEMU Socket

**Status:** Experimental

Rust desktop agent for calibrated vision, allow-listed QMP↔QEMU control, and an
egui UI. It connects to an existing QEMU QMP Unix socket and does not launch
QEMU or create that socket. Solitaire guest modes are disposable fixtures, not
the product. The target is Dijkstra / A* shortest-path solving rather than the
guest Solver, as practice for drone route planning. Beast acceptance is required
before promotion.

**Latest version:** 2.2.100 (numeric `major.minor.build` migration checkpoint;
Beast verification pending)

Recent highlights from the changelog:

- screen capture over TCP from QEMU Screen Grab Server, using version-3
  full-screen BGR8 frames on a persistent session, with the original QMP
  acquisition kept for comparison and reconnection after an idle disconnect;
- Pyramid reconnaissance exported to JSON (schema 2, explicit card values)
  through the shared `xsar::pyramid_json` codec;
- bounded, input-safe Level Up / OK confirmation across all five game types,
  with byte-original captures retained as regression evidence.

Related prior work: private [solitaire-solver](https://github.com/xSAR-research/solitaire-solver)
(TriPeaks-era predecessor; not archived).

- [Open the QMP QEMU Socket repository](https://github.com/xSAR-research/qmp-qemu-socket)

## QEMU Screen Grab Server

**Status:** Experimental

Companion to QMP QEMU Socket. A Rust TCP server that runs manually inside the
Windows guest, captures the interactive desktop with GDI and returns fresh
1920 × 1080 BGR8 frames on port 9999, as a faster alternative to grabbing the
screen through QMP.

**Latest version:** 0.1.3 (unreleased)

Recent highlights from the changelog:

- automatic per-run logging in the launch directory, mirrored to the console;
- full-screen version-3 BGR8 responses and repeated fresh requests on one
  connection (0.1.2, paired with xsar 0.4.x), keeping legacy version-2 requests
  for explicit comparison;
- bounded admission, queues and network deadlines, with per-stage timings and
  clean Ctrl+C shutdown once clients and the capture thread have finished.

- [Open the QEMU Screen Grab Server repository](https://github.com/xSAR-research/qemu-screen-grab-server)

## File Finder

**Status:** Experimental  
**Latest version:** 0.1.0

Linux-first Rust + egui desktop app for indexing, searching and safely triaging
files from one configured source. It uses an incremental SQLite (WAL) index,
plain-text and wildcard search, planned moves into destination buckets with
confirmation, a Trash Review bucket instead of permanent deletion, and
approximate duplicate detection with BLAKE3 samples or metadata. Targets KDE
Plasma on Wayland.

- [Open the File Finder repository](https://github.com/xSAR-research/file-finder)

## Summit File Management

**Status:** Experimental  
**Latest version:** 0.1.0

Priority-aware file search and management in Rust: a multi-share indexer with
incremental SMB scans, pluggable Meilisearch, Elasticsearch or embedded Tantivy
search, an egui desktop client and a REST/WebSocket server with a live web
console. The codebase is teaching-oriented, with module notes explaining why
each design choice was made. File Finder is the simpler single-process sibling.

- [Open the Summit File Management repository](https://github.com/xSAR-research/file-management)

---

[← Back to the xSAR repository map](README.md)
