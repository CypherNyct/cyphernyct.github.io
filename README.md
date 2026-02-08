# cyphernyct.github.io

Blog personal de ciberseguridad: writeups, apuntes, cheatsheets y más.

## Cómo añadir un nuevo post

1. Crea un archivo `.md` en la carpeta `_posts/`
2. El nombre del archivo debe seguir el formato: `YYYY-MM-DD-titulo.md`
3. Añade el front matter al inicio del archivo (ver ejemplos existentes)
4. Haz commit y push

### Ejemplo de front matter para writeup:

```yaml
---
layout: post
title: "Nombre de la máquina"
date: 2026-02-08
category: writeups
platform: DockerLabs
difficulty: Fácil
tags: [tag1, tag2, tag3]
---
```

### Categorías disponibles:
- `writeups` — Resolución de máquinas CTF
- `apuntes` — Notas de estudio
- `cheatsheets` — Referencias rápidas
- `tutoriales` — Guías paso a paso
- `blog` — Posts personales

### Plataformas para writeups:
- `DockerLabs`
- `HackTheBox`
- `TryHackMe`

### Dificultades:
- `Fácil`
- `Media`
- `Difícil`
