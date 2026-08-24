# SPEC-PRD-001 — Smoke health

| Campo | Valor |
|--------|--------|
| ID | SPEC-PRD-001 |
| Versión | 0.1.0 |
| Estado | Approved |
| Fecha | 2026-08-24 |
| Fuentes | `knowledge/raw/2026-08-24-smoke-seed.md`, `handbook/03-mvp-definition.md` |
| ADRs relacionados | N/A (sin decisión de stack) |
| Backlog | PBI-001 |
| Derivados | `specs/acceptance/SPEC-ACC-001-smoke-health.md`, worklog PBI-001 |

## Contexto

Validar que un consumidor de `sdaf-core` puede tener una spec Approved enlazada a backlog y acceptance.

## Alcance

Documentar la capacidad smoke «health»: el producto declara que el estado de salud lógico es OK cuando Gate 0 está cerrado para PBI-001.

## Criterios de aceptación

Ver [SPEC-ACC-001](../acceptance/SPEC-ACC-001-smoke-health.md).

## Fuera de alcance

Implementación en `src/`, endpoints HTTP, UI.

## Historial

| Versión | Fecha | Cambio |
|---------|--------|--------|
| 0.1.0 | 2026-08-24 | Approved para smoke de adopción |
