<div align="center">

# BornToBeFound

**Chaque candidat laisse une trace. Nous la rendons lisible.**

Plateforme OSINT de _background check_ pour le recrutement, complétée par une
Threat Intelligence qui émet des alertes.

[Projet annuel ESGI 2026](https://www.esgi.fr/) · Toulouse

[**Démo live →**](https://btbf.cleeryy.cloud) · [**Wiki →**](https://github.com/born2tofound/wiki/wiki)

</div>

---

## Le produit

BornToBeFound reconstitue le dossier public d'un candidat à partir de sources
ouvertes : collecte, recoupement, datation, puis **revue humaine signée**. Le
score n'est jamais une décision : il ouvre une conversation, avec ses sources.

Le volet Threat Intelligence surveille des indicateurs et émet des alertes
reliées aux investigations en cours.

## Les dépôts

| Dépôt | Rôle | Stack |
| --- | --- | --- |
| [`btbf-front`](https://github.com/born2tofound/btbf-front) | Vitrine et console d'investigation | Next.js 16, TypeScript, Tailwind v4, shadcn/ui, beUI |
| [`btbf-api`](https://github.com/born2tofound/btbf-api) | API, domaine et persistance | FastAPI, Python 3.13, MongoDB |
| [`btbf-platform`](https://github.com/born2tofound/btbf-platform) | Orchestration : submodules, Compose, déploiement | Docker, GHCR, Dokploy |
| [`wiki`](https://github.com/born2tofound/wiki/wiki) | Documentation vivante : architecture, API, front, déploiement, sécurité, contribution | GitHub Wiki |

## Principes

- **Sources ouvertes uniquement.** Pas d'accès privé, pas de contournement.
- **Revue humaine.** Aucune décision automatisée sur un candidat.
- **Traçabilité.** Chaque conclusion cite ses sources et sa date.
- **Vie privée.** Droit de réponse, suppression, journal d'audit.
- **Démonstration honnête.** Les données de la démo sont fictives.

## Stack

```text
Next.js 16 ── HTTP ── FastAPI ── MongoDB
     │                    │
     └── Docker ── GHCR ──┘
              Dokploy
```

## Équipe

| Rôle | GitHub |
| --- | --- |
| Chef de projet, architecture et revue | [@MalikIssiakhem](https://github.com/MalikIssiakhem) |
| Front-end, i18n et déploiement | [@cleeryy](https://github.com/cleeryy) |
| Contributeurs | [@hackerswa](https://github.com/hackerswa) · [@PigeonOccitan98](https://github.com/PigeonOccitan98) |

## Travailler ici

La méthode commune (branches, commits conventionnels, PR, revue) est décrite
dans [`CONTRIBUTING.md`](https://github.com/born2tofound/.github/blob/main/CONTRIBUTING.md).
Chaque dépôt ajoute ses commandes dans son `README.md`.

Suivi du MVP : [Project 1 — Todo BTBF](https://github.com/orgs/born2tofound/projects/1).

## Sécurité

Ne jamais ouvrir d'issue publique pour une vulnérabilité. Voir
[`SECURITY.md`](https://github.com/born2tofound/.github/blob/main/SECURITY.md).
