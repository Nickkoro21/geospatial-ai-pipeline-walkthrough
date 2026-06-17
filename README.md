# Autonomous Geospatial AI — Supervisor & Sub-agents 🛰️🤖

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-2E8B52?logo=github&logoColor=white)](https://nickkoro21.github.io/geospatial-ai-pipeline-walkthrough/)
[![License: MIT](https://img.shields.io/badge/Code-MIT-blue.svg)](#license)
[![Content: CC BY 4.0](https://img.shields.io/badge/Content-CC%20BY%204.0-lightgrey.svg)](#license)
[![HTML5](https://img.shields.io/badge/HTML5-no%20dependencies-E34F26?logo=html5&logoColor=white)](#tech)
[![SVG](https://img.shields.io/badge/SVG-vector-FFB13B?logo=svg&logoColor=white)](#tech)
[![Languages](https://img.shields.io/badge/i18n-EN%20%2F%20EL-5C6699)](#features)
[![Built with Claude](https://img.shields.io/badge/Built%20with-Claude%20(Anthropic)-D4A27F)](#credits)
[![Made with coffee](https://img.shields.io/badge/Made%20with-%E2%98%95%20coffee-6F4E37)](#made-with)

A self-contained, **bilingual (EN / EL) interactive walkthrough** of a proposed **autonomous geospatial AI** architecture — a planner that delegates to specialist sub-agents (GeoRAG), with an independent guardrail before any answer is returned. It accompanies **Chapter 8 — Future Work** of an MSc thesis in Geography & Geoinformatics on semantic segmentation of multispectral/thermal UAV imagery (MicaSense Altum-PT sensor; study area: Pamfila, Lesvos).

> **▶ Live demo:** https://nickkoro21.github.io/geospatial-ai-pipeline-walkthrough/

---

## What it shows

A step-by-step "query-to-answer" flow:

1. Read documents (OCR) → Document vector store
2. Web sources (approved domains)
3. Spatial geodatabase
4. Planner (supervisor) + three sub-agents with two-way dialogue
5. Authenticate & access (identity + rights)
6. Receive query + Clarify & refine
7. The planner dispatches three queries
8. Answers → Compose report (three deliverables)
9. Independent validator (checks rights & permitted output, no prompt knowledge)
10. Final answer (allow) — the Blocked path is shown but not triggered

Each step includes a small example pane (papers, ESRI `.emd` metadata, sample geodatabase records, a user session, an ambiguous → refined query dialogue, and a final map + "Download data" badge).

## Features

- Single `index.html` — **no dependencies** (inline SVG + vanilla JS).
- Language toggle with flags (default: English; Greek available).
- Dynamic full-screen layout, mobile-friendly, Play / Next / Prev / Restart.

## Run locally

Just open `index.html` in any modern browser — no build step, no server required.

<a id="tech"></a>
## Tech

Plain HTML5, hand-written inline SVG (icons, nodes, flags), vanilla JavaScript for the step state machine. No frameworks, no external requests.

## Sources (open access)

All links verified (June 2026).

- Perez, E., et al. (2018). [FiLM: Visual Reasoning with a General Conditioning Layer](https://arxiv.org/abs/1709.07871). AAAI / arXiv:1709.07871
- Gu, A., & Dao, T. (2023). [Mamba: Linear-Time Sequence Modeling with Selective State Spaces](https://arxiv.org/abs/2312.00752). arXiv:2312.00752
- Li, F., et al. (2025). [LMVMamba: A Hybrid U-Shape Mamba for Remote Sensing Segmentation](https://doi.org/10.3390/rs17193367). Remote Sensing, 17(19), 3367
- Cao, Y., et al. (2025). [Remote Sensing Image Segmentation Using Vision Mamba](https://www.mdpi.com/2072-4292/17/8/1390). Remote Sensing, 17(8), 1390
- Shi, Y., et al. (2025). [AuxDet: Auxiliary Metadata Matters for Omni-Domain Infrared Small Target Detection](https://arxiv.org/abs/2505.15184). arXiv:2505.15184
- Wang, J., et al. (2025). [GeoRAG: A Question-Answering Approach from a Geographical Perspective](https://arxiv.org/abs/2504.01458). arXiv:2504.01458
- Lundberg, S. M., & Lee, S.-I. (2017). [A Unified Approach to Interpreting Model Predictions (SHAP)](https://arxiv.org/abs/1705.07874). NeurIPS / arXiv:1705.07874
- Anthropic (2024). [Introducing the Model Context Protocol (MCP)](https://www.anthropic.com/news/model-context-protocol).

Infrastructure/tools referenced: PostGIS, pgvector, Arize Phoenix.

## Author

**Nikolaos Koroniadis** — MSc in Geography & Geoinformatics · GitHub [@Nickkoro21](https://github.com/Nickkoro21)
T-6 Texan II instructor pilot; interests in data science, GIS, deep learning, cartography, and human-factors accident analysis.

<a id="credits"></a>
## Credits & acknowledgements

- **Concept, direction & domain expertise:** Nikolaos Koroniadis
- **Design & implementation assistance:** Claude (Anthropic) — diagram, iconography, bilingual UI, and this walkthrough were co-developed with Claude.
- Thanks to the open-access research community whose work is referenced above.

## Contributors

[![Contributors](https://contrib.rocks/image?repo=Nickkoro21/geospatial-ai-pipeline-walkthrough)](https://github.com/Nickkoro21/geospatial-ai-pipeline-walkthrough/graphs/contributors)

## License

- **Code:** MIT
- **Content & figures:** CC BY 4.0

© 2026 Nikolaos Koroniadis.

<a id="made-with"></a>
---

<p align="center"><em>Made with ☕ coffee and ❤️ in Kalamata, Greece.</em></p>
