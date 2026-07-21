# INF-003 — Uso de NVIDIA Container Toolkit

## Estado

Aprobada

## Fecha

2026-07-21

## Direccionamiento

Los contenedores del proyecto van a utilizar GPU acelerado mediante NVIDIA Container Toolkit sobre Docker Engine.

## Alternativas consideradas

- `Docker` solo con CPU.
- `Docker Desktop` para `Windows`.
- Ejecución nativa sin contenedores.

## Motivo

Se requiere que los modelos de lenguaje utilicen la GPU `RTX 5060 Ti` desde contenedores `Linux` ejecutados sobre `WSL2`, manteniendo un entorno reproducible y aislado.

## Consecuencias

- `Ollama` va a usar la `GPU` desde `Docker`.
- `Open WebUI` podrá comunicarse con Ollama sin depender del host Windows.
- El entorno va a ser portable hacia otros servidores Linux con cambios apenas perceptibles.