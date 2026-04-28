# OpenClaw Coding Skills

[![Skills](https://img.shields.io/badge/Skills-13-blue?style=for-the-badge)](./skills/INDEX.md)
[![Referenzen](https://img.shields.io/badge/Ausf%C3%BChrungsreferenzen-21-green?style=for-the-badge)](./skills/)
[![Eval-Stichproben](https://img.shields.io/badge/Eval--Stichproben-39-orange?style=for-the-badge)](./evaluation/)
[![Trigger-Regeln](https://img.shields.io/badge/Trigger--Regeln-131-purple?style=for-the-badge)](./skills/TRIGGER-MATRIX.md)
[![Lizenz](https://img.shields.io/badge/Lizenz-MIT-brightgreen?style=for-the-badge)](./LICENSE)
[![Powered by MyClaw.ai](https://img.shields.io/badge/Powered%20by-MyClaw.ai-ff6b35?style=for-the-badge)](https://myclaw.ai)

**Hör auf zu hoffen, dass der Agent es richtig macht. Mach zuverlässiges Coding-Verhalten zum Standard.**

[English](./README.md) · [中文](./README.zh-CN.md) · [Deutsch](./README.de.md)

---

### Auf einen Blick

| Schicht | Inhalt | Anzahl |
|---------|--------|--------|
| **Workflow-Skills** | `spec` → `plan` → `build` → `test` → `review` → `ship` | 7 |
| **Spezialisten-Skills** | `debug` · `security` · `frontend` · `docs` · `deploy` · `refactor` | 6 |
| **Ausführungsreferenzen** | Wiederverwendbare Entscheidungshilfen in risikoreichen Skills | 21 Dateien |
| **Trigger-Matrix** | Anfrage→Skill-Zuordnung mit Grenzfallführung | 131 Regeln |
| **Evaluierungs-Assets** | Gelabelte Stichproben, Mehrdeutigkeitsfälle, Dry-Run & Live-Validierung | 39 Stichproben über 6 Datensätze |
| **Tuning-Infrastruktur** | Playbook, Ergebnis-Schema, Feedback-Schleife, Tuning-Log | Vollständiger Kreislauf |

> **70+ Dateien · 13 Skills · 21 Ausführungsreferenzen · 39 Eval-Stichproben · 131 Trigger-Regeln**

---

Produktionsreife Coding-Skills für OpenClaw-Agents.

Teil des [MyClaw.ai](https://myclaw.ai)-Ökosystems: eine wachsende Sammlung offener Assets, die darauf ausgelegt sind, rohe Agent-Fähigkeiten in zuverlässige Software-Ausführung zu verwandeln.

## Über MyClaw.ai

[MyClaw.ai](https://myclaw.ai) ist eine KI-Assistenzplattform, die jedem Nutzer einen vollständigen Server mit [OpenClaw](https://github.com/openclaw/openclaw) bereitstellt — dem führenden Open-Source-KI-Agent-Framework. Jede MyClaw-Instanz bietet vollständige Code-Kontrolle, Netzwerkzugang, Tool-Zugriff und die Möglichkeit, Skills wie diesen direkt zu installieren.

Innerhalb des MyClaw.ai-Ökosystems dient dieses Repository als **Coding-Verhaltensschicht**: Es schließt die Lücke zwischen „das Modell kann Code schreiben" und „der Agent kann Softwarearbeit mit Disziplin ausführen." MyClaw-Nutzer können diese Skills direkt in ihre Instanz installieren und sofort die Qualität ihrer Coding-Sessions verbessern.

Das offene MyClaw.ai-Ökosystem umfasst außerdem:

- **[openclaw-coding-skills](https://github.com/LeoYeAI/openclaw-coding-skills)** — Strukturiertes Coding-Verhaltenssystem (dieses Repo)
- **[openclaw-guardian](https://github.com/LeoYeAI/openclaw-guardian)** — Sicherheitsüberwachung und Schutz
- **[openclaw-auto-dream](https://github.com/LeoYeAI/openclaw-auto-dream)** — Kognitive Gedächtniskonsolidierung
- **[myclaw-backup](https://github.com/LeoYeAI/myclaw-backup)** — Vollständige Instanz-Sicherung und Wiederherstellung
- **[myclaw-bench](https://github.com/LeoYeAI/myclaw-bench)** — Agent-Fähigkeits-Benchmarking

Alles Open Source. Alles für dasselbe Ziel: KI-Agents in der echten Arbeit zuverlässiger und nützlicher zu machen.

---

Dieses Projekt macht nicht „das Modell schlauer", sondern „den Agent in echten Coding-Aufgaben reifer". Es nutzt Workflow-Skills, Spezialisten-Skills, Ausführungsreferenzen, Trigger-Zuordnung, Evaluierungs-Stichproben und Tuning-Schleifen, um das leicht abdriftende Coding-Verhalten in ein stabileres, überprüfbareres und wiederverwendbares Ausführungssystem zu verwandeln.

## Was dieses Projekt bietet

- Workflow-Skills: `spec`, `plan`, `build`, `test`, `review`, `ship`
- Spezialisten-Skills: `debug`, `security`, `frontend`, `docs`, `deploy`, `refactor`
- `references/`-Ausführungsreferenzen: Helfen dem Agent, an kritischen Entscheidungspunkten weniger zu raten und weniger Fehlurteile zu fällen
- `TRIGGER-MATRIX`: Verbessert die automatische Trigger-Trefferquote und Grenzfall-Klarheit
- `examples/`: Realistische Anfrage-Stichproben zur Kalibrierung der Trigger-Qualität
- `evaluation/`: Gelabelte Evaluierungssätze, Mehrdeutigkeits-Stichproben, Dry-Run-Validierung, Live-Validierung, Tuning-Kreislauf

Anders gesagt: Es ist kein einzelner Prompt und keine lose Sammlung von Skills, sondern ein systematisches Verhaltensoptimierungssystem, das um echte Coding-Workflows herum aufgebaut ist.

## Kernwert

Es verbessert nicht die Modellgewichte, sondern die Coding-Verhaltensqualität.

Viele Agents scheitern in der Softwareentwicklung nicht, weil sie keinen Code schreiben können, sondern weil ihre Ausführungsweise nicht ausgereift genug ist: Umfang nicht klar definiert bevor sie loslegen, Änderungen zu groß, Nachweise zu schwach, Review und Test vermischt, risikoreiche Aufgaben ohne ausreichende Struktur.

Der Wert dieses Projekts liegt darin, diese Fehlermuster systematisch zu reduzieren:

- Erst den Umfang definieren, dann programmieren
- In kleinen Schritten vorgehen, statt alles auf einmal
- Vor der Fertigmeldung ausreichende Nachweise verlangen
- Debug, Sicherheit, Deployment und Refactoring als Hochrisiko-Szenarien strukturiert behandeln
- Durch Stichproben, Evaluierung und Live-Validierung kontinuierlich optimieren

## Für wen

- Teams, die stabilere Coding-Ergebnisse von OpenClaw wollen
- Teams, die Engineering-Standards als wiederverwendbare Skills festhalten möchten
- Teams, die Agent-Verhalten kontinuierlich tunen wollen — nicht nur Prompts anpassen

## Einstieg

- Englische Hauptdokumentation: [README.md](./README.md)
- Installationsanleitung: [INSTALL.md](./INSTALL.md)
- Adoptionsleitfaden: [ADOPTION-GUIDE.md](./ADOPTION-GUIDE.md)
- Trigger-Zuordnung: [skills/TRIGGER-MATRIX.md](./skills/TRIGGER-MATRIX.md)
- Beispielaufgaben: [examples/README.md](./examples/README.md)
- Evaluierung und Tuning: [evaluation/README.md](./evaluation/README.md)
