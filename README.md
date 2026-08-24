# SDAF Adoption Smoke

Repo de **prueba de adopción** de [`sdaf-core@v0.1.0`](https://github.com/Cyberdine-Systems-Corporation/sdaf-core/releases/tag/v0.1.0).

No es un producto real. Sirve para validar que un consumidor puede:

1. Referenciar el core (submodule en `sdaf-core/`).
2. Declarar `sdaf.config.yaml`.
3. Materializar `AGENTS.md`.
4. Tener handbook de producto + `knowledge/` / `specs/` / `backlog/` / `worklogs/`.
5. Cerrar **Gate 0** para un PBI trivial (sin implementar código).

## Estructura

| Ruta | Rol |
|------|-----|
| `sdaf-core/` | Submodule pinneado a `v0.1.0` |
| `sdaf.config.yaml` | Escenario default-core del método |
| `AGENTS.md` | Router materializado |
| `handbook/` | Constitución de **producto** (smoke) |
| `knowledge/`, `specs/`, `architecture/`, `backlog/`, `worklogs/` | Artefactos SDAF del consumidor |
| `src/`, `tests/` | Vacíos a propósito (sin implementación) |

## Cómo clonar

```powershell
git clone --recurse-submodules https://github.com/Cyberdine-Systems-Corporation/sdaf-adoption-smoke.git
cd sdaf-adoption-smoke
```

Si ya clonaste sin submodules:

```powershell
git submodule update --init --recursive
```

## Gate 0 (smoke)

PBI: [backlog/PBI-001-smoke-health.md](backlog/PBI-001-smoke-health.md)  
Spec: [specs/product/SPEC-PRD-001-smoke-health.md](specs/product/SPEC-PRD-001-smoke-health.md) (Approved)  
Acceptance: [specs/acceptance/SPEC-ACC-001-smoke-health.md](specs/acceptance/SPEC-ACC-001-smoke-health.md)  
ADR: N/A (justificado en worklog; no toca stack/límites)  
Worklog: [worklogs/PBI-001-smoke-health/Iteration-001.md](worklogs/PBI-001-smoke-health/Iteration-001.md)

Verificar con la skill del core: `sdaf-core/skills/sdaf-gate0/SKILL.md`.

## Norma

Método: submodule `sdaf-core` (handbook Approved).  
Producto: este `handbook/` (smoke).
