# Awesome Ai Benchmarks

[English](README.md) | [Français](README.fr.md) | [Español](README.es.md) | [中文](README.zh-CN.md) | [日本語](README.ja.md) | **Русский**

Бенчмарки и оценка LLM

##LLM бенчмарки
[править править код]
|---|---|
MMLU - Широкие знания (множественный выбор)
| GPQA | Размышления на уровне выпускников
MBPP / HumanEval - генерация кода
[править править код] Реальный репо — тот, который имеет значение
MMLU-Pro - более жесткий MMLU
• Chatbot Arena (LMSYS) — наиболее доверенная
| ARC-AGI | Новые рассуждения
MT-Bench - многоповоротный разговор

##  framework фреймворки Eval
| Инструмент | Примечание
|---|---|
[lm-eval-harness] (https://github.com/EleutherAI/lm-evaluation-harness) Стандартная ОСС упряжка.
| [OpenAI evals] (https://github.com/openai/evals) | Рамки OpenAI |
[DeepEval] (https://github.com/confident-ai/deepeval) | тесты LLM в стиле pytest
| [RAGAS] (https://github.com/explodinggradients/ragas) | RAG-специфические метрики |
| [promptfoo] (https://github.com/promptfoo/promptfoo) | Быстрое тестирование CI/CD
| [Langfuse] (https://github.com/langfuse/langfuse) | Наблюдение + эвалы |

##   Изображение/другое
**ImageNet, COCO** — классика
- **GenEval, TIFA** - Имидж-ген
**ASR (WER)** — частота ошибок транскрипции речи

##  ️ Пещеры
- Benchmarks get gamed - check contamination & eval methodology (недоступная ссылка)
- Arena ELO отражает вкус, а не соответствие задач - тест на *вашу* рабочую нагрузку
Постройте внутренний эйвальный набор рано — 20 реальных примеров превзошли просмотр таблицы лидеров

##   Текущие пограничные ориентиры

Тестирование.
|---|---|
Проверено с помощью SWE-bench / Real GitHub
| ARC-AGI | Абстрактные рассуждения |
| GPQA | Наука высшего уровня |
FrontierMath - Исследовательская математика
Оригинальное название: Humanity's Last Exam
| Терминал-секция | CLI агентные задачи |

###Живые таблицы лидеров

- [LMArena] (https://lmarena.ai/) - предпочтение слепого человека
- [Искусственный анализ] (https://artificialanalysis.ai/) - скорость/стоимость/качество
- [LiveBench] (https://livebench.ai/) - без загрязнения
- [Open LLM Leaderboard] (https://huggingface.co/spaces/open-llm-leaderboard) - HF's

---
## Участие

Pull request'ы приветствуются — открой PR, он будет проверен и принят. Ведёт [aixisstudio](https://github.com/aixisstudio), автор [Snitch](https://github.com/aixisstudio/Snitch) — open-source application firewall.

## Лицензия: MIT
