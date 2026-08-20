# FireViewer

**Open infrastructure for wildfire observation, spatial reconstruction, temporal tracking and reproducible post-event analysis.**

FireViewer is an independent open-source research and engineering project maintained by **Unicorn Who Dev**.

The project combines geospatial processing, provenance-aware evidence management, AI-assisted analysis, human review and portable spatial/temporal packages so that wildfire incidents can be inspected while active and studied reproducibly afterwards.

> FireViewer is not an emergency alert service, an official wildfire source, a command tool or a certified propagation predictor.

## What we are building

```text
sources + observations
        ↓
provenance + evidence
        ↓
AI analysis / localisation / abstention
        ↓
human review
        ↓
reproducible spatial map build
        +
reviewed temporal fire states
        ↓
public exploration / replay / datasets / post-event studies
```

### Spatial reconstruction

The canonical map builder is headless and endpoint-driven. It produces portable OpenUSD/Blender map packages from measured geographic inputs on a Lambert-93 tile grid.

**FireViewer core no longer depends on Unity or NVIDIA Omniverse.** Omniverse can still be used in optional synthetic-data R&D inside the SDG workstream.

### Fire evolution

Observed, reconstructed, interpolated, simulated and predicted states remain separate. Unknown intervals stay unknown instead of being silently filled.

### Replay and research

FireViewer aims to preserve enough provenance, hashes, model/tool revisions and human decisions to reopen an incident later and use it for reproducible post-event studies, datasets and benchmarks.

## Repositories

| Component | Responsibility |
| --- | --- |
| **Documentation** | Architecture, status, safety, reproducibility and roadmap. |
| **Models** | Public model/dataset inventory, lifecycle, benchmark evidence and machine-readable registries. |
| **Frontend** | Contribution, human review and public 2D/3D exploration. |
| **Backend** | Incident registry, evidence, orchestration, audit and publication. |
| **AI worker** | Private analysis, visual anchors, localisation attempts and abstention. |
| **Spatial** | Headless map builder, geographic packages and temporal perimeter layers. |
| **SDG** | Optional synthetic-data and simulation research. |

- Documentation: <https://github.com/fireviewer/Fireviewer_doc>
- Model/data index: <https://github.com/fireviewer/models>
- Hugging Face: <https://huggingface.co/fireviewer>

## Models and datasets

The main public showcase follows the current FireViewer inventory rather than surfacing every historical artifact equally.

Current model work is represented by **seven active Hugging Face checkpoints** across fire/smoke detection and segmentation/representation research.

Current public data highlights include:

- `fire-smoke-detection-corpus-v1`;
- `prithvi-burnscars-training-dataset-v1`;
- `dinov3-cross-view-fireviewer-v1-dataset`;
- `simple-measured-scenes-v1` for measured spatial map builds.

Historical `firewarning-*` resources and older simulation/Omniverse packs are retained for compatibility, provenance and reproducibility but are **not promoted as the current primary FireViewer datasets**.

See the reviewed [Hugging Face inventory](https://github.com/fireviewer/models/blob/main/docs/HUGGING_FACE_INVENTORY.md) for the exact current/restricted/legacy classification.

## Looking for support and collaborators

FireViewer is currently maintained with limited independent resources. The project is looking for:

- GPU and CPU compute credits;
- object-storage and bandwidth support;
- geospatial / remote-sensing collaboration;
- wildfire-domain review;
- reproducible benchmark and evaluation support;
- research partnerships;
- grants or sponsorship that can fund infrastructure and sustained development.

Support does not buy influence over scientific conclusions or publication decisions.

See the canonical [Project Overview](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/PROJECT_OVERVIEW.md), [Funding Brief](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/FUNDING_BRIEF.md) and [Support & Partnerships](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/SUPPORT_AND_PARTNERSHIPS.md).

## Contact

Research, infrastructure support, sponsorship, provenance, security or data-removal requests:

**unicornwhodev@gmail.com**

---

### En français

FireViewer est une infrastructure ouverte de **documentation des incendies, reconstruction spatiale, suivi temporel et étude reproductible après événement**. Les ressources historiques restent disponibles pour la traçabilité, mais la vitrine principale privilégie les modèles, datasets et builds spatiaux qui représentent l'état actuel du projet.
