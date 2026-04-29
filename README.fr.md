# OpenClaw Coding Skills

[![Skills](https://img.shields.io/badge/Skills-13-blue?style=for-the-badge)](./skills/INDEX.md)
[![Références](https://img.shields.io/badge/Références_dexécution-21-green?style=for-the-badge)](./skills/)
[![Échantillons](https://img.shields.io/badge/Échantillons_éval-39-orange?style=for-the-badge)](./evaluation/)
[![Règles](https://img.shields.io/badge/Règles_de_déclenchement-131-purple?style=for-the-badge)](./skills/TRIGGER-MATRIX.md)
[![Licence](https://img.shields.io/badge/Licence-MIT-brightgreen?style=for-the-badge)](./LICENSE)
[![Powered by MyClaw.ai](https://img.shields.io/badge/Powered%20by-MyClaw.ai-ff6b35?style=for-the-badge)](https://myclaw.ai)

**Arrêtez d'espérer que l'agent va réussir. Faites du comportement de codage fiable le comportement par défaut.**

[English](./README.md) · [中文](./README.zh-CN.md) · [Deutsch](./README.de.md) · [Español](./README.es.md) · [Italiano](./README.it.md) · [日本語](./README.ja.md) · [Русский](./README.ru.md)

---

### En un coup d'œil

| Couche | Contenu | Nombre |
|--------|---------|--------|
| **Skills de flux de travail** | `spec` → `plan` → `build` → `test` → `review` → `ship` | 7 |
| **Skills spécialisés** | `debug` · `security` · `frontend` · `docs` · `deploy` · `refactor` | 6 |
| **Références d'exécution** | Aide à la décision réutilisable dans les skills à haut risque | 21 fichiers |
| **Matrice de déclenchement** | Correspondance requête→skill avec guidage des cas limites | 131 règles |
| **Assets d'évaluation** | Échantillons labellisés, cas ambigus, validation dry-run & live | 39 échantillons sur 6 ensembles de données |
| **Infrastructure de tuning** | Playbook, schéma de résultat, boucle de feedback, journal de tuning | Boucle fermée complète |

> **70+ fichiers · 13 skills · 21 références d'exécution · 39 échantillons d'évaluation · 131 règles de déclenchement**

---

Skills de codage de qualité production pour les agents OpenClaw.

Parte du écosystème [MyClaw.ai](https://myclaw.ai) : un ensemble croissant d'assets open source conçus pour transformer la capacité brute de l'agent en exécution logicielle fiable.

## À propos de MyClaw.ai

[MyClaw.ai](https://myclaw.ai) est une plateforme d'assistant IA qui donne à chaque utilisateur un serveur complet exécutant [OpenClaw](https://github.com/openclaw/openclaw) — le framework d'agent IA open source leader. Chaque instance MyClaw offre un contrôle code complet, un accès réseau, des outils et la possibilité d'installer des skills comme celui-ci.

Dans l'écosystème MyClaw.ai, ce dépôt sert de **couche de comportement de codage** : il comble le fossé entre « le modèle peut écrire du code » et « l'agent peut exécuter un travail logiciel avec discipline ». Les utilisateurs MyClaw peuvent installer ces skills directement dans leur instance pour améliorer instantanément la qualité de leurs sessions de codage.

L'écosystème open source MyClaw.ai comprend également :

- **[openclaw-coding-skills](https://github.com/LeoYeAI/openclaw-coding-skills)** — Système de comportement de codage structuré (ce dépôt)
- **[openclaw-guardian](https://github.com/LeoYeAI/openclaw-guardian)** — Surveillance et protection de sécurité
- **[openclaw-auto-dream](https://github.com/LeoYeAI/openclaw-auto-dream)** — Consolidation de mémoire cognitive
- **[myclaw-backup](https://github.com/LeoYeAI/myclaw-backup)** — Sauvegarde et restauration complètes d'instance
- **[myclaw-bench](https://github.com/LeoYeAI/myclaw-bench)** — Référentiel des capacités des agents

Tout est open source. Tout est conçu pour le même objectif : rendre les agents IA plus fiables et plus utiles dans le travail réel.

---

Ce projet ne rend pas « le modèle plus intelligent », mais « l'agent plus mature dans les vraies tâches de codage ». Il utilise des workflow skills, des skills spécialisés, des références d'exécution, une correspondance de déclenchement, des échantillons d'évaluation et des boucles de tuning pour transformer un comportement de codage qui dérive facilement en un système d'exécution plus stable, plus vérifiable et plus réutilisable.

## Ce que ce projet fournit

- Workflow skills : `spec`, `plan`, `build`, `test`, `review`, `ship`
- Skills spécialisés : `debug`, `security`, `frontend`, `docs`, `deploy`, `refactor`
- `references/` — Références d'exécution : aident l'agent à moins deviner et moins se tromper aux points de décision critiques
- `TRIGGER-MATRIX` : Améliore le taux de déclenchement automatique et la clarté des cas limites
- `examples/` : Échantillons de requêtes réalistes pour calibrer la qualité du déclenchement
- `evaluation/` : Ensembles d'évaluation labellisés, échantillons ambigus, validation dry-run, validation live, boucle de tuning

En un mot : ce n'est pas un prompt unique ni un ensemble disparate de skills, c'est un système d'optimisation comportementale construit autour de vrais workflow de codage.

## Valeur centrale

Il n'améliore pas les poids du modèle, mais la qualité du comportement de codage.

De nombreux agents échouent en développement logiciel non pas parce qu'ils ne peuvent pas écrire du code, mais parce que leur mode d'exécution n'est pas assez mature : périmètre non défini avant de commencer, modifications trop grandes, preuves trop faibles, review et test mélangées, tâches à haut risque sans structure suffisante.

La valeur de ce projet est de réduire systématiquement ces modes d'échec :

- Définir le périmètre avant de coder
- Avancer par petites étapes au lieu de tout faire d'un coup
- Exiger des preuves suffisantes avant de se déclarer terminé
- Traiter de manière structurée debug, sécurité, déploiement et refactoring comme des scénarios à haut risque
- Optimiser en continu grâce aux échantillons, à l'évaluation et à la validation live

## Pour qui

- Les équipes qui veulent des résultats de codage plus stables avec OpenClaw
- Les équipes qui souhaitent ancrer les standards d'ingénierie sous forme de skills réutilisables
- Les équipes qui veulent tuner le comportement de l'agent en continu — pas seulement ajuster les prompts

## Points d'entrée

- Documentation principale anglaise : [README.md](./README.md)
- Guide d'installation : [INSTALL.md](./INSTALL.md)
- Guide d'adoption : [ADOPTION-GUIDE.md](./ADOPTION-GUIDE.md)
- Correspondance de déclenchement : [skills/TRIGGER-MATRIX.md](./skills/TRIGGER-MATRIX.md)
- Exemples de tâches : [examples/README.md](./examples/README.md)
- Évaluation et tuning : [evaluation/README.md](./evaluation/README.md)