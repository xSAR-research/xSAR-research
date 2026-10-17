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

## Basic Route Planning

**Status:** Early development

Console Rust workspace for route-planning practice ahead of Dijkstra and A*
shortest-path work for drones. It uses a deterministic card-game process to
simulate a weighted routing model with impasses on different routes. Deals are
ingested through the shared `xsar::pyramid_json` codec, with strict bounded
input and deterministic output.

- **Pyramid** presents 1,432 possible routes, most of which end in an impasse,
  so an A* approach is needed to find a way through.
- **Spider** (planned) introduces recon-detection routing to simulate complete
  search-area coverage, plus rerouting back to branch points to try other
  branches. Obscured card values supply the unknown permutations.
- **TriPeaks** (planned) works in a similar way: many routes stay unknown until
  traversal, simulated by obscured cards that are only revealed as you go.

The overall aim is to model search-area coverage with weighting on different
paths, where obscured cards stand in for impassable features such as rough
terrain, or areas that can't be searched because of flooding or uncontrolled
bushfires.

- [Open the Basic Route Planning repository](https://github.com/xSAR-research/basic-route-planning)

---

[← Back to the xSAR repository map](README.md)
