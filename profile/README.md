# FireViewer

**Evidence-centred infrastructure for documenting, reviewing, mapping and studying wildfire events.**

FireViewer is an independent research and engineering project maintained by **Unicorn Who Dev**. It combines public and official sources, authorised contributions, deterministic geographic processing, machine-assisted analysis, human review and reproducible spatial products while preserving provenance and uncertainty.

> FireViewer is not an emergency alert service, an official wildfire source, an incident-command tool or a certified fire-propagation predictor. In an emergency, follow the relevant authorities and emergency services.

## System overview

```text
public / official sources + authorised media
                    |
                    v
        acquisition and provenance
                    |
                    v
     visual observations and evidence
                    |
                    v
 deterministic geographic hypotheses
                    |
                    v
 versioned event evidence and history
                    |
                    v
 multimodal assessment / abstention
                    |
                    v
       policy gate and human review
                    |
                    v
 reviewed event state + spatial products
```

Visual detections remain image-space evidence. Geographic candidates are produced separately from camera, map, terrain, satellite and event-history evidence. A multimodal assessment may accept, reject or abstain; it cannot silently turn a visual detection into geographic truth.

The current deterministic fire-state reconstruction is **Part.4 3.2**. Its baseline fusion profile remains uncalibrated and therefore cannot authorize unattended publication.

## Repositories

| Resource | Role | Public status |
| --- | --- | --- |
| [Fireviewer_doc](https://github.com/fireviewer/Fireviewer_doc) | Canonical architecture, status, governance, safety and repository documentation. | Public |
| [fireviewer-ai-worker](https://github.com/fireviewer/fireviewer-ai-worker) | Evidence acquisition, visual processing, geographic hypotheses, satellite evidence, event dossiers and point assessment. | Public |
| [fireviewer-spatial](https://github.com/fireviewer/fireviewer-spatial) | Deterministic map production, portable spatial packages, observed temporal layers and validation. | Public |
| [fireviewer-sdg](https://github.com/fireviewer/fireviewer-sdg) | Synthetic-data and simulation research kept separate from real-event evidence. | Public |
| [FireViewer on Hugging Face](https://huggingface.co/fireviewer) | Model cards, dataset cards, weights, measured maps and hosted research artifacts. | Mixed public / restricted |

The frontend, backend and model registry are currently private implementation repositories. Their roles are documented in the [repository guide](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/public/REPOSITORIES.md) without presenting their source as publicly accessible.

## Maps, simulation and legacy artifacts

FireViewer keeps three artifact families deliberately separate:

- **Measured maps** — real geographic map builds. The canonical Hub repository is [`simple-measured-scenes-v1`](https://huggingface.co/datasets/fireviewer/simple-measured-scenes-v1). Existing package paths may be consumed directly by the viewer and must not be renamed or reorganised without an explicit migration.
- **Synthetic and reproduction material** — Omniverse scenarios, generated observations and historical reproduction packs. These are not measured-map productions and are never real-event evidence.
- **Legacy models** — deprecated, superseded, incomplete or low-quality checkpoints retained only for provenance and reproducibility. They are kept outside the active public model list and consolidated in a private archive when retained.

Historical `firewarning-*` names can remain in slugs, manifests or source namespaces for compatibility. They do not identify a separate active project.

## Evidence and safety boundary

FireViewer preserves source identity, time, rights, hashes, revisions, uncertainty and review outcomes when applicable. The acquisition pipeline is not intended to become a shadow archive of third-party articles, public media or transcripts.

Observation, geographic hypothesis, reconstruction, simulation, prediction and publication are distinct result types. A detector box is not a GPS coordinate; a thermal footprint is not an exact fire front; a simulated scene is not evidence of a real incident.

When evidence is insufficient, **unknown** or **abstain** is preferable to unsupported precision.

## Current maturity

FireViewer is an active research MVP. Core contracts, acquisition paths, deterministic geographic processing, satellite evidence, review surfaces, Part.4 3.2 reconstruction and spatial tooling exist, but the complete real-data path has not been qualified as an unattended production service.

The dated implementation boundary is maintained in [`STATUS.md`](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/public/STATUS.md).

## Contribute or collaborate

Contributions to software, mapping, accessibility, provenance, data governance, evaluation and research validation are welcome. Infrastructure credits, lawful evaluation data and research partnerships can also materially support the project.

Do not use GitHub to report an emergency or request assistance.

For research, infrastructure, security, provenance, rights or data-removal enquiries: **unicornwhodev@gmail.com**.
