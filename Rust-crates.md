# xSAR Rust Crates

[← Back to the xSAR repository map](README.md)

**Status:** Early development

Reusable Rust components for Linux applications, embedded firmware, hardware interfaces and shared protocols.

Coverage includes:

- versioned data and message schemas;
- sensor and acquisition abstractions;
- Linux and embedded transport boundaries;
- parsing, validation and calibration support;
- explicit target, feature and MSRV requirements;
- examples and tests that demonstrate intended use.

## CAN FD backplane protocol crate

**Status:** Early development

A shared Rust crate is planned as the authoritative definition of communication
between RP2350 nodes and the flight controller. It should be usable from both
embedded firmware and Linux-side tooling without coupling the protocol to a
particular CAN controller or transceiver.

The crate direction includes:

- stable message identifiers and priority classes;
- typed frame payloads with explicit units and scaling;
- encode, decode and validation support;
- protocol and schema version negotiation;
- node identity, capability, heartbeat and fault messages;
- `no_std`-capable protocol types where practical;
- adapters at the boundary for embedded CAN FD drivers and Linux SocketCAN;
- golden vectors and cross-target compatibility tests.

---

[← Back to the xSAR repository map](README.md)
