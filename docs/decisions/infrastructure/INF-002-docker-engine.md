# INF-002 — Contenedores del Proyecto

## Estado

Aprobada

## Fecha

2026-07-21

## Direccionamiento

El proyecto va a utilizar `Docker Engine` instalado directamente dentro de `Ubuntu 20.04 LTS` sobre `WSL2`.

## Alternativas consideradas

- `Docker Desktop`.
- Podman.
- Containerd sin `Docker`.

## Motivo

`Docker` se puede instalar de manera muy ligera, integrada por completo en `Linux` y evita depender de `Docker Desktop` para `Windows`. Asimismo, simplifica el uso de `Ollama`, `Open WebUI` y `NVIDIA Container Toolkit`.

## Consecuencias

Todos los servicios del proyceto (`Ollama`, `Open WebUI`, `ChromaDB` y futuros microservicios) se van a desplegar por medio de `Docker Compose` utilizando `Docker Engine` como runtime.