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

---

[← Back to the xSAR repository map](README.md)
