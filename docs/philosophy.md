# Philosophie d'ATLAS Toolkit

## Le problème

Des milliers d'entreprises (banques, assurances, secteur public, industrie, télécoms) portent des applications COBOL, Delphi, BizTalk en production depuis 20-40 ans. Elles tournent, elles font tourner le business, mais :

- Les développeurs qui les maintiennent partent en retraite
- La documentation est incomplète ou perdue
- Les règles métier sont enfouies dans le code
- Moderniser coûte cher et fait peur

**Résultat** : chaque programme de modernisation réinvente tout. Aucun pattern partagé, aucun outil commun, pas de catalogue des pièges déjà rencontrés.

## Notre conviction

**La modernisation legacy est un métier d'ingénieur, pas d'aventurier**. Les patterns existent, ils se répètent. Les erreurs sont souvent les mêmes. Les vérifications aussi.

Chez Access International, on modernise du COBOL et du Delphi depuis 1999. On a livré 10 POC récemment (2024-2026) couvrant 8 stacks COBOL, 1 Delphi, 1 BizTalk, pour un total de ~35 524 lignes converties vers TypeScript/Java/.NET.

On a décidé d'ouvrir **les briques réutilisables** — patterns, outils de parité, scaffolds d'exemple — sous licence MIT.

## Ce qu'on ouvre

- ✅ Patterns de traduction (source → cible) avec tests
- ✅ Outils de comparaison (parity-tester)
- ✅ Exemples publics (IBM samples, open datasets)
- ✅ Scaffolds d'exemples
- ✅ Vocabulaire et références

## Ce qu'on n'ouvre pas

- ❌ Les 10 étapes ATLAS détaillées (méthodologie complète)
- ❌ Les 9 principes directeurs
- ❌ Les 49 learnings de retour d'expérience
- ❌ Le code de nos clients (confidentialité)
- ❌ Les templates de registre de discordances (format propriétaire)

**Pourquoi cette frontière** : la valeur d'ATLAS n'est pas dans les patterns techniques (qui existent ailleurs). Elle est dans l'agencement méthodologique + la discipline opérationnelle. On partage les briques, on monétise l'agencement.

## Ce qu'on attend de la communauté

### Ce qui aide

- Signaler des bugs dans les patterns
- Proposer de nouveaux patterns (surtout Delphi, BizTalk, PowerBuilder — stacks mal documentées)
- Porter un exemple sur une autre stack cible (Python, Go, Rust)
- Traduire les patterns FR ↔ EN

### Ce qui n'est pas la bonne porte

- Aide gratuite sur votre programme de migration commercial — contactez-nous sur [access-international.dev/fr/contact](https://access-international.dev/fr/contact)
- Documentation générale sur COBOL (voir IBM docs, wikipedia)
- Cours de programmation (voir freeCodeCamp, codecademy)

## Inspirations

- [Strangler Fig pattern](https://martinfowler.com/bliki/StranglerFigApplication.html) de Martin Fowler
- [Kubernetes community model](https://github.com/kubernetes/community) pour l'organisation OSS
- [Pattern JDK](https://openjdk.org) pour le ton technique
- [Refactoring Guru](https://refactoring.guru) pour la pédagogie

## Gouvernance

ATLAS Toolkit est maintenu par Access International. Décisions éditoriales (quelles contributions acceptées, quels patterns inclus) par l'équipe Access. Licence MIT garantit la libre utilisation.

Si le projet grandit, création d'un comité steering avec contributeurs externes (après 10+ contributeurs actifs).

## Contact

- Site : [access-international.dev](https://access-international.dev)
- Email : `hello@access-international.dev`
- Issues : [github.com/elloumima/atlas-toolkit/issues](https://github.com/elloumima/atlas-toolkit/issues)
