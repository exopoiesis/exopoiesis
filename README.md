### Exopoiesis Research

**Designing self-maintaining inorganic systems at the boundary between chemistry and biology.**

We study whether iron sulfide minerals — the same materials found at deep-sea hydrothermal vents — can be engineered into a minimal system that maintains itself without being alive. The core idea: a bilayer pentlandite + mackinawite membrane that drives CO2 reduction to formate using only a pH gradient — no enzymes, no genes, no replication.

---

#### Current work

| Project | Description | Status |
|---------|-------------|--------|
| [digital-twin](https://github.com/exopoiesis/digital-twin) | ORACLE pipeline: Sobol sensitivity, Gillespie SSA, FNO/PINN surrogates, DFT scripts, SRE monitoring for cloud compute | Active |
| [sulfide-proton-barriers](https://github.com/exopoiesis/sulfide-proton-barriers) | DFT NEB calculations of H+ diffusion barriers in iron sulfides (pentlandite, mackinawite, pyrite, troilite) | Active |
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
