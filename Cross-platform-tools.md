# xSAR Cross-Platform Tools

[← Back to the xSAR repository map](README.md)

Portable utilities intended to provide the same core behaviour across Linux,
macOS and Windows.

## Dedup Wordlist

**Status:** Active  
**Implementation:** Rust  
**Platforms:** Linux, macOS and Windows

High-performance wordlist cleaner and de-duplicator for very large text dumps.
It streams and cleans the source, removes invalid entries, performs parallel slab
sorting, and writes a de-duplicated result through a k-way merge.

The utility includes pre-flight storage checks, configurable worker limits,
memory estimates, swap-thrashing risk gates, progress reporting and a final
processing summary.

- [Open the Dedup Wordlist repository](https://github.com/xSAR-research/dedup-wordlist)

## DualScope

**Status:** Experimental  
**Implementation:** Rust  
**Platforms:** Linux, macOS and Windows

Dual-channel CSV viewer in an oscilloscope style. It overlays two `time,value`
captures on an interactive zoom-and-pan plot, with a simple moving-average
filter, colour, line-width and grid controls, and persistent TOML settings.

It is deliberately kept as a style reference: a compact, complete application
used to capture and compare coding conventions, module layout and UI habits.

- [Open the DualScope repository](https://github.com/xSAR-research/dualscope)

---

[← Back to the xSAR repository map](README.md)
