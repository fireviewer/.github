# FireViewer

**Préserver, reconstruire et étudier les incendies de végétation à partir de sources vérifiables.**

FireViewer est un MVP de recherche actif, né des travaux autour de l’incendie de Die. Le projet rassemble sources officielles, images autorisées, satellite et données géographiques pour conserver la chronologie et le contexte spatial d’un événement.

> **observé ≠ reconstruit ≠ simulé ≠ prédit**

FireViewer ne prédit pas la propagation future. Il n’est ni un service d’alerte, ni une source officielle de sécurité civile, ni un outil de commandement. Une détection n’est pas une coordonnée géographique ; les résultats IA sensibles restent soumis à validation humaine.

## Comprendre le projet

- [Présentation en une page](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/public/presentations/PRESENTATION_1_PAGE.md).
- [Partenaires et financeurs](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/public/presentations/PRESENTATION_PARTENAIRES_FINANCEURS.md).
- [Architecture et responsabilités](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/public/ARCHITECTURE.md).
- [État du projet et limites de réception](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/public/STATUS.md).

## Architecture et maturité

Collecte et normalisation → preuves versionnées → vision et hypothèses géographiques → recoupement → calcul Fire State/Part.4 → revue humaine → publication dans l’atlas 2D/3D.

Le backend conserve incidents, droits, preuves durables, révisions et décisions. Le Map Builder générique UWD fournit séparément des packages géographiques : une carte mesurée n’est pas une observation incendie. Les terrains suivent leur réception technique propre. L’atlas et ses cartes existent ; leur présence ne qualifie pas tous les nouveaux parcours de bout en bout.

La simulation reste un chantier distinct en attente. Unreal n’est pas une dépendance à introduire dans le site web. Le worker historique reste transitoire ; les nouveaux algorithmes appartiennent aux composants spécialisés.

## Dépôts et ressources

L’[inventaire GitHub du 19 septembre 2026](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/public/ORGANISATION.md) comprend **18 dépôts** : 16 dépôts cœur, institutionnels, infrastructure ou transition et 2 auxiliaires Android (gestion associative et atelier d’annotation). Le producteur UWD reste externe. Les sources applicatives sont privées ; le profil et la documentation sont publics.

[Hugging Face](https://huggingface.co/fireviewer) héberge les modèles, corpus et cartes versionnés. Le [catalogue public documenté](https://github.com/fireviewer/Fireviewer_doc/blob/main/docs/public/HUGGINGFACE.md) distingue 5 modèles et 4 datasets, avec des niveaux de maturité différents. Publication, licence, résultat de benchmark et promotion runtime sont des questions séparées.

## Gouvernance et soutien

L’association française FIRE-VIEWER assure l’administration et la gestion des ressources qu’elle contrôle. Le développement technique est actuellement assuré principalement par un mainteneur. Les actifs antérieurs et les composants UWD restent soumis à leurs licences ou conventions ; le placement d’un dépôt ne transfère pas les droits.

Les contributions en données, géomatique, recherche, validation, accessibilité, calcul et financement sont utiles. Un soutien ne donne aucune autorité sur les preuves ou les résultats.

[Contribution](https://github.com/fireviewer/.github/blob/main/CONTRIBUTING.md) · [Gouvernance](https://github.com/fireviewer/Fireviewer_doc/blob/main/GOVERNANCE.md) · [Code de conduite](https://github.com/fireviewer/.github/blob/main/CODE_OF_CONDUCT.md) · [Sécurité](https://github.com/fireviewer/.github/blob/main/SECURITY.md) · [Support](https://github.com/fireviewer/.github/blob/main/SUPPORT.md).

**Site institutionnel : [fire-viewer.fr](https://fire-viewer.fr)**
**Contact : contact@fire-viewer.fr**

Revue documentaire : 19 septembre 2026. Aucun nouveau test fonctionnel n’est revendiqué par cette actualisation.
