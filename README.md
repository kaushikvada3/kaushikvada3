![Kaushik Vada — Silicon physical design. Implementation, timing, and ML for EDA.](assets/signal-path.svg)

**Physical Design Intern at Tenstorrent** · Previously worked on **SoC physical design at Arm**.

[LinkedIn](https://www.linkedin.com/in/kaushikv198/) · [Résumé](https://docs.google.com/document/d/e/2PACX-1vSyzg7xP-kLY4hlj06RHcTYx3mMqTlArWZOHtVajV9I3I6Unh8v5zvn2t6UqPtoHcnp11qQ7FiBVzmv/pub) · [Browse my repositories](https://github.com/kaushikvada3?tab=repositories)

## AI for timing signoff

> **If we analyze fewer timing corners, which failing paths would we miss?**

That’s the question behind my interest in machine learning for physical design. A path can pass at one voltage and temperature and fail at another. To evaluate a corner-selection model, I’d start with the setup and hold violations from a full run, then check which ones disappear when I use only the selected corners. Those misses tell me where the model needs work.

## From RTL to layout

| Project Obsidian | Two-level cache |
| :--- | :--- |
| **2D graphics accelerator** | **Physical implementation** |
| I use Obsidian to follow a graphics design from RTL into layout. I’m interested in where a short logical connection becomes a long physical wire. | I took a cache through synthesis, placement, and clock-tree synthesis with Synopsys Fusion Compiler and the SAED 32 nm library. |

## Teaching chip design

I developed *Hands-On Introduction to Industry Chip Design Tools*. One exercise I like starts with a late path. Find the driver in the layout, trace the wire to its loads, and decide which part of the path you’d change first.

<details>
<summary><strong>Implementation and analysis tools</strong></summary>

| Task | Tools |
| :--- | :--- |
| Synthesis and place-and-route | Synopsys Fusion Compiler, Cadence Innovus |
| Extraction and timing analysis | Synopsys StarRC, Synopsys PrimeTime, Cadence Tempus |
| Automation | Tcl, Python |

</details>
