# Autonomous Geospatial AI — Supervisor & Sub-agents (interactive walkthrough)

A self-contained, bilingual (EN / EL) interactive walkthrough of a proposed **autonomous geospatial AI** architecture (planner / sub-agents, GeoRAG, independent guardrail). It accompanies **Chapter 8 — Future Work** of an MSc thesis in Geography & Geoinformatics on semantic segmentation of multispectral/thermal UAV imagery (MicaSense Altum-PT sensor; study area: Pamfila, Lesvos).

**Live demo (GitHub Pages):** _https://<USERNAME>.github.io/geospatial-ai-pipeline-walkthrough/_ (filled in after Pages is enabled)

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

## Sources (open access / Elsevier)

- Perez, E., et al. (2018). FiLM: Visual Reasoning with a General Conditioning Layer. arXiv:1709.07871
- Gu, A., & Dao, T. (2023). Mamba: Linear-Time Sequence Modeling with Selective State Spaces. arXiv:2312.00752
- Li, F., et al. (2025). LMVMamba. Remote Sensing, 17(19), 3367. https://doi.org/10.3390/rs17193367
- Cao, Y., et al. (2025). Vision Mamba RS segmentation. Remote Sensing, 17(8), 1390
- Shi, Y., et al. (2025). AuxDet. arXiv:2505.15184
- Wang, J., et al. (2025). GeoRAG. arXiv:2504.01458
- Liang, J., et al. (2025). GeoGraphRAG. Int. J. Applied Earth Observation and Geoinformation, 142, 104712 (Elsevier)
- Lundberg, S. M., & Lee, S.-I. (2017). SHAP. arXiv:1705.07874
- Anthropic (2024). Model Context Protocol (MCP).

Infrastructure/tools: PostGIS, pgvector, Arize Phoenix.

## License

Code: MIT. Content/figures: CC BY 4.0. © Nikolaos Koroniadis.

---

*Created as companion educational/presentation material for Chapter 8 of the thesis.*
