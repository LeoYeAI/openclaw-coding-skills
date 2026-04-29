# OpenClaw Coding Skills

[![Skills](https://img.shields.io/badge/Competenze-13-blue?style=for-the-badge)](./skills/INDEX.md)
[![Riferimenti](https://img.shields.io/badge/Riferimenti_esecuzione-21-green?style=for-the-badge)](./skills/)
[![Campioni eval](https://img.shields.io/badge/Campioni_eval-39-orange?style=for-the-badge)](./evaluation/)
[![Regole trigger](https://img.shields.io/badge/Regole_trigger-131-purple?style=for-the-badge)](./skills/TRIGGER-MATRIX.md)
[![Licenza](https://img.shields.io/badge/Licenza-MIT-brightgreen?style=for-the-badge)](./LICENSE)
[![Powered by MyClaw.ai](https://img.shields.io/badge/Powered%20by-MyClaw.ai-ff6b35?style=for-the-badge)](https://myclaw.ai)

**Smetti di sperare che l'agente faccia la cosa giusta. Rendi il comportamento di codifica affidabile lo standard.**

[English](./README.md) · [中文](./README.zh-CN.md) · [Deutsch](./README.de.md) · [Français](./README.fr.md) · [Español](./README.es.md) · [Italiano](./README.it.md) · [日本語](./README.ja.md) · [Русский](./README.ru.md)

---

### A colpo d'occhio

| Livello | Contenuto | Quantità |
|---------|-----------|----------|
| **Skill di workflow** | `spec` → `plan` → `build` → `test` → `review` → `ship` | 7 |
| **Skill specialistiche** | `debug` · `security` · `frontend` · `docs` · `deploy` · `refactor` | 6 |
| **Riferimenti di esecuzione** | Supporto decisionale riutilizzabile nelle skill ad alto rischio | 21 file |
| **Matrice dei trigger** | Mappatura richiesta→skill con guida per i casi limite | 131 regole |
| **Asset di valutazione** | Campioni etichettati, casi ambigui, validazione dry-run e live | 39 campioni su 6 dataset |
| **Infrastruttura di tuning** | Playbook, schema risultati, ciclo di feedback, log di tuning | Ciclo chiuso completo |

> **70+ file · 13 skill · 21 riferimenti di esecuzione · 39 campioni di valutazione · 131 regole trigger**

---

Skill di codifica di livello produzione per agenti OpenClaw.

Parte dell'ecosistema [MyClaw.ai](https://myclaw.ai): un insieme crescente di asset aperti progettati per trasformare le capacità grezze dell'agente in un'esecuzione software affidabile.

## Informazioni su MyClaw.ai

[MyClaw.ai](https://myclaw.ai) è una piattaforma di assistente IA che fornisce a ogni utente un server completo con [OpenClaw](https://github.com/openclaw/openclaw) — il principale framework open-source per agenti IA. Ogni istanza MyClaw offre controllo completo del codice, accesso alla rete, strumenti e la possibilità di installare skill come questa direttamente.

All'interno dell'ecosistema MyClaw.ai, questo repository funge da **livello di comportamento di codifica**: colma il divario tra "il modello può scrivere codice" e "l'agente può eseguire lavoro software con disciplina". Gli utenti MyClaw possono installare queste skill direttamente nella loro istanza per migliorare istantaneamente la qualità delle sessioni di codifica.

L'ecosistema open source MyClaw.ai include anche:

- **[openclaw-coding-skills](https://github.com/LeoYeAI/openclaw-coding-skills)** — Sistema strutturato di comportamento di codifica (questo repo)
- **[openclaw-guardian](https://github.com/LeoYeAI/openclaw-guardian)** — Monitoraggio e protezione della sicurezza
- **[openclaw-auto-dream](https://github.com/LeoYeAI/openclaw-auto-dream)** — Consolidamento della memoria cognitiva
- **[myclaw-backup](https://github.com/LeoYeAI/myclaw-backup)** — Backup e ripristino completo dell'istanza
- **[myclaw-bench](https://github.com/LeoYeAI/myclaw-bench)** — Benchmark delle capacità dell'agente

Tutto open source. Tutto progettato per lo stesso obiettivo: rendere gli agenti IA più affidabili e più utili nel lavoro reale.

---

Questo progetto non rende "il modello più intelligente", ma "l'agente più maturo nei compiti di codifica reali". Utilizza skill di workflow, skill specialistiche, riferimenti di esecuzione, mappatura dei trigger, campioni di valutazione e cicli di tuning per trasformare un comportamento di codifica che tende a deviare in un sistema di esecuzione più stabile, verificabile e riutilizzabile.

## Cosa fornisce questo progetto

- Skill di workflow: `spec`, `plan`, `build`, `test`, `review`, `ship`
- Skill specialistiche: `debug`, `security`, `frontend`, `docs`, `deploy`, `refactor`
- `references/` — Riferimenti di esecuzione: aiutano l'agente a indovinare meno e sbagliare meno nei punti decisionali critici
- `TRIGGER-MATRIX`: Migliora il tasso di successo del trigger automatico e la chiarezza dei casi limite
- `examples/`: Campioni di richieste realistiche per calibrare la qualità del trigger
- `evaluation/`: Set di valutazione etichettati, campioni ambigui, validazione dry-run, validazione live, ciclo di tuning

In sintesi: non è un singolo prompt né una raccolta sparsa di skill, ma un sistema di ottimizzazione comportamentale costruito attorno a flussi di lavoro di codifica reali.

## Valore centrale

Non migliora i pesi del modello, ma la qualità del comportamento di codifica.

Molti agenti falliscono nello sviluppo software non perché non sanno scrivere codice, ma perché il loro modo di esecuzione non è abbastanza maturo: ambito non definito prima di iniziare, modifiche troppo grandi, prove troppo deboli, review e test mescolati, compiti ad alto rischio senza struttura sufficiente.

Il valore di questo progetto è ridurre sistematicamente questi pattern di fallimento:

- Prima definire l'ambito, poi programmare
- Avanzare a piccoli passi invece di fare tutto in una volta
- Richiedere prove sufficienti prima di dichiarare il completamento
- Trattare in modo strutturato debug, sicurezza, deployment e refactoring come scenari ad alto rischio
- Ottimizzare continuamente attraverso campioni, valutazione e validazione live

## Per chi

- Team che vogliono risultati di codifica più stabili con OpenClaw
- Team che vogliono consolidare gli standard ingegneristici come skill riutilizzabili
- Team che vogliono ottimizzare il comportamento dell'agente in modo continuo — non solo aggiustare i prompt

## Punti di accesso

- Documentazione principale in inglese: [README.md](./README.md)
- Guida all'installazione: [INSTALL.md](./INSTALL.md)
- Guida all'adozione: [ADOPTION-GUIDE.md](./ADOPTION-GUIDE.md)
- Mappatura dei trigger: [skills/TRIGGER-MATRIX.md](./skills/TRIGGER-MATRIX.md)
- Esempi di attività: [examples/README.md](./examples/README.md)
- Valutazione e tuning: [evaluation/README.md](./evaluation/README.md)
