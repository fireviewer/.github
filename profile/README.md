# FireViewer

**Evidence-centred infrastructure for documenting, reviewing, mapping, and
studying wildfire events.**

FireViewer is an independent research and engineering project maintained by
**Unicorn Who Dev**. It connects public sources, authorised contributions,
official geographic products, deterministic calculations, machine-assisted
analysis, and human review while preserving provenance and uncertainty.

> FireViewer is not an emergency alert service, an official wildfire source,
> an incident-command tool, or a certified fire-propagation predictor. In an
> emergency, follow the relevant authorities and emergency services.

## How the system is designed

```text
sources and authorised media
            |
            v
evidence tickets and visual observations
            |
            v
deterministic geographic hypotheses
            |
            v
versioned event evidence and history
            |
            v
multimodal assessment and explicit abstention
            |
            v
policy gate, human review, and versioned publication
```

Visual detectors provide boxes and scores; they do not create GPS truth. A
separate geographic stage uses the upload position, camera metadata, terrain,
maps, satellite references, and earlier reviewed event states to propose
candidate points. The final multimodal stage judges those candidates and may
accept, reject, or abstain. It cannot silently overwrite the original point.

Automatic-publication eligibility requires an accepted result, calibrated
confidence strictly above 0.85, a managed multimodal provider, and no missing
required evidence or hard contradiction. Other results require human review;
a correction is stored as a competing JSON object with its own evidence trail.

## Publicly accessible resources

| Resource | Role |
| --- | --- |
| [Fireviewer_doc](https://github.com/fireviewer/Fireviewer_doc) | Canonical project, architecture, safety, data-governance, and current-status documentation. |
| [fireviewer-ai-worker](https://github.com/fireviewer/fireviewer-ai-worker) | Evidence acquisition, visual processing, geographic hypotheses, provider adapters, and point assessment. |
| [fireviewer-spatial](https://github.com/fireviewer/fireviewer-spatial) | Deterministic map packages, observed temporal layers, provenance, and spatial validation. |
| [fireviewer-sdg](https://github.com/fireviewer/fireviewer-sdg) | Synthetic-data and simulation research, kept separate from real-event evidence. |
| [FireViewer on Hugging Face](https://huggingface.co/fireviewer) | Authoritative public model and dataset cards, revisions, weights, and hosted artifacts. |

Some implementation repositories are currently private. They are described in
the [repository guide](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/public/REPOSITORIES.md)
without being presented as publicly accessible.

## Data and safety

FireViewer keeps source tickets, hashes, derived claims, evidence revisions,
review decisions, and failure outcomes. The acquisition pipeline is not a
shadow archive: scraped articles, copied public media, and full transcripts are
not retained by default. User media requires explicit authorisation for each
relevant use.

Observation, reconstruction, simulation, and prediction are distinct result
types. A model output is derived evidence, not a source, coordinate authority,
or publication decision.

## Current maturity

FireViewer is an active research MVP. Core contracts and several integration
paths exist, but the complete real-data flow has not been qualified as an
unattended production service. Optional paid GPU stages are not assumed active,
and publication remains guarded. The dated, evidence-based boundary is in the
[current status](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/public/STATUS.md).

## Contribute or contact

Contributions to software, accessibility, mapping, provenance, data governance,
testing, and research validation are welcome. Do not use GitHub to report an
emergency or request assistance.

For research, infrastructure, security, provenance, rights, or data-removal
enquiries, contact **unicornwhodev@gmail.com**.
