# Security policy — BornToBeFound

## Versions supportées

| Version | Support |
| --- | --- |
| `0.1.x` | Corrections de sécurité |
| `< 0.1` | Non supportée |

Le projet est un projet annuel ESGI ; il n'est pas destiné à traiter des
données personnelles réelles.

## Signaler une vulnérabilité

**Ne jamais créer d'issue publique.** Utiliser les _GitHub Security Advisories_
du dépôt concerné :

- <https://github.com/born2tofound/btbf-front/security/advisories/new>
- <https://github.com/born2tofound/btbf-api/security/advisories/new>
- <https://github.com/born2tofound/btbf-platform/security/advisories/new>

Inclure si possible : version/commit, environnement, étapes de reproduction,
impact, preuve (log, capture) et correctif suggéré.

## Périmètre

Sont considérés comme critiques :

- fuite de secret (clé, token, mot de passe, chaîne de connexion) ;
- accès non autorisé à MongoDB ou à l'API ;
- injection (NoSQL, commande, template) ;
- exposition de données personnelles ou de fichiers `.env` ;
- contournement de la validation Pydantic ou des server actions ;
- dépendance vulnérable connue.

## Règles pour les contributeurs

- Jamais de secret en clair dans le code, un commit, une issue ou une capture.
- Un secret poussé est **compromis** : le révoquer, pas seulement le supprimer.
- Les dépendances suivent les correctifs ; Dependabot ouvre les PR.
- Les logs ne contiennent ni token ni donnée personnelle.

## Divulgation

Nous accusons réception sous 72 h ouvrées et coordonnons une divulgation
responsable après correctif. Merci de ne pas publier de détail exploitable avant
accord.
