# AGENTS.md — Router de agentes SdafAdoptionSmoke

| Campo | Valor |
|--------|--------|
| Versión | 0.1.0 |
| Estado | Approved |
| Fecha | 2026-08-24 |
| Norma | `sdaf-core/handbook/13-ai-agent-framework.md`, `sdaf-core/handbook/14-prompt-engineering-standard.md`, `sdaf-core/handbook/15-agent-traceability.md`, `sdaf-core/skills/README.md` |
| Config | `sdaf.config.yaml` |
| Core | submodule `sdaf-core` @ `v0.1.0` |

---

## Propósito

Índice operativo para invocar agentes de **ingeniería** en este smoke de adopción.
Antes de cualquier feature: Gate 0 (`sdaf-core/handbook/09-development-workflow.md`).

## Modelo

| Estado | Agentes |
|--------|---------|
| **Activo** | Specification, Architecture, Testing+Review |
| **Stub** | Product, Domain, Application, DevOps, Review, Testing |

## Handoff canónico

```text
Specification → Architecture → (implementación del consumidor)
                                      ↘ Testing+Review ↗
```

En este smoke **no** hay implementación de producto; el objetivo es validar Gate 0 y el cableado del core.

## Inventario

Contratos y prompts viven en el submodule:

| Agente | Contrato | Prompt | Estado |
|--------|----------|--------|--------|
| Specification | [sdaf-core/agents/specification-agent.md](sdaf-core/agents/specification-agent.md) | [sdaf-core/prompts/agents/specification-agent.md](sdaf-core/prompts/agents/specification-agent.md) | active |
| Architecture | [sdaf-core/agents/architecture-agent.md](sdaf-core/agents/architecture-agent.md) | [sdaf-core/prompts/agents/architecture-agent.md](sdaf-core/prompts/agents/architecture-agent.md) | active |
| Testing+Review | [sdaf-core/agents/testing-review-agent.md](sdaf-core/agents/testing-review-agent.md) | [sdaf-core/prompts/agents/testing-review-agent.md](sdaf-core/prompts/agents/testing-review-agent.md) | active |
| Product | [sdaf-core/agents/product-agent.md](sdaf-core/agents/product-agent.md) | [sdaf-core/prompts/agents/product-agent.md](sdaf-core/prompts/agents/product-agent.md) | stub |
| Domain | [sdaf-core/agents/domain-agent.md](sdaf-core/agents/domain-agent.md) | [sdaf-core/prompts/agents/domain-agent.md](sdaf-core/prompts/agents/domain-agent.md) | stub |
| Application | [sdaf-core/agents/application-agent.md](sdaf-core/agents/application-agent.md) | [sdaf-core/prompts/agents/application-agent.md](sdaf-core/prompts/agents/application-agent.md) | stub |
| DevOps | [sdaf-core/agents/devops-agent.md](sdaf-core/agents/devops-agent.md) | [sdaf-core/prompts/agents/devops-agent.md](sdaf-core/prompts/agents/devops-agent.md) | stub |
| Review | [sdaf-core/agents/review-agent.md](sdaf-core/agents/review-agent.md) | [sdaf-core/prompts/agents/review-agent.md](sdaf-core/prompts/agents/review-agent.md) | stub |
| Testing | [sdaf-core/agents/testing-agent.md](sdaf-core/agents/testing-agent.md) | [sdaf-core/prompts/agents/testing-agent.md](sdaf-core/prompts/agents/testing-agent.md) | stub |

## Skills

Playbooks en [`sdaf-core/skills/`](sdaf-core/skills/). Citar `skill-id@version` en worklogs.

| Prioridad | Skills (core) |
|-----------|----------------|
| Alta | `sdaf-gate0`, `sdaf-worklog-handoff`, `sdaf-agent-router` |
| Media | `spec-draft-pbi`, `adr-propose` |

## Gobernanza

- Prompt de sistema: [sdaf-core/prompts/system/master-architect.md](sdaf-core/prompts/system/master-architect.md)
- Worklogs: `worklogs/` (este repo)
- Idioma: castellano (`sdaf-core/.cursor/rules/idioma-castellano.mdc`)

## Restricciones globales

Ningún agente: aprueba handbook/specs por sí solo; salta Gate 0; implementa alcance Out del MVP; introduce secretos; reescribe historia git sin orden humana.
