# xSAR Firmware

[← Back to the xSAR repository map](README.md)

**Status:** Early development

Rust firmware for embedded sensing, control and communications, with current emphasis on RP2350-based nodes.

Coverage includes:

- RP2350 firmware and board-level hardware interfaces;
- deterministic acquisition and control loops;
- CAN FD sensor and control nodes;
- node identity, configuration and health reporting;
- flight-controller backplane participation;
- protocol separation for reuse across transports;
- build, flash, verification and recovery workflows.

## CAN FD node firmware

The RP2350 node firmware will provide the embedded endpoint for the CAN FD
node-to-flight-controller backplane. Each node should expose its identity,
capabilities, sensor or actuator data, configuration state and health without
leaking board-specific details into the shared protocol.

Current implementation:

- [RP2350 CAN FD Node Firmware](https://github.com/xSAR-research/xsar-node-firmware-can-fd)

---

[← Back to the xSAR repository map](README.md)
