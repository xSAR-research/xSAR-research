# xSAR Research

Practical research and engineering projects spanning Rust, Linux, Raspberry Pi,
embedded systems, sensors, data acquisition and supporting infrastructure.

Projects range from early hardware evaluation through to usable software tools.
Repository status is shown clearly so visitors can distinguish working
applications from active experiments and planned work.

## Project map

```text
xSAR
├── Sensors
│   ├── Thermal and precision ADC
│   │   ├── Sensor harvester
│   │   ├── Sensor logger display
│   │   └── ADS1256 precision ADC bench
│   │
│   ├── Ranging
│   │   ├── LiDAR
│   │   └── Doppler ranging
│   │
│   ├── Power and battery measurement
│   │   ├── Current and voltage sensing
│   │   └── Coulomb-counting battery state
│   │
│   └── Embedded sensor nodes
│       └── RP2350 CAN FD firmware
│
└── Linux tooling
    ├── Warm Drive Cache
    └── Message Queue Framework
```

---

## Sensors

### Thermal and precision ADC

| Project | Status | Purpose |
|---|---|---|
| [xSAR Sensor Harvester](https://github.com/xSAR-research/xsar-sensor-harvester) | Experimental | Raspberry Pi sensor acquisition using ADS1115, NTC thermistors and a BMP180 reference sensor. |
| [xSAR Sensor Logger Display](https://github.com/xSAR-research/xsar-sensor-logger-display) | Experimental | Rust desktop viewer for comparing timestamped sensor captures using elapsed-time, oscilloscope-style plots. |
| ADS1256 Precision ADC Bench | Planned | SPI-connected 24-bit, eight-channel ADC evaluation, noise characterisation and multiplexed-channel testing. |

### Ranging

| Project | Status | Purpose |
|---|---|---|
| LiDAR sensing | Planned | Evaluation and integration of optical ranging sensors. |
| Doppler ranging | Planned | High-resolution Doppler and radar-based range and velocity measurement. |

### Power and battery measurement

| Project | Status | Purpose |
|---|---|---|
| Current and voltage sensing | Planned | Precision acquisition of electrical system voltage and current. |
| Coulomb-counting battery state | Planned | Charge integration and battery state-of-charge estimation. |

### Embedded sensor nodes

| Project | Status | Purpose |
|---|---|---|
| [RP2350 CAN FD Node Firmware](https://github.com/xSAR-research/xsar-node-firmware-can-fd) | Early development | Rust firmware for distributed RP2350-based CAN FD sensor and control nodes. |

---

## Linux tools

| Project | Status | Purpose |
|---|---|---|
| [Warm Drive Cache](https://github.com/xSAR-research/warm-drive-cache) | Active | Linux storage tooling for controlled cache warming and data placement. |
| Message Queue Framework | Planned | A reusable Linux message-queue framework for communication between services, acquisition processes and analysis tools. |

---

## Project status

| Status | Meaning |
|---|---|
| **Usable** | Documented and ready for others to clone, build and operate. |
| **Active** | In regular use and continuing development. |
| **Experimental** | Working research prototype; interfaces and behaviour may change. |
| **Early development** | Initial implementation exists but is not yet a complete working system. |
| **Planned** | Defined project direction without a public implementation yet. |
| **Archived** | Retained for reference but no longer under active development. |

---

## Engineering focus

Current work centres on:

- Rust applications and embedded firmware
- Arch Linux on x86_64 and Raspberry Pi 5
- Linux hardware interfaces including I²C, SPI, UART and CAN FD
- Precision analogue acquisition and sensor validation
- Repeatable experimental datasets and traceable hardware configurations
- Practical tools that can move from a breadboard experiment to a documented,
  runnable repository

Each repository aims to provide a clear project status, hardware requirements,
build instructions, current limitations and the next meaningful milestone.
