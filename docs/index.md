---
---
LLM benchmarks & evaluation tools — measure what matters

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

## 🆕 Current frontier benchmarks

| Benchmark | Tests |
|---|---|
| SWE-bench Verified | Real GitHub issue fixes |
| ARC-AGI | Abstract reasoning |
| GPQA | Graduate-level science |
| FrontierMath | Research math |
| Humanity's Last Exam | Cross-domain expert |
| Terminal-Bench | CLI agentic tasks |

## 📊 Live leaderboards

- [LMArena](https://lmarena.ai/) — blind human preference
- [Artificial Analysis](https://artificialanalysis.ai/) — speed/cost/quality
- [LiveBench](https://livebench.ai/) — contamination-free
- [Open LLM Leaderboard](https://huggingface.co/spaces/open-llm-leaderboard) — HF's

---
Maintained by [aixisstudio](https://github.com/aixisstudio).