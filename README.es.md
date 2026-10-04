# plain-language

[English](README.md)

Un conjunto breve de reglas de lenguaje claro para agentes de programación, en inglés y español.
El agente las aplica a sus respuestas, documentación, comentarios y mensajes de commit.
También puedes pedirle que revise o reescriba un texto en lenguaje claro.

Las reglas siguen los cuatro principios de la norma ISO 24495-1 (en España, UNE-ISO 24495-1): pertinente, localizable, comprensible y utilizable.
La redacción es propia; no copia texto de la norma.
Ocupan unos 600 tokens, así que puedes cargarlas en todas las sesiones.

## Instalar como skill

Ejecuta:

```sh
npx skills add gecm0/plain-language
```

O copia `skills/plain-language/` en la carpeta de skills de tu agente:

| Agente | Carpeta |
|---|---|
| Claude Code | `~/.claude/skills/` |
| Codex | `~/.agents/skills/` |
| Pi | `~/.agents/skills/` o `~/.pi/agent/skills/` |

## Activarlo siempre

El agente carga un skill solo cuando decide que hace falta.
Para aplicar las reglas en todas las respuestas, carga también el archivo desde las instrucciones globales del agente:

| Agente | Archivo | Qué añadir |
|---|---|---|
| Claude Code | `~/.claude/CLAUDE.md` | `@~/.claude/skills/plain-language/SKILL.md` |
| Codex | `~/.codex/AGENTS.md` | el contenido de `SKILL.md` |
| Pi | `~/.pi/agent/APPEND_SYSTEM.md` | el contenido de `SKILL.md` |

Codex y Pi no admiten importaciones: pega el contenido o crea un enlace simbólico a `SKILL.md`.

## Licencia

MIT
