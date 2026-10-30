# Ai Coding Rules

[English](README.md) | [Français](README.fr.md) | **Español** | [中文](README.zh-CN.md) | [日本語](README.ja.md) | [Русский](README.ru.md)

Reglas para Cursor, CLAUDE.md y AGENTS.md

Lo que es

Los ficheros de la era AI: **`CLAUDE.md`, `.cursor/rules`, `AGENTS.md`, `.windsurfrules`, `.github/copilot-instructions.md`** — el config a nivel de proyecto que hace que las herramientas de codificación AI entiendan realmente su base de código.

La diferencia entre una sugerencia de AI inútil y una gran es generalmente este archivo.

## 📁 La colección

### By tool
← Archivo Silencioso Silencioso
|---|---|---|
TENIDO `CLAUDE.md` TENIDO Código Claude TEN automáticamente, repo root TEN
Silencio `.cursor/rules/*.mdc` Silencio Cursor Silencio Glob-matched or always ←
← `AGENTS.md` Silencio OpenAI Codex, otros ¦
Silencio `.windsurfrules`
Silencio `.github/copilot-instructions.md`
Silencio `.continue/config`
Silencio `.aider.conf.yml`

## By stack — ready-made templates
Plantilla Silencioso Las mejores líneas dentro de Silencio
|---|---|
← `python-fastapi.md` Silencio pydantic v2 sintaxis, patrones de asinc, no print() — use logging ←
← `typescript-nextjs.md` Silencioso aplicación de las convenciones de router, componentes del servidor por defecto, validación de zod
Silencio `rust-cli.md` Silencio clap v4, de todos modos vs este terror split Silencio
← `go-service.md` Silencioso diseño estándar, no global estado ←
confidencialidad `react-vite.md` Silencioso ganchos reglas, tanstack-query for fetching

Qué gran archivo de reglas contiene

```markdown
# Project: Acme API

## Stack
FastAPI + SQLAlchemy async + Postgres. Tests: pytest-asyncio.

## Conventions
- All endpoints return Pydantic schemas, never dicts
- DB access only through `db/repositories/`
- No `print()` — `structlog` only
- Commits: conventional format (`feat:`, `fix:`)

## Commands
- Test: `pytest -xvs`
- Lint: `ruff check --fix`
- Run dev: `uvicorn app:app --reload`

## Never do
- Don't add deps without asking
- Don't modify migrations by hand — alembic generates them
- Don't commit `.env`
```

## 🧠 Rules that measurably help (community-tested)

1. **Sección de clientes** — la AI deja de adivinar cómo realizar pruebas
2. **"Nunca hacer" lista** — las restricciones negativas impiden los peores problemas
3. **Un archivo por dominio** en `.cursor/rules` con globs: `frontend/*.mdc` → `**/*.tsx`
4. **Link, no pega** — referencia archivos reales: `@src/db/base.py` como el ejemplo ORM
5. **Manténgase bajo 150 líneas**; las reglas más largas se ignoran/ truncan

---
## Contribuir

Los pull requests son bienvenidos: abre una PR y será revisada y fusionada. Mantenido por [aixisstudio](https://github.com/aixisstudio), autor de [Snitch](https://github.com/aixisstudio/Snitch), firewall de aplicaciones open source.

## Licencia: MIT
