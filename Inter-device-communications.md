# xSAR Inter-device Communications

[← Back to the xSAR repository map](README.md)

**Status:** Early development

Reliable communication between sensors, controllers, Linux systems and embedded nodes.

Coverage includes:

- CAN FD, UART, SPI and I²C interfaces;
- framed messages, schemas and versioning;
- addressing, discovery and capability reporting;
- timeouts, retries and fault containment;
- observable link state and diagnostic data;
- transport-independent Rust interfaces where practical.

## CAN FD node-to-flight-controller backplane

The CAN FD work is intended to form the primary communications backplane between
distributed RP2350 sensor or control nodes and the flight controller.

Hardware available or inbound for evaluation includes multiple CAN FD interface
modules, USB CAN/CAN FD analysers and Makerbase CANable-family analyser hardware.
The exact capability of each board will be verified against its controller,
transceiver and firmware before it is assigned a role in the backplane.

The backplane design is expected to cover:

- deterministic identifier allocation and message priority;
- node discovery, identity and capability reporting;
- heartbeat, health and fault-state messages;
- configuration and command acknowledgement;
- sensor data publication with explicit units and scaling;
- bus-load measurement, error-state observation and recovery;
- analyser-assisted interoperability testing;
- classical CAN compatibility only where deliberately required.

---

[← Back to the xSAR repository map](README.md)
