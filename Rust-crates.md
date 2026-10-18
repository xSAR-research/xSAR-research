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

## xSAR core crate

**Status:** Experimental  
**Latest version:** 0.4.100 (numeric `major.minor.build` migration checkpoint;
verification pending)

The shared [xsar](https://github.com/xSAR-research/xsar) crate. Its root holds
the drone telemetry types (node state, flight mode, position, flight-controller
state and mesh telemetry) with no external dependencies by default. Optional
features add reusable QMP transport, pixel-to-QMP geometry, PNG decoding,
image-matching scans, a bounded TCP capture client, and card and deal models
with the bounded `pyramid_json` codec used by QMP QEMU Socket and Basic Route
Planning.

Recent highlights from the changelog:

- TCP capture client for version-3 full-screen BGR8 frames with bounded
  persistent sessions, cooperative cancellation and idle-disconnect recovery;
- `pyramid_json` schema 2 with explicit card values, while still reading
  schema 1 strictly;
- allocation-free bottom-up black-run search for menu and button detection;
- move to Charlie's numeric version policy, with a build counter independent of
  the QMP QEMU Socket application.

- [Open the xsar repository](https://github.com/xSAR-research/xsar)

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
