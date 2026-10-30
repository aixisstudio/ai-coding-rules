# Ai Coding Rules

[English](README.md) | [Français](README.fr.md) | [Español](README.es.md) | **中文** | [日本語](README.ja.md) | [Русский](README.ru.md)

Cursor 规则、CLAUDE.md、AGENTS.md 配置集

# # 这是什么 # # What this is #

AI时代的点文件: **`CLAUDE.md`, `.cursor/rules`, `AGENTS.md`, `.windsurfrules`, `.github/copilot-instructions.md`**]——使AI编码工具实际理解你的代码库的项目级配置.

一个没用的AI建议和一个伟大的建议之间的区别通常是这个文件.

□□□□□□□□□ collection集.

按工具分类
QQ 文件 QQ 工具 装入 QQ
|---|---|---|
`CLAUDE.md` 克劳德代码 自动重播根
`.cursor/rules/*.mdc` 光彩相配或总是
* `AGENTS.md` * OpenAI Codex,其他 * 新兴标准 *
~ `.windsurfrules` ~ 风浪 ~ 项目根 ~
`.github/copilot-instructions.md` 副驾驶 工作空间
`.continue/config` 继续 IDE 配置
{\fn黑体\fs22\bord1\shad0\3aHBE\4aH00\fscx67\fscy66\2cHFFFFFF\3cH808080}CLI的配置 {\fn黑体\fs22\bord1\shad0\3aHBE\4aH00\fscx67\fscy66\2cHFFFFFF\3cH808080}你觉得呢?

### 依堆-现成模板
[永久失效連結] [永久失效連結] 腾讯网.
|---|---|
QQ `python-fastapi.md` QQ pydantic v2 语法, async图案, 无打印 () —— 使用日志 QQ
QQ `typescript-nextjs.md` 应用程序路由器常规,服务器组件默认, Zod 验证 QQ
{\fn黑体\fs22\bord1\shad0\3aHBE\4aH00\fscx67\fscy66\2cHFFFFFF\3cH808080}无论怎样 {\fn黑体\fs22\bord1\shad0\3aHBE\4aH00\fscx67\fscy66\2cHFFFFFF\3cH808080}你都喜欢我
QQ `go-service.md` 标准布局,无全局状态 QQ
~ `react-vite.md` ~ 钩子规则, 获取的纹章- query ~ ~

################################################################################################################################################################################################################################################################

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

□ □ □ 规则,可以衡量帮助(社区测试)

1. ** 命令部分** - AI停止猜测如何进行测试
2. **"Never do"列表**——负面限制防止最坏的diffs.
3. ** `.cursor/rules`中一个文件(每个域)**,含阴光:`frontend/*.mdc` → `**/*.tsx`
4. **Link,不要粘贴**——参考真实文件:`@src/db/base.py`作为ORM示例.
5. ** 保持在150行以内** -- -- 更长的规则被忽略/搁置

---
## 贡献

欢迎提交 Pull Request，我们会审查并合并。由 [aixisstudio](https://github.com/aixisstudio) 维护，他也是开源应用防火墙 [Snitch](https://github.com/aixisstudio/Snitch) 的作者。

## 许可证: MIT
