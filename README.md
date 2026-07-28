 FireViewer

**Cartographie 3D, chronologique et incidente-centrique pour mieux comprendre les incendies.**

FireViewer est un projet open source qui rassemble des données ouvertes, des observations documentées, des contributions citoyennes et des analyses automatisées supervisées afin de produire une représentation visuelle, datée et sourcée d’un incendie.

Le principe central est simple : **un incendie correspond à une page publique persistante**. Cette page peut évoluer au fil des observations validées, afficher plusieurs niveaux de détail 3D et conserver la mémoire de l’événement après sa clôture.

> FireViewer est un projet de développement et de recherche. Ce n’est ni un service d’alerte, ni une source officielle, ni un outil de conduite des secours. Il ne remplace jamais les consignes des autorités et services d’urgence.

## Principes

- **Open source** : le code, les contrats, les outils de préparation et les pipelines sont publiés dans des dépôts publics.
- **Incident-centrique** : une identité stable relie les observations, épisodes, modèles et mises à jour d’un même incendie.
- **État daté** : chaque information est rattachée à une date, une provenance et un niveau de confiance.
- **Incertitudes visibles** : l’absence de preuve ou une localisation incertaine doit rester explicite.
- **Revue humaine** : les analyses automatisées ne sont pas présentées comme des faits établis sans validation.
- **Aucune prédiction opérationnelle** : FireViewer ne prédit pas la propagation et ne fournit pas de consignes à la population ou aux équipes de secours.

## Dépôts publics

| Dépôt | Rôle |
| --- | --- |
| [`fireviewer-frontend`](https://github.com/fireviewer/fireviewer-frontend) | Site public, espace d’administration, consultation incidente-centrique et viewer 3D. |
| [`fireviewer-backend`](https://github.com/fireviewer/fireviewer-backend) | API, registre des incidents, rattachement des observations, validation, audit et publication. |
| [`fireviewer-ai-worker`](https://github.com/fireviewer/fireviewer-ai-worker) | Analyse factuelle de médias, orchestration des modèles, contrats de sortie et mécanismes d’abstention. |
| [`fireviewer-spatial`](https://github.com/fireviewer/fireviewer-spatial) | Préparation des packages spatiaux, LiDAR, orthophotos, Blender, Unity et contrats de catalogue. |
| [`fireviewer-sdg`](https://github.com/fireviewer/fireviewer-sdg) | Génération de corpus synthétiques avec NVIDIA Omniverse et Isaac Sim, real-to-sim, sim-to-real et contrôle de provenance. |

## Fonctionnement général

1. Des sources ouvertes et des contributions documentées sont collectées.
2. Les médias, textes et métadonnées sont analysés et recoupés.
3. Des faits, repères et zones peuvent être proposés avec leur niveau d’incertitude.
4. Une revue humaine accepte, corrige, rattache ou rejette les propositions.
5. La page publique de l’incident est mise à jour avec un état daté et traçable.
6. Une fois l’événement terminé, la page reste disponible comme archive chronologique.

## État du projet

FireViewer est en développement actif. Les dépôts contiennent le socle technique, les contrats, les tests et les outils de production, mais leur présence ne signifie pas que le système est certifié ou déployé comme service opérationnel de sécurité civile.

Les modèles, jeux de données, cartes de modèles, cartes de datasets et résultats d’évaluation sont publiés progressivement sur l’organisation Hugging Face :

**https://huggingface.co/fireviewer**

## Contribuer

Les issues et pull requests sont bienvenues lorsqu’elles concernent le code, la documentation, les tests, l’accessibilité, la qualité des données, la cartographie, la 3D ou l’évaluation des modèles.

GitHub ne doit pas être utilisé pour signaler une urgence ou transmettre une demande de secours. En situation réelle, contactez les services d’urgence compétents et suivez les canaux officiels.

## Licences et données externes

Chaque dépôt précise sa licence. Les données IGN, OpenStreetMap, Copernicus, NASA, EFFIS, médias, contributions et autres ressources externes conservent leurs licences, conditions de réutilisation et règles de citation propres.

---

- GitHub : https://github.com/fireviewer
- Hugging Face : https://huggingface.co/fireviewer
