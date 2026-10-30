# Awesome Ai Benchmarks

[English](README.md) | [Français](README.fr.md) | [Español](README.es.md) | [中文](README.zh-CN.md) | **日本語** | [Русский](README.ru.md)

LLM ベンチマークと評価ツール

LLMベンチマーク
| ベンチマーク | 対策 |
|---|---|
| MMLU | 幅広い知識 |
| GPQA | 大学院レベルの推論 |
| ヒューマンイーバル / MBPP | コード生成 |
| SWE-bench | リアルレポ問題の修正 |
| MMLU-Pro | より硬いMMLU |
| チャットボット・アリーナ(LMSYS) | 人間好みのELO - 最も信頼される |
| ARC-AGI | ノベル推論 |
| MT-Bench | マルチターン会話 |

## Evalフレームワーク
| ツール | ノート |
|---|---|
| [lm-eval-harness](https://github.com/EleutherAI/lm-evaluation-harness) | 標準OSSハーネス |
| 【OpenAI evals】(https://github.com/openai/evals) | OpenAIのフレームワーク |
| [DeepEval](https://github.com/confident-ai/deepeval) | pytest-style LLMテスト |
| 【RAGAS】(https://github.com/explodinggradients/ragas) | RAG専用メトリック |
| [promptfoo](https://github.com/promptfoo/promptfoo) | プロンプト CI/CD テスト |
| [Langfuse](https://github.com/langfuse/langfuse) | 観察性+無効 |

## 📐 イメージ/その他
- **ImageNet, COCO** — 古典
- **GenEval, TIFA** — イメージ・ジェネラル
-**ASR(WER)** — スピーチの転写エラー率

## ✨ 洞窟
- ベンチマークがゲームをゲット — 汚染と楕円形の方法論をチェック
- 闘技場ELOは、味を反映します, ないタスクフィット — *your*のワークロードのテスト
- 初期に内部の楕円セットを構築 — 20 実際の例は、リーダーボードの閲覧をビートします

##現在のフロンティアベンチマーク

| ベンチマーク | テスト |
|---|---|
| SWE-bench 検証 | 実際のGitHubの問題修正 |
| ARC-AGI | 抽象的な推論 |
| GPQA | 大学院レベルの科学 |
| フロンティア数学 | 研究数学 |
| 人類最後の試験 | クロスドメインの専門家 |
| ターミナルベンチ | クリエイティカルタスク |

## ライブリーダーボード

- [LMArena](https://lmarena.ai/) — 盲目の人間の好み
- [構造解析](https://artificialanalysis.ai/) — スピード/コスト/品質
- [LiveBench](https://livebench.ai/) — 汚染のない
- [LLM リーダーボードを開く](https://huggingface.co/spaces/open-llm-leaderboard) — HF の

---
## 貢献

プルリクエストを歓迎します。レビューしてマージします。[aixisstudio](https://github.com/aixisstudio) による管理 — オープンソースのアプリケーションファイアウォール [Snitch](https://github.com/aixisstudio/Snitch) の作者です。

## ライセンス: MIT
