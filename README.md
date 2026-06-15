### Exopoiesis Research

**Designing self-maintaining inorganic systems at the boundary between chemistry and biology.**

We study whether iron sulfide minerals — the same materials found at deep-sea hydrothermal vents — can be engineered into a minimal system that maintains itself without being alive. The core idea: a bilayer pentlandite + mackinawite membrane that drives CO2 reduction to formate using only a pH gradient — no enzymes, no genes, no replication.

---

#### Current work

| Project | Description | Status |
|---------|-------------|--------|
| [interfacial-proton-trap-fes](https://github.com/exopoiesis/interfacial-proton-trap-fes) | **Paper.** Confinement-stabilized interfacial hydrogen/proton trap at the mackinawite/water interface (DFT + apples-to-apples MLIP umbrella sampling) and a pentlandite–mackinawite bilayer membrane | Submitted |
| [magnetic-preflight-neb-gates](https://github.com/exopoiesis/magnetic-preflight-neb-gates) | **Paper.** Magnetic-first pre-flight gates for well-posed DFT NEB in transition-metal sulfides — certify endpoint spin-sheet topology / structural integrity before the expensive band (machine-checked) | Submitted |
| [mlip-vs-dft-iron-sulfides](https://github.com/exopoiesis/mlip-vs-dft-iron-sulfides) | **Paper.** Where foundation MLIPs fail for iron-sulfide defect kinetics — four failure modes + a DFT benchmark of vacancy-anchored H migration (pyrite, marcasite, mackinawite, greigite) | Submitted |
| [ignat](https://github.com/exopoiesis/ignat) | Claude Code skills + specialist agents for scientific paper review, cross-disciplinary insight, and systematic invention — a rigor pipeline (review → ground-check → formalize) | v0.2 |
| [tm-spec](https://github.com/exopoiesis/tm-spec) | One readable YAML file per experiment: a machine-readable specification standard for computational (DFT/MLIP) experiments | Released |
| [corpus-core](https://github.com/exopoiesis/corpus-core) | Shared engine for the reading system — semantic + text search, section-aware chunker, throttled fetching, a generic MCP-server scaffold | Released |
| [arXiv Radar](https://exopoiesis.space/arxiv-radar-chemistry/) | Five daily, self-updating, relevance-filtered arXiv feeds (chemistry · physics · electrochemistry · chemical-engineering · polymers) + an MCP server ([arxiv-radar-mcp](https://github.com/exopoiesis/arxiv-radar-mcp)) to search abstracts and pull full text on demand | Live |
| [lab-corpus-mcp](https://github.com/exopoiesis/lab-corpus-mcp) | MCP server for the research corpus — ingests any literature (PDFs, slides) via MinerU, made searchable through the same embedding stack | Released |
| [prodromos](https://github.com/exopoiesis/prodromos) | A $0 pre-flight gate before expensive DFT — discrimination-optimal window placement and error-probability prediction | Released |
| [sulfide-proton-barriers](https://github.com/exopoiesis/sulfide-proton-barriers) | First intermediate results — preliminary MACE-MP-0 NEB barriers in iron sulfides + the TM6v3 protocell model (refined by the DFT work) | Preliminary |
| [digital-twin](https://github.com/exopoiesis/digital-twin) | ORACLE pipeline: Sobol sensitivity, Gillespie SSA, FNO/PINN surrogates, DFT scripts, SRE monitoring for cloud compute | Active |
| [crystalformer-x](https://github.com/exopoiesis/crystalformer-x) | Post-generation analysis and screening toolkit for CrystalFormer: Voronoi channel analysis, percolation, composition-biased sampling | New |
| [yt-slide-mark](https://github.com/exopoiesis/yt-slide-mark) | Extract slides from YouTube videos and pair them with transcript text in Markdown | Released |
| [exopoiesis.space](https://exopoiesis.github.io) | Project website (EN/RU/ZH) | Live |

#### Key results

- **Pentlandite** blocks protons: E_a = 1.1 eV (GPAW DFT), 0.9 eV (ABACUS DFT), 1.43 eV (MACE-MP-0)
- **Mackinawite** conducts protons via Grotthuss mechanism: E_a = 0.44 eV (MACE), 0.74 eV (GPAW DFT)
- **Pyrite** has low hop barrier but high vacancy formation energy: E_f = 1.95 eV
- Cross-verification across 3 DFT codes (GPAW, Quantum ESPRESSO, ABACUS) + ML potential (MACE)
- Bilayer membrane architecture enables spontaneous CO2 reduction at pH gradient >= 2.3
- ORACLE surrogate model: RF feature importance (AUC = 0.982) identifies k_d as dominant parameter
- System is transport-limited: membrane thickness is the only tunable lever

#### Methods & tools

`Python` · `ASE` · `GPAW` · `Quantum ESPRESSO` · `ABACUS` · `JDFTx` · `MACE-MP-0` · `CrystalFormer` · `MatterGen` · `CHGNet`
`CI-NEB` · `AIMD` · `DFT+U` · `CANDLE solvation` · `Gillespie SSA` · `Sobol sensitivity` · `FNO` · `PINN` · `PyTorch` · `JAX`
`Docker` · `Vast.ai` · `GCP` · `Claude Code`

#### About

Independent researcher, Ukraine. Background in computer hardware engineering.
Funded by [Trelis Research](https://trelis.com) AI compute grant.
This project is developed through human-AI collaboration using [Claude Code](https://claude.ai/code) (Anthropic).

igor@exopoiesis.space | [exopoiesis.space](https://exopoiesis.space)
