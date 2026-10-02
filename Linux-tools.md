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
**Implementation:** Rust (egui)  
**Platform:** Arch Linux on beast (QEMU host); Windows 11 guest fixtures

Rust desktop agent: calibrated vision detectors and effect proofs, allow-listed
QMP↔QEMU control over a Unix socket, and an egui UI. Solitaire guest modes
(TriPeaks, Pyramid, Klondike) are disposable fixtures for the capture and
control loop — not the product. Beast gameplay acceptance is required before
promoting the current candidate.

Related prior work: private [solitaire-solver](https://github.com/xSAR-research/solitaire-solver)
(TriPeaks-era predecessor; not archived).

- [Open the QMP QEMU Socket repository](https://github.com/xSAR-research/qmp-qemu-socket)


---

[← Back to the xSAR repository map](README.md)
