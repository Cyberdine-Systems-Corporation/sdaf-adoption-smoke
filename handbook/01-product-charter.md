# 01 — Product Charter (smoke)

| Campo | Valor |
|--------|--------|
| Versión | 0.1.0 |
| Estado | Approved |
| Fecha | 2026-08-24 |

## Propósito

Definir el producto **SdafAdoptionSmoke**: vehículo mínimo para validar la adopción de `sdaf-core`, no un SaaS real.

## Problema

Hace falta un repo consumidor de referencia que ejercite Gate 0 y el cableado del núcleo sin arrastrar dominio de negocio.

## Alcance In

- Documentar adopción (submodule, config, AGENTS.md).
- Una capacidad smoke Approved con acceptance y PBI.
- Cerrar Gate 0 **sin** escribir código de producto.

## Alcance Out

- UI, API, base de datos, auth, IA de producto.
- Packs de stack (`sdaf-stack-*`).
- Implementación en `src/`.

## Éxito

Un humano o agente puede clonar este repo, inicializar el submodule y verificar Gate 0 del PBI-001 con evidencias en rutas.
