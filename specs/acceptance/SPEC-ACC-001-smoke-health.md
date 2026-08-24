# SPEC-ACC-001 — Smoke health

| Campo | Valor |
|--------|--------|
| ID | SPEC-ACC-001 |
| Versión | 0.1.0 |
| Estado | Approved |
| Fecha | 2026-08-24 |
| Fuentes | SPEC-PRD-001 |
| Backlog | PBI-001 |

## Criterios de aceptación

### Dado / Cuando / Entonces

```text
Dado el repo sdaf-adoption-smoke con submodule sdaf-core@v0.1.0
Cuando un revisor aplica sdaf-gate0 al PBI-001
Entonces G0.1–G0.5 están evidencias por ruta y el gate puede declararse cerrado sin código en src/
```

```text
Dado SPEC-PRD-001 y SPEC-ACC-001 Approved
Cuando se consulta el backlog PBI-001
Entonces el PBI enlaza ambas specs y declara Out de implementación
```

## Historial

| Versión | Fecha | Cambio |
|---------|--------|--------|
| 0.1.0 | 2026-08-24 | Approved |
