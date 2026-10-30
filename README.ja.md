# Ai Coding Rules

[English](README.md) | [Français](README.fr.md) | [Español](README.es.md) | [中文](README.zh-CN.md) | **日本語** | [Русский](README.ru.md)

Cursor ルール・CLAUDE.md・AGENTS.md 集

##  What これは何ですか?

AI時代のドットファイル:**`CLAUDE.md`、`.cursor/rules`、`AGENTS.md`、`.windsurfrules`、`.github/copilot-instructions.md`** - AIコーディングツールが実際にあなたのコードベースを理解するプロジェクトレベルの構成。

役に立たないAI提案と素晴らしいものの違いは、通常このファイルです。

## 📁コレクション

### ツールで
| ファイル | ツール | ロード |
|---|---|---|
| `CLAUDE.md` | クロードコード | オートマチック・レポルート |
| `.cursor/rules/*.mdc` | キュラー | グローブマッチ・アンド・いつも |
| `AGENTS.md` | OpenAI Codex 他 | 新興規格 |
| `.windsurfrules` | ウィンドサーフィン | プロジェクトルート |
| `.github/copilot-instructions.md` | コピロット | ワークスペース |
| `.continue/config` | 続き | IDEの構成 |
| `.aider.conf.yml` | エイダー | クリコンフィグ |

### スタックによる — 既製のテンプレート
| テンプレート | 内側のベストライン |
|---|---|
| `python-fastapi.md` | pydantic v2 構文, async パターン, no print() — 使用 ロギング |
| `typescript-nextjs.md` | アプリルータ規約、サーバコンポーネントのデフォルト、zod検証 |
| `rust-cli.md` | clap v4、何とか対この恐怖の割れ目 |
| `go-service.md` | 標準レイアウト | グローバルな状態 |
| `react-vite.md` | ホークルール・タンスタククリ |

## 本当に素晴らしいルールファイルが含まれています

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

# # # 間違いなく助けるルール (コミュニティテスト済み)

1.**Commands セクション** — AI はテストを実行する方法の推測を停止します
2.**"Never do" list** — 負の制約は最悪の差を防ぎます
3。**`.cursor/rules`の1ファイルごとのドメイン**:`frontend/*.mdc` → `**/*.tsx`
4。 **リンク、貼り付けないでください** — 実際のファイルを参照: ORM 例として`@src/db/base.py`
5。**150行未満** - 長いルールは無視/調整される

---
## 貢献

プルリクエストを歓迎します。レビューしてマージします。[aixisstudio](https://github.com/aixisstudio) による管理 — オープンソースのアプリケーションファイアウォール [Snitch](https://github.com/aixisstudio/Snitch) の作者です。

## ライセンス: MIT
