# INF-001 — Plataforma base del servidor

## Estado 

Aprobada

## Fecha

2026-07-20

## Direccionamiento

El backend del proyecto se va a ejecutar sobre `WSL2` usando `Ubuntu 24.04 LTS`.

## Alternativas consideradas

- `Windows` nativo.
- `Ubuntu 22.04 LTS`.
- `Ubuntu 26.04 LTS`.

## Motivo

Se prioriza estabilidad y compatibilidad con `Docker Engine`, `Ollama`, `NVIDIA Container Toolkit` y el ecosistema de `IA` por sobre utilizar una entrega de mayor actualidad del sistema operativo.

## Consecuencias

La infraestructura del backend en su totalidad (`Docker`, `Ollama`,`Python`, `Open WebUI` y servicios relacionados) se va a instalar dentro de `Ubuntu` sobre `WSL2`.