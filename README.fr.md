# Awesome Ai Benchmarks

[English](README.md) | **Français** | [Español](README.es.md) | [中文](README.zh-CN.md) | [日本語](README.ja.md) | [Русский](README.ru.md)

Benchmarks & évaluation de LLM — mesurer ce qui compte

_Le contenu détaillé (listes, liens, descriptions) est en anglais pour rester maintenable — les sections ci-dessous te guident._

## 🏆 LLM benchmarks
| Benchmark | Measures |
|---|---|
| MMLU | Broad knowledge (multiple choice) |
| GPQA | Graduate-level reasoning |
| HumanEval / MBPP | Code generation |
| SWE-bench | Real repo issue fixing — the one that matters |
| MMLU-Pro | Harder MMLU |
| Chatbot Arena (LMSYS) | Human-preference ELO — most trusted |
| ARC-AGI | Novel reasoning |
| MT-Bench | Multi-turn conversation |

## 🧰 Eval frameworks
| Tool | Note |
|---|---|
| [lm-eval-harness](https://github.com/EleutherAI/lm-evaluation-harness) | The standard OSS harness |
| [OpenAI evals](https://github.com/openai/evals) | OpenAI's framework |
| [DeepEval](https://github.com/confident-ai/deepeval) | pytest-style LLM tests |
| [RAGAS](https://github.com/explodinggradients/ragas) | RAG-specific metrics |
| [promptfoo](https://github.com/promptfoo/promptfoo) | Prompt CI/CD testing |
| [Langfuse](https://github.com/langfuse/langfuse) | Observability + evals |

## 📐 Image/other
- **ImageNet, COCO** — classics
- **GenEval, TIFA** — image-gen evals
- **ASR (WER)** — speech transcription error rate

## ⚠️ Caveats
- Benchmarks get gamed — check contamination & eval methodology
- Arena ELO reflects taste, not task fit — test on *your* workload
- Build an internal eval set early — 20 real examples beat leaderboard browsing

---
## Contribuer

Les pull requests sont les bienvenues : ouvre une PR, elle sera relue et fusionnée. Maintenu par [aixisstudio](https://github.com/aixisstudio), auteur de [Snitch](https://github.com/aixisstudio/Snitch), pare-feu applicatif open source.

## Licence: MIT
