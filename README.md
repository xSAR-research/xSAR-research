# xSAR Research

Practical research and engineering projects spanning Rust, Linux, Raspberry Pi,
embedded systems, sensors, data acquisition and supporting infrastructure.

Projects range from early hardware evaluation through to usable software tools.
Repository status is shown clearly so visitors can distinguish working
applications from active experiments and planned work.

## Project map

- **xSAR**
  - [Sensors](Sensors.md)
    - [Thermal and precision ADC](Sensors.md#thermal-and-precision-adc)
      - [xSAR Sensor Harvester](https://github.com/xSAR-research/xsar-sensor-harvester)
      - [xSAR Sensor Logger Display](https://github.com/xSAR-research/xsar-sensor-logger-display)
      - [ADS1256 Precision ADC Bench](Sensors.md#ads1256-precision-adc-bench)
    - [Ranging](Sensors.md#ranging)
      - [LiDAR](Sensors.md#lidar)
      - [Doppler ranging](Sensors.md#doppler-ranging)
    - [Power and battery measurement](Sensors.md#power-and-battery-measurement)
      - [Current and voltage sensing](Sensors.md#current-and-voltage-sensing)
      - [Coulomb-counting battery state](Sensors.md#coulomb-counting-battery-state)
    - [Embedded sensor nodes](Sensors.md#embedded-sensor-nodes)
      - [RP2350 CAN FD Node Firmware](https://github.com/xSAR-research/xsar-node-firmware-can-fd)
  - [Linux tools](Linux-tools.md)
    - [Warm Drive Cache](https://github.com/xSAR-research/warm-drive-cache)
    - [Message Queue Framework](Linux-tools.md#message-queue-framework)

The project map is the front door. Major areas have their own Markdown index so
the profile remains concise while project descriptions and navigation can grow.

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
