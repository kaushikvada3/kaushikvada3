<h1 align="center">Kaushik Vada</h1>
<p align="center"><strong>ASIC physical design &nbsp;·&nbsp; Timing analysis &nbsp;·&nbsp; Machine learning for EDA</strong></p>
<p align="center">Physical Design Intern at <b>Tenstorrent</b> &nbsp;|&nbsp; Previously, SoC Physical Design at <b>Arm</b></p>
<p align="center"><a href="https://www.linkedin.com/in/kaushikv198/">LinkedIn</a> &nbsp;·&nbsp; <a href="https://docs.google.com/document/d/e/2PACX-1vSyzg7xP-kLY4hlj06RHcTYx3mMqTlArWZOHtVajV9I3I6Unh8v5zvn2t6UqPtoHcnp11qQ7FiBVzmv/pub">Résumé</a> &nbsp;·&nbsp; <a href="https://github.com/kaushikvada3?tab=repositories">Repositories</a></p>

---

I like the moment a timing report sends me back to the layout. Two gates can look close together in RTL and end up far apart on silicon. When a path misses timing, I want to know how much delay came from the cells, how much came from the wire, and what a fix would do to the other paths sharing that driver.

## Research focus · AI for timing signoff

> **Which operating conditions do we need to analyze to catch the paths that fail timing?**

A path that limits frequency at one timing corner can look comfortable at another. I’m exploring how machine learning can help select corners for analysis. The test I care about is whether a smaller set still catches the setup and hold violations found by the full set. A single missed violation can matter more than a small average prediction error.

## Hardware portfolio

| Project | Engineering work |
| :--- | :--- |
| **Project Obsidian**<br>2D graphics accelerator | I use this design to trace the path from graphics RTL to physical layout. |
| **Two-level cache**<br>Digital implementation | I took a cache through synthesis, placement, and clock-tree synthesis in Fusion Compiler with the SAED 32 nm library. |
| **Ten-cell battery management system**<br>Board design and firmware | I worked on a six-layer PCB and STM32 firmware that measures cell voltage, pack current, and temperature. A USB connection brings those readings into a dashboard. |

<details>
<summary><b>Inside my toolchain</b></summary>

| Task | Tools |
| :--- | :--- |
| Synthesis, placement, and clock trees | Synopsys Fusion Compiler, Cadence Innovus |
| Extraction and static timing analysis | Synopsys StarRC and PrimeTime, Cadence Tempus |
| Automation and report analysis | Tcl, Python |

</details>

## Teaching chip design

I developed *Hands-On Introduction to Industry Chip Design Tools*. One exercise I like is to pick a slow path in a report, locate its cells in the layout, and trace the wires between them. It makes the connection between a number in a report and a physical design decision visible.
