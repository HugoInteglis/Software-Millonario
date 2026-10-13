# Software Millonario

Proyecto para idear, validar y construir un software rentable con la ayuda de
Claude Code como cofundador técnico.

## Cómo usarlo

1. Abre Claude Code en este repositorio (las instrucciones están en `CLAUDE.md`).
2. Evalúa una idea: `/validar-idea <tu idea>`
3. Si la idea pasa el filtro: `/plan-mvp <tu idea>`
4. Construye el MVP semana a semana siguiendo `docs/mvp.md`.

## Estructura

- `CLAUDE.md` — rol, principios y stack por defecto del agente.
- `.claude/agents/estratega-negocio.md` — subagente de investigación de mercado.
- `.claude/skills/validar-idea/` — puntuación objetiva de ideas.
- `.claude/skills/plan-mvp/` — plan de MVP ejecutable.
- `docs/ideas.md` — ideas evaluadas.
- `docs/decisiones.md` — registro de decisiones.
