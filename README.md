# xSAR Research

**xSAR** means **Search Assess Respond**.

Practical engineering repositories for Rust, Linux, cross-platform utilities,
Raspberry Pi, RP2350, sensing, positioning, signal processing and communications.

The emphasis is on useful functionality, measurable behaviour and enough
technical detail for another person to build, run, evaluate or extend the work.

Core architecture lives in [xsar](https://github.com/xSAR-research/xsar)
(autonomous drone swarm mesh architecture and telemetry orchestration).
Articles and progress notes are published at [xsar.com.au](https://xsar.com.au)
and on X at [@xSAR_Research](https://x.com/xSAR_Research); the site's source
is in [xsar-website](https://github.com/xSAR-research/xsar-website).

## Repository map

### [Cross-platform tools](Cross-platform-tools.md)

**Active** — Portable Rust utilities intended to provide consistent behaviour
across Linux, macOS and Windows.

### [Digital signal processing](Digital-signal-processing.md)

**Early development** — Hardware and software DSP for acquisition, filtering,
spectral analysis and real-time interpretation.

### [Firmware](Firmware.md)

**Early development** — Rust firmware for RP2350-based sensing, control and
communications nodes.

### [Inter-device communications](Inter-device-communications.md)

**Early development** — Reliable links, shared message formats and fault handling
between sensors, embedded controllers, flight controllers and Linux systems.

### [Linux tools](Linux-tools.md)

**Early development** — Linux utilities for storage, file search and triage,
services, inter-process communication, and QEMU host control over an existing
QMP socket with guest screen capture over TCP.

### [Mesh communications and arbitration](Mesh-communications-and-arbitration.md)

**Planned** — Distributed routing, contention control, traffic priority and
recovery for networks of sensor and control nodes.

### [Positioning and navigation](Positioning-and-navigation.md)

**Early development** — GNSS receiver evaluation, position and timing acquisition,
integration with mobile nodes and flight-control systems, and route-planning
practice for search-area coverage.

### [RF — LORAN, Wi-Fi and Bluetooth](RF.md)

**Early development** — RF sensing, timing, positioning and data-link work
across LORAN, Wi-Fi and Bluetooth systems.

### [Rust crates](Rust-crates.md)

**Early development** — Reusable Rust components for Linux applications,
embedded firmware, hardware interfaces and shared protocols, including the
xsar core crate.

### [Sensors](Sensors.md)

**Early development** — Sensor acquisition, precision analogue measurement,
ranging, battery monitoring and embedded sensor-node functionality.

### [Terrain and feature matching](Terrain-and-feature-matching.md)

**Planned** — AI-assisted matching of topographic, optical, LiDAR and thermal
features for localisation, comparison and change detection.

---

## Development status

| Status | Meaning |
|---|---|
| **Planned** | Defined direction or capability without a public implementation yet. |
| **Early development** | Initial design or implementation exists, but the interfaces and operating model are still forming. |
| **Experimental** | Working research functionality; behaviour and interfaces may still change. |
| **Usable** | Documented sufficiently for another person to clone, build and operate. |
| **Active** | In regular use and continuing development. |

### Superseded and archived

**Archived** repositories are retained as technical history or reference after
their functionality has been replaced or superseded by a newer implementation.

---

## Engineering targets

A broad and diverse coverage of the following:

- Rust crates, Linux applications, cross-platform utilities and embedded firmware;
- Arch Linux on x86_64 and Raspberry Pi 5 on aarch64;
- RP2350 firmware, hardware interfaces and CAN FD nodes;
- CAN FD node-to-flight-controller communications and analysis;
- GNSS positioning, velocity, timing and navigation integration;
- hardware and software digital signal processing;
- sensor acquisition, calibration, comparison and visualisation;
- inter-device, mesh and RF communications;
- terrain, topographic and thermal feature matching;
- repeatable datasets, traceable configurations and measurable behaviour.
