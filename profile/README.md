# FireViewer

**Open-source infrastructure for documented wildfire observation, spatial
reconstruction, temporal tracking, and reproducible post-event study.**

FireViewer is an independent research and engineering project maintained by
**Unicorn Who Dev**. It connects sources, observations, provenance, automated
analysis, and human review so that uncertainty remains visible and an event can
be studied again without turning a hypothesis into a fact.

> FireViewer is not an alert service, an official source, a command tool, or a
> certified wildfire-propagation predictor. In an emergency, follow the
> guidance of the relevant authorities and emergency services.

## What the project is building

```text
sources + documented observations
              ↓
provenance + evidence
              ↓
automated analysis / explicit abstention
              ↓
human review
              ↓
reproducible spatial map build + reviewed temporal states
              ↓
public exploration and post-event studies
```

The canonical mapping pipeline is headless and endpoint-driven. It remains
separate from visualisation layers, simulation, and any prediction. Observations,
reconstructions, interpolations, simulations, and predictions are never treated
as the same kind of result.

## Public repositories

| Repository | Public role |
| --- | --- |
| [Fireviewer_doc](https://github.com/fireviewer/Fireviewer_doc) | Canonical documentation: scope, architecture, security, status, contracts, and roadmap. |
| [models](https://github.com/fireviewer/models) | Lightweight public registry of resources visible on Hugging Face; no weights, caches, or datasets are copied into it. |
| [fireviewer-frontend](https://github.com/fireviewer/fireviewer-frontend) | Contribution, human review, and public event exploration. |
| [fireviewer-backend](https://github.com/fireviewer/fireviewer-backend) | Incident registry, evidence, audit, orchestration, and publication. |
| [fireviewer-ai-worker](https://github.com/fireviewer/fireviewer-ai-worker) | Private analysis, visual anchors, localisation attempts, and abstention. |
| [fireviewer-spatial](https://github.com/fireviewer/fireviewer-spatial) | Spatial maps, geographic packages, and temporal layers. |
| [fireviewer-sdg](https://github.com/fireviewer/fireviewer-sdg) | Separate research on synthetic data and simulation. |

Model cards, published weights, and dataset cards on
[Hugging Face](https://huggingface.co/fireviewer) are authoritative. The GitHub
registry documents only what is publicly verifiable at a given time; it does not
present a resource as deployed, qualified, or operational by default.

## Public documentation and local working material

GitHub contains material intended to explain, contribute to, and verify the
project: canonical documentation, contracts, code, and portable guides. Working
notes, machine paths, raw logs, unqualified results, provider configuration,
private evidence, and exports remain local and are never copied into public
repositories.

The complete rule is in the
[documentation policy](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/REPOSITORY_DOCUMENTATION_POLICY.md).

## Status and contribution

The project is under development. The presence of code, a model, or a local test
does not prove deployment, geographic accuracy, or scientific qualification.
Contributions to code, testing, accessibility, mapping, provenance, and
evaluation are welcome.

Do not use GitHub to report an emergency or request assistance.

## Links

- [Project documentation](https://github.com/fireviewer/Fireviewer_doc)
- [Public model and dataset registry](https://github.com/fireviewer/models)
- [Hugging Face organisation](https://huggingface.co/fireviewer)
- Research, infrastructure, security, provenance, or data-removal contact:
  **unicornwhodev@gmail.com**
