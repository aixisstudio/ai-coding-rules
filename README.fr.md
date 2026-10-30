# Ai Coding Rules

[English](README.md) | **Français** | [Español](README.es.md) | [中文](README.zh-CN.md) | [日本語](README.ja.md) | [Русский](README.ru.md)

Rules Cursor, CLAUDE.md, AGENTS.md — la config qui rend les IA de code plus malines

Ce que c'est

Les dotfiles de l'ère AI: **`CLAUDE.md`, `.cursor/rules`, `AGENTS.md`, `.windsurfrules`, `.github/copilot-instructions.md`** — la configuration au niveau du projet qui fait que les outils de codage AI comprennent réellement votre base de code.

La différence entre une suggestion inutile d'IA et une grande est généralement ce fichier.

La collection

Par outil
Outil chargé
|---|---|---|
Code Claude de `CLAUDE.md`
`.cursor/rules/*.mdc`-Cursor
Codex OpenAI, autres
`.windsurfrules`?Surf éolien?
Espace de travail
IDE configurance
`.aider.conf.yml`=Aider=CLI config=

### Par pile — modèles prêts à l'emploi
Modèle Meilleures lignes à l'intérieur
|---|---|
`python-fastapi.md`=Syntaxe pydantique v2, patrons d'async, pas d'impression() — utiliser logging
Conventions de routeur d'applications `typescript-nextjs.md`, composants de serveur par défaut, validation zod
`rust-cli.md`="clap v4, de toute façon contre cette erreur scindé"
La disposition standard du `go-service.md`, pas d'état global
`react-vite.md`=Règles des crochets, brantack-query pour récupérer

Qu'est-ce qu'un grand fichier de règles contient

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

Règles qui aident mesurablement (test communautaire)

1. ** Section des commandes** — l'IA arrête de deviner comment exécuter les tests
2. ** "Ne jamais faire" la liste** — des contraintes négatives empêchent les pires diffs
3. **One-file-par-domaine** en `.cursor/rules` avec globs: `frontend/*.mdc` → `**/*.tsx`
4. **Lien, ne pas coller** — référencer les fichiers réels: `@src/db/base.py` comme exemple ORM
5. **Conserver moins de 150 lignes** — les règles plus longues sont ignorées/tronquées

---
## Contribuer

Les pull requests sont les bienvenues : ouvre une PR, elle sera relue et fusionnée. Maintenu par [aixisstudio](https://github.com/aixisstudio), auteur de [Snitch](https://github.com/aixisstudio/Snitch), pare-feu applicatif open source.

## Licence: MIT
