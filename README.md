# Kaushik Vada

**Physical design intern at Tenstorrent. Previously, SoC physical design at Arm.**

[LinkedIn](https://www.linkedin.com/in/kaushikv198/) · [Résumé](https://docs.google.com/document/d/e/2PACX-1vSyzg7xP-kLY4hlj06RHcTYx3mMqTlArWZOHtVajV9I3I6Unh8v5zvn2t6UqPtoHcnp11qQ7FiBVzmv/pub) · [Browse my repositories](https://github.com/kaushikvada3?tab=repositories)

![Illustrative chip floorplan with a signal route highlighted between two cells.](assets/signal-path.svg)

A timing report tells me a path is late. The part I enjoy is finding out why. I trace the path through the layout, separate cell delay from wire delay, and look at what else shares the driver before changing it.

## Machine learning for timing signoff

**Can a smaller set of timing corners still catch the paths that fail?** A path can meet timing at one voltage and temperature and fail at another. I’m exploring how to select corners with machine learning, then compare that selection against a full analysis. The first thing I look for is a setup or hold violation the smaller set missed.

## Selected hardware

### Ten-cell battery management system

I worked on the six-layer board and STM32 firmware for a ten-cell pack. The firmware sends cell voltages, temperature readings, and pack current over USB. You can follow a measurement from the board into the desktop dashboard in the [battery management system repository](https://github.com/kaushikvada3/BMS-Senior-Design).

### Two-level cache

I took a cache from RTL through synthesis, placement, and clock-tree synthesis in Synopsys Fusion Compiler using the SAED 32 nm library.

### Project Obsidian

A 2D graphics accelerator I use to explore how decisions in graphics RTL carry through to physical layout.

## Teaching chip design

I developed *Hands-On Introduction to Industry Chip Design Tools*. One exercise I like is to give someone a timing report and ask them to find the slow path on the layout. Once they can point to the driver, the wire, and its loads, the delay numbers have a physical explanation.

<details>
<summary>Tools I use for implementation and timing</summary>

- **Implementation** — Synopsys Fusion Compiler and Cadence Innovus
- **Extraction and timing** — Synopsys StarRC, Synopsys PrimeTime, and Cadence Tempus
- **Automation** — Tcl and Python

</details>
