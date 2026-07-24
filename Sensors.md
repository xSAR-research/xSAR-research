# xSAR Sensors

[← Back to the xSAR project map](README.md)

Sensor acquisition, ranging, power measurement and embedded-node projects.
Projects range from early hardware evaluation through to runnable Rust tools and
firmware.

## Thermal and precision ADC

### xSAR Sensor Harvester

**Status:** Experimental

Raspberry Pi sensor acquisition using the ADS1115, NTC thermistors and a BMP180
reference sensor.

- [Open the xSAR Sensor Harvester repository](https://github.com/xSAR-research/xsar-sensor-harvester)
- Current acquisition interface: I²C
- Current experiment: compare physical NTC dividers while rotating ADS1115 input channels

### xSAR Sensor Logger Display

**Status:** Experimental

Rust desktop viewer for comparing timestamped sensor captures using elapsed-time,
oscilloscope-style plots.

- [Open the xSAR Sensor Logger Display repository](https://github.com/xSAR-research/xsar-sensor-logger-display)
- Current data source: xSAR Sensor Harvester CSV captures
- Current focus: repeatable comparison of multiple overnight runs

### ADS1256 Precision ADC Bench

**Status:** Planned

SPI-connected evaluation of the 24-bit, eight-channel ADS1256, including noise,
gain, channel multiplexing, settling behaviour and comparison against the existing
ADS1115 acquisition path.

## Ranging

### LiDAR

**Status:** Planned

Evaluation and integration of optical ranging sensors, including measurement
repeatability, target behaviour, interface support and usable range.

### Doppler ranging

**Status:** Planned

High-resolution Doppler and radar-based range and velocity measurement, including
sensors targeting sub-centimetre precision over approximately five metres.

## Power and battery measurement

### Current and voltage sensing

**Status:** Planned

Precision acquisition of electrical-system voltage and current for power analysis
and battery monitoring.

### Coulomb-counting battery state

**Status:** Planned

Charge integration and battery state-of-charge estimation based on measured current,
voltage, elapsed time and calibration data.

## Embedded sensor nodes

### RP2350 CAN FD node firmware

**Status:** Early development

Rust firmware for distributed RP2350-based CAN FD sensor and control nodes.

- [Open the RP2350 CAN FD Node Firmware repository](https://github.com/xSAR-research/xsar-node-firmware-can-fd)

---

[← Back to the xSAR project map](README.md)
