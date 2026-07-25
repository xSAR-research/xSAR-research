# xSAR Linux and Cross-Platform Tools

[← Back to the xSAR repository map](README.md)

Practical utilities and supporting frameworks for Linux systems work, portable
command-line processing, service integration and data handling.

## Dedup Wordlist

**Status:** Active  
**Implementation:** Rust  
**Platforms:** Linux, macOS and Windows

High-performance wordlist cleaner and de-duplicator for very large text dumps.
It streams and cleans the source, removes invalid entries, performs parallel slab
sorting, and writes a de-duplicated result through a k-way merge.

The utility includes pre-flight storage checks, configurable worker limits,
memory estimates, swap-thrashing risk gates, progress reporting and a final
processing summary.

- [Open the Dedup Wordlist repository](https://github.com/xSAR-research/dedup-wordlist)

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
