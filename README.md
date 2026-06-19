# Trip Planner

Outil de planification d'itinéraires de voyage sous forme de page web statique, déployée via **GitHub Pages**.

## Principe

Chaque itinéraire est conçu et codé directement dans [index.html](index.html), le fichier servi par GitHub Pages. Pas de build, pas de dépendances — une seule page HTML auto-suffisante.

## Itinéraire actuel : Vietnam — 1 mois

Trois variantes d'un voyage d'un mois au Vietnam, axées plein air, paysages et gastronomie locale :

| Itinéraire | Trajet | Meilleure saison |
|---|---|---|
| 1 — Du nord au centre | Hanoï → Sapa → Ha Long → Hội An → Phong Nha → Hué | Oct – Fév |
| 2 — Centre & Sud | Da Nang → Phong Nha → Dalat → Mũi Né → HCMV → Phú Quốc | Nov – Août |
| 3 — Le Vietnam complet | Hanoï → Ninh Bình → Ha Long → Hội An → Phong Nha → Dalat → Phú Quốc | Oct – Fév |

## Modifier ou créer un itinéraire

Éditer directement `index.html` :

- **En-tête** — titre et sous-titre dans `<header>`
- **Onglets** — boutons dans `.tabs` (un `.tab-btn` par itinéraire)
- **Étapes** — blocs `.stop` dans chaque `.itinerary` (nom, durée, description, tags)
- **Barre de résumé** — `.total-bar` en bas de chaque itinéraire

Pour ajouter un nouvel itinéraire, dupliquer un bloc `<div class="itinerary itN">`, incrémenter l'indice, et ajouter le bouton correspondant dans `.tabs`.

## Déploiement (GitHub Pages)

1. Pousser les modifications sur la branche `main`
2. Dans les paramètres du dépôt → **Pages** → Source : `main` / `/ (root)`
3. GitHub Pages sert automatiquement `index.html` à la racine

La page est accessible à l'adresse : `https://<utilisateur>.github.io/<nom-du-dépôt>/`
