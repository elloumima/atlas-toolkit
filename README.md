**Langues :** **Français** · [English](README.en.md)

# ATLAS Toolkit

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/elloumima/atlas-toolkit?style=social)](https://github.com/elloumima/atlas-toolkit)
[![Contributors](https://img.shields.io/github/contributors/elloumima/atlas-toolkit)](https://github.com/elloumima/atlas-toolkit/graphs/contributors)

> **Open-source patterns, tools and examples for legacy modernization** — COBOL, Delphi, BizTalk to cloud-native stacks.

Maintenu par [Access International](https://access-international.dev), une ESN tunisienne qui modernise du code legacy depuis 1999. Ce toolkit capture les patterns répétables que nous avons identifiés en livrant plus de 10 POC de migration (35 524 lignes converties).

## Pourquoi ce toolkit

La modernisation legacy est un chantier stratégique pour des milliers d'entreprises (banques, assurances, secteur public, industrie). Pourtant, chaque programme réinvente la roue. Pas de catalogue partagé, peu de patterns documentés en open source, aucun outillage commun pour prouver la parité fonctionnelle.

**ATLAS Toolkit ouvre nos patterns**. Pas toute la méthodologie (qui reste propriétaire), mais les briques techniques réutilisables : patterns de traduction, test de parité, scaffolds de migration, règles de discordances.

## Contenu

### `/patterns`

Patterns de traduction documentés, avec exemple source → cible + tests de parité.

| Source | Cible | Pattern | Fichier |
|---|---|---|---|
| COBOL | TypeScript | PERFORM loops → forEach/for-of | [`patterns/cobol/perform-loops.md`](patterns/cobol/perform-loops.md) |
| COBOL | Java | EVALUATE → switch/case | À venir |
| COBOL | TypeScript | File I/O indexed → Map | À venir |
| Delphi | TypeScript | TStringList → Array | À venir |
| BizTalk | Azure Logic Apps | Orchestration XLANG → workflow.json | À venir |

### `/tools`

Petits outils de ligne de commande pour automatiser les tâches répétitives.

| Outil | But |
|---|---|
| `parity-tester` | Compare run legacy vs run cible, identifie les discordances |
| `discrepancy-registry` | Génère un registre signable de discordances |
| `cobol-splitter` | Découpe un programme COBOL monolithe en modules traductibles |

### `/examples`

Exemples complets fonctionnels — pas des stubs.

- [`examples/card-demo-cobol/`](examples/card-demo-cobol/) : application CARDDEMO (IBM sample) migrée COBOL → TypeScript Cloudflare Worker
- Autres à venir

### `/docs`

- [`docs/philosophy.md`](docs/philosophy.md) — pourquoi on documente ces patterns
- [`docs/contributing-guide.md`](docs/contributing-guide.md) — comment proposer un nouveau pattern
- [`docs/atlas-methodology-intro.md`](docs/atlas-methodology-intro.md) — aperçu de la méthodologie complète (intro, sans les détails propriétaires)

## Quickstart

```bash
# Cloner
git clone https://github.com/elloumima/atlas-toolkit.git
cd atlas-toolkit

# Installer deps pour les outils
cd tools/parity-tester && npm install

# Lancer un exemple
cd ../../examples/card-demo-cobol && npm install && npm test
```

## Contribuer

Les contributions sont **bienvenues et encouragées**. Pattern de migration trouvé qui fonctionne ? Outil utile pour comparer des runs ? Exemple pédagogique ?

Voir [`CONTRIBUTING.md`](CONTRIBUTING.md) pour le process détaillé.

**Bon premiers tickets** :
- [Issues avec label `good first issue`](https://github.com/elloumima/atlas-toolkit/labels/good%20first%20issue)

## Qui utilise ce toolkit

- [Access International](https://access-international.dev) (maintainer)
- *Ajoutez votre entreprise via PR — on aime savoir*

## Stack cibles supportées

- **TypeScript** (Cloudflare Workers, Node.js, Deno)
- **Java 21** (Spring Boot)
- **.NET 8** (ASP.NET Core)
- **Python** (FastAPI, Polars pour batch)
- **Azure Logic Apps** (pour orchestrations BizTalk)

## Licence

MIT. Vous pouvez utiliser les patterns et outils dans vos projets commerciaux, sans attribution obligatoire mais appréciée.

## Liens

- Site : [access-international.dev](https://access-international.dev)
- Méthodologie complète : [access-international.dev/fr/methodologie-atlas](https://access-international.dev/fr/methodologie-atlas)
- Contact : [access-international.dev/fr/contact](https://access-international.dev/fr/contact)
- Twitter/X : [@accessint](https://twitter.com/accessint) *(placeholder)*

---

*"Le legacy qui fait tourner les banques, les assurances et les administrations n'est pas un problème à cacher — c'est un patrimoine à moderniser avec méthode."*
