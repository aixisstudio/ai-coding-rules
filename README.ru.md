# Ai Coding Rules

[English](README.md) | [Français](README.fr.md) | [Español](README.es.md) | [中文](README.zh-CN.md) | [日本語](README.ja.md) | **Русский**

Правила для Cursor, CLAUDE.md, AGENTS.md

###Что это такое

Точечные файлы эпохи ИИ: **`CLAUDE.md`, `.cursor/rules`, `AGENTS.md`, `.windsurfrules`, `.github/copilot-instructions.md`** — конфигурация проектного уровня, которая позволяет инструментам кодирования ИИ фактически понимать вашу кодовую базу.

Разница между бесполезным предложением ИИ и отличным обычно заключается в этом файле.

###Коллекция

### Инструмент
Скачать игру Tool Loaded
|---|---|---|
| `CLAUDE.md` | Claude Code | Автоматически, repo root |
| `.cursor/rules/*.mdc` | Cursor | Glob-совместимый или всегда |
| `AGENTS.md` | OpenAI Codex, другие | Новые стандарты |
| `.windsurfrules` | Windsurf | Корень проекта
`.github/copilot-instructions.md` | Copilot | Workspace
| `.continue/config` | Continue | IDE config |
| `.aider.conf.yml` | Aider | CLI конфигурация |

### By stack — готовые шаблоны
Лучшие строки внутри
|---|---|
| `python-fastapi.md` | pydantic v2 syntax, async patterns, no print() — используйте logging |
| `typescript-nextjs.md` | соглашения маршрутизатора приложений, серверные компоненты по умолчанию, валидация зондов |
| `rust-cli.md` | хлопок v4, как бы то ни было, vs это разделение
| `go-service.md` | стандартная компоновка без глобального состояния |
| `react-vite.md` | правила крючков, запрос танстака для извлечения |

##  a️ Какой файл правил

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

## ) Правила, которые могут помочь (проверено сообществом)

1. ** Командный раздел** — ИИ перестает гадать, как запускать тесты
2. ** "Никогда не делай" список ** - отрицательные ограничения предотвращают худшие диффы
3. ** Один файл на домен** в `.cursor/rules` с шарами: `frontend/*.mdc` → `**/*.tsx`
4. **Ссылка, не вставляйте ** — ссылки на реальные файлы: `@src/db/base.py` в качестве примера ORM
5. ** Держите под 150 строк ** - более длинные правила игнорируются / усечены

---
## Участие

Pull request'ы приветствуются — открой PR, он будет проверен и принят. Ведёт [aixisstudio](https://github.com/aixisstudio), автор [Snitch](https://github.com/aixisstudio/Snitch) — open-source application firewall.

## Лицензия: MIT
