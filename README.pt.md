# OpenClaw Coding Skills

[![Skills](https://img.shields.io/badge/Skills-13-blue?style=for-the-badge)](./skills/INDEX.md)
[![Referências](https://img.shields.io/badge/Referências_de_execução-21-green?style=for-the-badge)](./skills/)
[![Amostras](https://img.shields.io/badge/Amostras_eval-39-orange?style=for-the-badge)](./evaluation/)
[![Regras](https://img.shields.io/badge/Regras_de_gatilho-131-purple?style=for-the-badge)](./skills/TRIGGER-MATRIX.md)
[![Licença](https://img.shields.io/badge/Licença-MIT-brightgreen?style=for-the-badge)](./LICENSE)
[![Powered by MyClaw.ai](https://img.shields.io/badge/Powered%20by-MyClaw.ai-ff6b35?style=for-the-badge)](https://myclaw.ai)

**Pare de esperar que o agente acerte. Faça do comportamento de codificação confiável o padrão.**

[English](./README.md) · [中文](./README.zh-CN.md) · [Deutsch](./README.de.md) · [Français](./README.fr.md) · [Español](./README.es.md) · [Italiano](./README.it.md) · [日本語](./README.ja.md) · [Русский](./README.ru.md)

---

### Em um relance

| Camada | Conteúdo | Quantidade |
|--------|----------|------------|
| **Skills de fluxo de trabalho** | `spec` → `plan` → `build` → `test` → `review` → `ship` | 7 |
| **Skills especializados** | `debug` · `security` · `frontend` · `docs` · `deploy` · `refactor` | 6 |
| **Referências de execução** | Suporte à decisão reutilizável em skills de alto risco | 21 arquivos |
| **Matriz de gatilhos** | Mapeamento solicitação→skill com orientação de limites | 131 regras |
| **Assets de avaliação** | Amostras etiquetadas, casos ambíguos, validação dry-run & live | 39 amostras em 6 conjuntos de dados |
| **Infraestrutura de tuning** | Playbook, esquema de resultado, loop de feedback, log de tuning | Loop fechado completo |

> **70+ arquivos · 13 skills · 21 referências de execução · 39 amostras de avaliação · 131 regras de gatilho**

---

Skills de codificação de nível de produção para agentes OpenClaw.

Parte do ecossistema [MyClaw.ai](https://myclaw.ai): um conjunto crescente de assets abertos projetados para transformar capacidade bruta de agente em execução de software confiável.

## Sobre o MyClaw.ai

[MyClaw.ai](https://myclaw.ai) é uma plataforma de assistente de IA que oferece a cada usuário um servidor completo executando [OpenClaw](https://github.com/openclaw/openclaw) — o principal framework de agente de IA open source. Cada instância MyClaw oferece controle de código completo, acesso à rede, ferramentas e a capacidade de instalar skills como esta diretamente.

Dentro do ecossistema MyClaw.ai, este repositório serve como a **camada de comportamento de codificação**: ele preenche a lacuna entre "o modelo pode escrever código" e "o agente pode executar trabalho de software com disciplina". Usuários MyClaw podem instalar esses skills diretamente em sua instância para melhorar instantaneamente a qualidade das sessões de codificação.

O ecossistema open source MyClaw.ai também inclui:

- **[openclaw-coding-skills](https://github.com/LeoYeAI/openclaw-coding-skills)** — Sistema de comportamento de codificação estruturado (este repositório)
- **[openclaw-guardian](https://github.com/LeoYeAI/openclaw-guardian)** — Monitoramento e proteção de segurança
- **[openclaw-auto-dream](https://github.com/LeoYeAI/openclaw-auto-dream)** — Consolidação de memória cognitiva
- **[myclaw-backup](https://github.com/LeoYeAI/myclaw-backup)** — Backup e restauração completos de instância
- **[myclaw-bench](https://github.com/LeoYeAI/myclaw-bench)** — Referencial de capacidade do agente

Tudo open source. Tudo projetado para o mesmo objetivo: tornar agentes de IA mais confiáveis e mais úteis no trabalho real.

---

Este projeto não torna "o modelo mais inteligente", mas "o agente mais maduro em tarefas reais de codificação". Ele usa workflow skills, skills especializados, referências de execução, mapeamento de gatilhos, amostras de avaliação e loops de tuning para transformar comportamento de codificação que tende a dériva em um sistema de execução mais estável, mais verificável e mais reutilizável.

## O que este projeto fornece

- Workflow skills: `spec`, `plan`, `build`, `test`, `review`, `ship`
- Skills especializados: `debug`, `security`, `frontend`, `docs`, `deploy`, `refactor`
- `references/` — Referências de execução: ajudam o agente a adivinhar menos e errar menos nos pontos de decisão críticos
- `TRIGGER-MATRIX`: Melhora a taxa de acerto de gatilho automático e a clareza dos casos limite
- `examples/`: Amostras de solicitações realistas para calibrar a qualidade do gatilho
- `evaluation/`: Conjuntos de avaliação etiquetados, amostras ambíguas, validação dry-run, validação live, loop de tuning

Resumindo: não é um prompt único nem uma coleção solta de skills, é um sistema de otimização comportamental construído em torno de fluxos de trabalho reais de codificação.

## Valor central

Ele não melhora os pesos do modelo, mas a qualidade do comportamento de codificação.

Muitos agentes falham no desenvolvimento de software não porque não conseguem escrever código, mas porque seu modo de execução não é suficientemente maduro: escopo não definido antes de começar, mudanças muito grandes, evidências muito fracas, review e teste misturados, tarefas de alto risco sem estrutura suficiente.

O valor deste projeto é reduzir sistematicamente esses padrões de falha:

- Definir primeiro o escopo, depois codificar
- Avançar em passos pequenos em vez de fazer tudo de uma vez
- Exigir evidências suficientes antes de declarar conclusão
- Tratar de forma estruturada debug, segurança, deployment e refactoring como cenários de alto risco
- Otimizar continuamente através de amostras, avaliação e validação live

## Para quem

- Equipes que desejam resultados de codificação mais estáveis com o OpenClaw
- Equipes que desejam institucionalizar padrões de engenharia como skills reutilizáveis
- Equipes que desejam ajustar o comportamento do agente continuamente — não apenas ajustar prompts

## Pontos de entrada

- Documentação principal em inglês: [README.md](./README.md)
- Guia de instalação: [INSTALL.md](./INSTALL.md)
- Guia de adoção: [ADOPTION-GUIDE.md](./ADOPTION-GUIDE.md)
- Mapeamento de gatilhos: [skills/TRIGGER-MATRIX.md](./skills/TRIGGER-MATRIX.md)
- Exemplos de tarefas: [examples/README.md](./examples/README.md)
- Avaliação e tuning: [evaluation/README.md](./evaluation/README.md)