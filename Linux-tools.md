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

---

[← Back to the xSAR repository map](README.md)
