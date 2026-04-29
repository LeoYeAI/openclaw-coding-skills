# OpenClaw Coding Skills

[![Skills](https://img.shields.io/badge/Habilidades-13-blue?style=for-the-badge)](./skills/INDEX.md)
[![Referencias](https://img.shields.io/badge/Referencias_de_ejecución-21-green?style=for-the-badge)](./skills/)
[![Muestras](https://img.shields.io/badge/Muestras_eval-39-orange?style=for-the-badge)](./evaluation/)
[![Reglas](https://img.shields.io/badge/Reglas_de_disparo-131-purple?style=for-the-badge)](./skills/TRIGGER-MATRIX.md)
[![Licencia](https://img.shields.io/badge/Licencia-MIT-brightgreen?style=for-the-badge)](./LICENSE)
[![Powered by MyClaw.ai](https://img.shields.io/badge/Powered%20by-MyClaw.ai-ff6b35?style=for-the-badge)](https://myclaw.ai)

**Deja de esperar que el agente lo haga bien. Haz del comportamiento de codificación confiable el padrão por defecto.**

[English](./README.md) · [中文](./README.zh-CN.md) · [Deutsch](./README.de.md) · [Français](./README.fr.md) · [Italiano](./README.it.md) · [日本語](./README.ja.md) · [Русский](./README.ru.md)

---

### De un vistazo

| Capa | Contenido | Cantidad |
|------|-----------|----------|
| **Habilidades de flujo de trabajo** | `spec` → `plan` → `build` → `test` → `review` → `ship` | 7 |
| **Habilidades especializadas** | `debug` · `security` · `frontend` · `docs` · `deploy` · `refactor` | 6 |
| **Referencias de ejecución** | Soporte de decisión reutilizable en habilidades de alto riesgo | 21 archivos |
| **Matriz de disparadores** | Correspondencia solicitud→habilidad con guía de casos límite | 131 reglas |
| **Assets de evaluación** | Muestras etiquetadas, casos ambiguos, validación dry-run y live | 39 muestras en 6 conjuntos de datos |
| **Infraestructura de tuning** | Playbook, esquema de resultados, bucle de feedback, log de tuning | Bucle cerrado completo |

> **70+ archivos · 13 habilidades · 21 referencias de ejecución · 39 muestras de evaluación · 131 reglas de disparo**

---

Habilidades de codificación de nivel de producción para agentes OpenClaw.

Parte del ecosistema [MyClaw.ai](https://myclaw.ai): un conjunto creciente de assets abiertos diseñados para transformar la capacidad bruta del agente en ejecución de software confiable.

## Sobre MyClaw.ai

[MyClaw.ai](https://myclaw.ai) es una plataforma de asistente de IA que le da a cada usuario un servidor completo ejecutando [OpenClaw](https://github.com/openclaw/openclaw) — el principal framework de agente de IA de código abierto. Cada instancia de MyClaw ofrece control de código completo, acceso a la red, herramientas y la capacidad de instalar habilidades como esta directamente.

Dentro del ecosistema MyClaw.ai, este repositorio sirve como la **capa de comportamiento de codificación**: cierra la brecha entre "el modelo puede escribir código" y "el agente puede ejecutar trabajo de software con disciplina". Los usuarios de MyClaw pueden instalar estas habilidades directamente en su instancia para mejorar instantáneamente la calidad de sus sesiones de codificación.

El ecosistema de código abierto MyClaw.ai también incluye:

- **[openclaw-coding-skills](https://github.com/LeoYeAI/openclaw-coding-skills)** — Sistema de comportamiento de codificación estructurado (este repositorio)
- **[openclaw-guardian](https://github.com/LeoYeAI/openclaw-guardian)** — Supervisión y protección de seguridad
- **[openclaw-auto-dream](https://github.com/LeoYeAI/openclaw-auto-dream)** — Consolidación de memoria cognitiva
- **[myclaw-backup](https://github.com/LeoYeAI/myclaw-backup)** — Copia de seguridad y restauración completa de instancia
- **[myclaw-bench](https://github.com/LeoYeAI/myclaw-bench)** — Referencia de capacidad del agente

Todo es de código abierto. Todo está diseñado para el mismo objetivo: hacer que los agentes de IA sean más confiables y más útiles en el trabajo real.

---

Este proyecto no hace "el modelo más inteligente", sino "el agente más maduro en tareas reales de codificación". Utiliza habilidades de flujo de trabajo, habilidades especializadas, referencias de ejecución, correspondencia de disparadores, muestras de evaluación y bucles de tuning para transformar un comportamiento de codificación que tiende a derivar en un sistema de ejecución más estable, más verificable y más reutilizable.

## Lo que este proyecto proporciona

- Habilidades de flujo de trabajo: `spec`, `plan`, `build`, `test`, `review`, `ship`
- Habilidades especializadas: `debug`, `security`, `frontend`, `docs`, `deploy`, `refactor`
- `references/` — Referencias de ejecución: ayudan al agente a adivinar menos y cometer menos errores en los puntos de decisión críticos
- `TRIGGER-MATRIX`: Mejora la tasa de acierto de disparo automático y la claridad de los casos límite
- `examples/`: Muestras de solicitudes realistas para calibrar la calidad del disparo
- `evaluation/`: Conjuntos de evaluación etiquetados, muestras ambiguas, validación dry-run, validación live, bucle de tuning

En resumen: no es un prompt único ni una colección dispersa de habilidades, es un sistema de optimización comportamental construido en torno a flujos de trabajo reales de codificación.

## Valor central

No mejora los pesos del modelo, sino la calidad del comportamiento de codificación.

Muchos agentes fallan en el desarrollo de software no porque no puedan escribir código, sino porque su modo de ejecución no es suficientemente maduro: alcance no definido antes de comenzar, cambios demasiado grandes, evidencias demasiado débiles, review y test mezcladas, tareas de alto riesgo sin estructura suficiente.

El valor de este proyecto es reducir sistemáticamente estos patrones de fallo:

- Definir primero el alcance, luego programar
- Avanzar en pasos pequeños en lugar de hacerlo todo de una vez
- Exigir evidencias suficientes antes de declarar finalización
- Tratar de forma estructurada debug, seguridad, despliegue y refactoring como escenarios de alto riesgo
- Optimizar continuamente a través de muestras, evaluación y validación live

## Para quién

- Equipos que desean resultados de codificación más estables con OpenClaw
- Equipos que desean institucionalizar estándares de ingeniería como habilidades reutilizables
- Equipos que desean ajustar el comportamiento del agente continuamente — no solo ajustar prompts

## Puntos de entrada

- Documentación principal en inglés: [README.md](./README.md)
- Guía de instalación: [INSTALL.md](./INSTALL.md)
- Guía de adopción: [ADOPTION-GUIDE.md](./ADOPTION-GUIDE.md)
- Correspondencia de disparadores: [skills/TRIGGER-MATRIX.md](./skills/TRIGGER-MATRIX.md)
- Ejemplos de tareas: [examples/README.md](./examples/README.md)
- Evaluación y tuning: [evaluation/README.md](./evaluation/README.md)