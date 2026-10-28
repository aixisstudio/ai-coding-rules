# Ai Coding Rules

[English](README.md) | [Français](README.fr.md) | [Español](README.es.md) | [中文](README.zh-CN.md) | [日本語](README.ja.md) | **Русский**

Правила для Cursor, CLAUDE.md, AGENTS.md

_Подробное содержимое (списки, ссылки, описания) ведётся на английском — разделы ниже помогут сориентироваться._

## 📐 What this is

The dotfiles of the AI era: **`CLAUDE.md`, `.cursor/rules`, `AGENTS.md`, `.windsurfrules`, `.github/copilot-instructions.md`** — the project-level config that makes AI coding tools actually understand your codebase.

The difference between a useless AI suggestion and a great one is usually this file.

## 📁 The collection

### By tool
| File | Tool | Loaded |
|---|---|---|
| `CLAUDE.md` | Claude Code | Automatically, repo root |
| `.cursor/rules/*.mdc` | Cursor | Glob-matched or always |
| `AGENTS.md` | OpenAI Codex, others | Emerging standard |
| `.windsurfrules` | Windsurf | Project root |
| `.github/copilot-instructions.md` | Copilot | Workspace |
| `.continue/config` | Continue | IDE config |
| `.aider.conf.yml` | Aider | CLI config |

### By stack — ready-made templates
| Template | Best lines inside |
|---|---|
| `python-fastapi.md` | pydantic v2 syntax, async patterns, no print() — use logging |
| `typescript-nextjs.md` | app router conventions, server components default, zod validation |
| `rust-cli.md` | clap v4, anyhow vs thiserror split |
| `go-service.md` | standard layout, no global state |
| `react-vite.md` | hooks rules, tanstack-query for fetching |

## ✍️ What a great rules file contains

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

1. **Commands section** — the AI stops guessing how to run tests
2. **"Never do" list** — negative constraints prevent the worst diffs
3. **One-file-per-domain** in `.cursor/rules` with globs: `frontend/*.mdc` → `**/*.tsx`
4. **Link, don't paste** — reference real files: `@src/db/base.py` as the ORM example
5. **Keep under 150 lines** — longer rules get ignored/truncated

---
## Участие

Pull request'ы приветствуются — открой PR, он будет проверен и принят. Ведёт [aixisstudio](https://github.com/aixisstudio), автор [Snitch](https://github.com/aixisstudio/Snitch) — open-source application firewall.

## Лицензия: MIT
