# xSAR Positioning and Navigation

[← Back to the xSAR repository map](README.md)

**Status:** Early development

Position, velocity and timing acquisition for mobile nodes, flight-control
systems and sensor platforms.

## GNSS receiver evaluation

Hardware available for comparative testing includes u-blox NEO-6M,
NEO-7-series and NEO-M8-family receiver modules.

The initial work will compare:

- receiver configuration and host interfaces;
- cold, warm and hot start behaviour;
- fix availability, reported accuracy and update rate;
- antenna placement and interference sensitivity;
- position, velocity and timing output;
- repeatability under static and moving conditions;
- integration with Raspberry Pi 5 and RP2350-based systems.

The NEO-M8 family extends the work beyond GPS-only reception, with support for
GPS/QZSS, Galileo, GLONASS and BeiDou, including concurrent use of multiple GNSS
constellations where supported by the module variant and configuration.

## Navigation integration

The longer-term direction includes:

- a common Rust representation for position, velocity, time and fix quality;
- recorded datasets for receiver and antenna comparison;
- fusion boundaries for inertial, terrain and feature-matching inputs;
- clear separation between receiver transport, protocol parsing and navigation logic;
- health, integrity and loss-of-fix reporting to the flight controller.

---

[← Back to the xSAR repository map](README.md)
