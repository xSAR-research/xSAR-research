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

Linux storage tooling for controlled cache warming and data placement.

- [Open the Warm Drive Cache repository](https://github.com/xSAR-research/warm-drive-cache)

## QMP QEMU Socket

**Status:** Experimental

Rust desktop agent for calibrated vision, allow-listed QMP↔QEMU control, and an
egui UI. It connects to an existing QEMU QMP Unix socket and does not launch
QEMU or create that socket. Solitaire guest modes are disposable fixtures, not
the product. The target is Dijkstra / A* shortest-path solving rather than the
guest Solver, as practice for drone route planning. Beast acceptance is required
before promotion.

Related prior work: private [solitaire-solver](https://github.com/xSAR-research/solitaire-solver)
(TriPeaks-era predecessor; not archived).

- [Open the QMP QEMU Socket repository](https://github.com/xSAR-research/qmp-qemu-socket)

## QEMU Screen Grab Server

**Status:** Experimental

Companion to QMP QEMU Socket. A Rust TCP server that runs manually inside the
Windows guest, captures the interactive desktop with GDI and returns fresh
1920 × 1080 BGR8 frames on port 9999, as a faster alternative to grabbing the
screen through QMP.

- [Open the QEMU Screen Grab Server repository](https://github.com/xSAR-research/qemu-screen-grab-server)

---

[← Back to the xSAR repository map](README.md)
