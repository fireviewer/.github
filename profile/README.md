# FireViewer

**Infrastructure open source pour l’observation documentée des incendies, la
reconstruction spatiale, le suivi temporel et l’étude reproductible après
événement.**

FireViewer est un projet indépendant de recherche et d’ingénierie maintenu par
**Unicorn Who Dev**. Il relie les sources, les observations, leur provenance,
des analyses automatisées et une revue humaine afin que l’incertitude reste
visible et qu’un événement puisse être réétudié sans transformer une hypothèse
en fait.

> FireViewer n’est ni un service d’alerte, ni une source officielle, ni un outil
> de commandement, ni un prédicteur certifié de propagation. En cas d’urgence,
> suivre les autorités et services compétents.

## Ce que le projet construit

```text
sources + observations documentées
              ↓
provenance + éléments de preuve
              ↓
analyse automatisée / abstention explicite
              ↓
revue humaine
              ↓
carte spatiale reproductible + états temporels revus
              ↓
exploration publique et études après événement
```

La chaîne de cartographie canonique est sans interface et pilotée par endpoints.
Elle reste distincte des couches de visualisation, de la simulation et de toute
prédiction. Les observations, reconstructions, interpolations, simulations et
prédictions ne sont jamais confondues.

## Dépôts publics

| Dépôt | Rôle public |
| --- | --- |
| [Fireviewer_doc](https://github.com/fireviewer/Fireviewer_doc) | Documentation canonique : périmètre, architecture, sécurité, statut, contrats et feuille de route. |
| [models](https://github.com/fireviewer/models) | Registre public léger des ressources visibles sur Hugging Face ; aucun poids, cache ou dataset n’y est copié. |
| [fireviewer-frontend](https://github.com/fireviewer/fireviewer-frontend) | Contribution, revue humaine et exploration publique des événements. |
| [fireviewer-backend](https://github.com/fireviewer/fireviewer-backend) | Registre d’incidents, preuves, audit, orchestration et publication. |
| [fireviewer-ai-worker](https://github.com/fireviewer/fireviewer-ai-worker) | Analyse privée, repères visuels, tentatives de localisation et abstention. |
| [fireviewer-spatial](https://github.com/fireviewer/fireviewer-spatial) | Cartes spatiales, paquets géographiques et couches temporelles. |
| [fireviewer-sdg](https://github.com/fireviewer/fireviewer-sdg) | Recherche séparée sur données synthétiques et simulation. |

Les cartes de modèles, les poids publiés et les cartes de datasets font autorité
sur [Hugging Face](https://huggingface.co/fireviewer). Le registre GitHub
documente seulement ce qui est publiquement vérifiable à une date donnée ; il ne
présente pas une ressource comme déployée, qualifiée ou opérationnelle par défaut.

## Documentation publique et travail local

GitHub contient les documents destinés à comprendre, contribuer et vérifier le
projet : documentation canonique, contrats, code et guides portables. Les notes
de travail, chemins de machines, journaux bruts, résultats non qualifiés,
configurations de fournisseurs, preuves privées et exports restent locaux et ne
sont jamais copiés dans les dépôts publics.

La règle complète est dans la
[politique de documentation](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/REPOSITORY_DOCUMENTATION_POLICY.md).

## État et contribution

Le projet est en développement. Une présence de code, de modèle ou de test local
ne vaut pas preuve de déploiement, de précision géographique ou de qualification
scientifique. Les contributions sur le code, les tests, l’accessibilité, la
cartographie, la provenance et l’évaluation sont bienvenues.

Ne pas utiliser GitHub pour signaler une urgence ou demander des secours.

## Liens

- [Documentation du projet](https://github.com/fireviewer/Fireviewer_doc)
- [Registre public des modèles et datasets](https://github.com/fireviewer/models)
- [Organisation Hugging Face](https://huggingface.co/fireviewer)
- Contact recherche, infrastructure, sécurité, provenance ou retrait de données : **unicornwhodev@gmail.com**
