<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/sthanika-ai/.github/main/profile/assets/banner-dark.png?v=2">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/sthanika-ai/.github/main/profile/assets/banner-light.png?v=2">
  <img alt="Sthānika AI — an independent research lab building small, specialist, open AI models for Indian languages and domains." src="https://raw.githubusercontent.com/sthanika-ai/.github/main/profile/assets/banner-light.png?v=2">
</picture>

<br/>
<br/>

[![Website](https://img.shields.io/badge/sthanika.ai-56BF4F?style=for-the-badge&logo=firefox&logoColor=1E281F&labelColor=1E281F)](https://sthanika.ai)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-56BF4F?style=for-the-badge&logo=huggingface&logoColor=1E281F&labelColor=1E281F)](https://huggingface.co/sthanika-ai)
[![Contact](https://img.shields.io/badge/hello@sthanika.ai-56BF4F?style=for-the-badge&logo=maildotru&logoColor=1E281F&labelColor=1E281F)](mailto:hello@sthanika.ai)

<br/>

**An independent research lab building small, specialist, open AI models<br/>for Indian languages and domains.**

<table>
<tr>
<td align="center" width="185"><h1>4</h1><b>open models</b><br/><sub>on Hugging Face</sub></td>
<td align="center" width="185"><h1>11</h1><b>public repos</b><br/><sub>code, harnesses, leaderboards</sub></td>
</tr>
</table>

</div>

---

Sthānika AI builds small, specialist open models and the benchmarks used to judge them, and
releases everything with weights, datasets, evaluation code, and papers. Our work focuses on
what general-purpose models get wrong about India: its languages, its units and number
systems, its scripts, and its public-service domains such as agriculture.

[sthanika.ai](https://sthanika.ai) · [Hugging Face](https://huggingface.co/sthanika-ai) · [hello@sthanika.ai](mailto:hello@sthanika.ai)

---

# What we've built

Models, datasets, and the code behind them. Weights and datasets live on the Hugging Face Hub;
the code that produced them is here on GitHub.

| Release | Type | What it does or measures | Hugging Face | GitHub |
|---|---|---|---|---|
| **Sieve** (2B · 4B · 9B) | Models | Calibrated probabilities for typed questions about text or JSON, without generating text | [Collection](https://huggingface.co/collections/sthanika-ai/sieve) | [Sieve](https://github.com/sthanika-ai/Sieve) · [decision-index](https://github.com/sthanika-ai/decision-index) |
| **gemma3-12b-kcc-advisory** | Model | Crop advisory for Indian farmers in 11 languages | [Model](https://huggingface.co/sthanika-ai/gemma3-12b-kcc-advisory) | — |
| **Indic-KCC-Agri-Advisory-Benchmark** | Benchmark | Open-ended agri-advisory QA in 11 languages | [Dataset](https://huggingface.co/datasets/sthanika-ai/Indic-KCC-Agri-Advisory-Benchmark) | [Harness](https://github.com/sthanika-ai/Indic-KCC-Agri-Advisory-Benchmark) · [Leaderboard](https://github.com/sthanika-ai/Indic-Agri-Benchmark-Model-Configs) |
| **Bharat-Knowledge-Probe (BKP-500)** | Benchmark | India-specific knowledge vs. weak arithmetic | [Dataset](https://huggingface.co/datasets/sthanika-ai/Bharat-Knowledge-Probe-Benchmark) | [Harness](https://github.com/sthanika-ai/Bharat-Knowledge-Probe-Benchmark) · [Model runs](https://github.com/sthanika-ai/BKP-500-model-runs) |

<br/>

## 🎯 &nbsp;Sieve &nbsp;— decision models

<a href="https://huggingface.co/collections/sthanika-ai/sieve"><img alt="Collection" src="https://img.shields.io/badge/🤗%20Collection-Sieve-FFD21E?style=flat-square"></a>
<a href="https://github.com/sthanika-ai/Sieve"><img alt="Code" src="https://img.shields.io/badge/Code-1E281F?style=flat-square&logo=github&logoColor=white"></a>
<a href="https://github.com/sthanika-ai/decision-index"><img alt="Benchmark suite" src="https://img.shields.io/badge/decision--index-1E281F?style=flat-square&logo=github&logoColor=white"></a>
![Method](https://img.shields.io/badge/method-LoRA-56BF4F?style=flat-square)
![License](https://img.shields.io/badge/code-Apache--2.0-56BF4F?style=flat-square)

Decision models that **return calibrated probabilities for typed questions** — choice, yes/no,
or score — about text or JSON, **without generating text**. Training code and evaluation
are open.

| Model | Results |
|---|---|
| [**Sieve-2B**](https://huggingface.co/sthanika-ai/sieve-2b) | [Decision-index results](https://huggingface.co/datasets/sthanika-ai/Sieve-2B-decision-index-results) |
| [**Sieve-4B**](https://huggingface.co/sthanika-ai/Sieve-4B) | [Decision-index results](https://huggingface.co/datasets/sthanika-ai/Sieve-4B-decision-index-results) |
| [**Sieve-9B**](https://huggingface.co/sthanika-ai/Sieve-9B) | [Decision-index results](https://huggingface.co/datasets/sthanika-ai/Sieve-9B-decision-index-results) |

Reproduce the full benchmark suite locally, or as a single Hugging Face Job, with
[**decision-index**](https://github.com/sthanika-ai/decision-index).

<br/>

## 🌱 &nbsp;gemma3-12b-kcc-advisory &nbsp;— crop advisory model

<a href="https://huggingface.co/sthanika-ai/gemma3-12b-kcc-advisory"><img alt="Model" src="https://img.shields.io/badge/🤗%20Model-sthanika--ai%2Fgemma3--12b--kcc--advisory-FFD21E?style=flat-square"></a>
![Base](https://img.shields.io/badge/base-gemma--3--12b--it-56BF4F?style=flat-square)
![Method](https://img.shields.io/badge/method-LoRA%20%2F%20PEFT-56BF4F?style=flat-square)
![Languages](https://img.shields.io/badge/languages-11-56BF4F?style=flat-square)

A **12B crop-advisory model for Indian farmers**, fine-tuned on real Kisan Call Centre
advisory conversations across 11 Indian languages.

Judged on our own [Indic-KCC-Agri-Advisory-Benchmark](https://huggingface.co/datasets/sthanika-ai/Indic-KCC-Agri-Advisory-Benchmark)
(1–5 scale, four axes), it **more than closes the gap to models twice its size**:

| | Correctness | Naturalness | Groundedness | Safety |
|---|:---:|:---:|:---:|:---:|
| **gemma3-12b-kcc-advisory** *(ours, 12B)* | **3.44** | **4.13** | **3.93** | **4.54** |
| `gemma-3-12b-it` *(its own base, 12B)* | 2.30 | 3.22 | 3.44 | 4.84 |
| `gemma-3-27b-it` *(baseline, 27B)* | 3.26 | 3.78 | 4.16 | 4.76 |

**+1.14 correctness over the base model it was trained from**, and ahead of the 27B
baseline on the axis that matters most for advisory quality — at less than half the
parameters.

<br/>

## 🌾 &nbsp;Indic-KCC-Agri-Advisory-Benchmark

<a href="https://huggingface.co/datasets/sthanika-ai/Indic-KCC-Agri-Advisory-Benchmark"><img alt="Dataset" src="https://img.shields.io/badge/🤗%20Dataset-Indic--KCC--Agri--Advisory--Benchmark-FFD21E?style=flat-square"></a>
<a href="https://github.com/sthanika-ai/Indic-KCC-Agri-Advisory-Benchmark"><img alt="Harness" src="https://img.shields.io/badge/Harness-1E281F?style=flat-square&logo=github&logoColor=white"></a>
<a href="https://github.com/sthanika-ai/Indic-Agri-Benchmark-Model-Configs"><img alt="Leaderboard" src="https://img.shields.io/badge/Leaderboard-1E281F?style=flat-square&logo=github&logoColor=white"></a>

Open-ended agricultural-advisory question answering in **11 Indian languages**, built from
real farmer questions and the answers given by human agents at India's **Kisan Call Centre**.

500 questions were sampled once in English, then translated into the other 10 languages — so
every language scores the *same* 500 underlying questions, and cross-language comparisons are
apples-to-apples rather than confounded by a different question mix per language.

**5,500 rows · 22 baseline models evaluated · 2-stage LLM-judged scoring across 4 axes**

> ⚠️ **Benchmark only — not agronomic advice.** KCC references are noisy call-centre
> transcripts; do not act on any answer as farming guidance.

<br/>

## 🏛️ &nbsp;Bharat-Knowledge-Probe-Benchmark &nbsp;(BKP-500)

<a href="https://huggingface.co/datasets/sthanika-ai/Bharat-Knowledge-Probe-Benchmark"><img alt="Dataset" src="https://img.shields.io/badge/🤗%20Dataset-Bharat--Knowledge--Probe--Benchmark-FFD21E?style=flat-square"></a>
<a href="https://github.com/sthanika-ai/Bharat-Knowledge-Probe-Benchmark"><img alt="Harness" src="https://img.shields.io/badge/Harness-1E281F?style=flat-square&logo=github&logoColor=white"></a>
<a href="https://github.com/sthanika-ai/BKP-500-model-runs"><img alt="Leaderboard" src="https://img.shields.io/badge/Leaderboard-1E281F?style=flat-square&logo=github&logoColor=white"></a>

*Does your model know where it is?*

A benchmark of **things every Indian knows and frontier LLMs routinely fumble** — lakh/crore
arithmetic, Indian digit grouping, state-specific land units (bigha, katha, guntha),
traditional mass units, the Indian fiscal year, agricultural crop seasons, government
schemes, and structural identifiers (PAN, GSTIN, IFSC, PIN codes).

Every quantitative item has a **matched control twin** — arithmetically identical but framed
internationally — so the score separates *missing India-specific knowledge* from *weak
arithmetic*. That distinction is the whole point.

**552 core items, each reviewed by two people · 19 models evaluated · best model scores just 53.2%**

<br/>

---

# Studies

Open evaluation studies on how models handle Indian languages, scripts, and tokenization.
Each repo ships the code and configs to reproduce it from a clean clone.

| Study | The question | Repo |
|---|---|---|
| **CodeMixTax** | How much answer quality do models lose on Hinglish? | [CodeMixTax](https://github.com/sthanika-ai/CodeMixTax) |
| **India in the Wild** | Can vision-language models read real Indian street text? | [india-in-the-wild](https://github.com/sthanika-ai/india-in-the-wild) |
| **MILU evaluation** | How do newer LLMs score on MILU, and at what compute cost? | [milu-llm-evaluation](https://github.com/sthanika-ai/milu-llm-evaluation) |
| **Token fertility** | How many more tokens do Indic languages cost than English? | [token_fertility](https://github.com/sthanika-ai/token_fertility) |

<br/>

## 🔤 &nbsp;CodeMixTax &nbsp;— the code-mixing tax

The same question in English, Hinglish, Hindi, and their romanized forms, across **16
open-weight models on MMLU and GSM8K**. Scored with a floor-adjusted retention metric so weak
models aren't flattered by guessing.

**Code-mixing is not the problem. Romanization is.** Hinglish is the easiest non-English form
for every model on both tasks. Romanized Hindi, which removes both the English words and the
Devanagari script, is where models collapse: on MMLU the average model keeps 86.5% of its
English headroom on Hinglish but only 41.4% on romanized Hindi. English strength doesn't
transfer: the best English model in the study is mid-table on robustness.

<br/>

## 🪧 &nbsp;India in the Wild &nbsp;— scene-text reading

Can vision-language models read what India actually looks like: hand-painted shop signage,
fare boards, and multi-script hoardings, photographed in the wild rather than scanned from
clean pages? **Eight open-weight VLMs** transcribed all **1,319 test images** (24,987 gold
text items, 14 scripts) from the BSTD dataset, with identical prompts and programmatic,
non-model-judged scoring.

The Qwen2.5-VL models lead (32B: 0.471 fuzzy F1; 7B: 0.466), and the weakest model scores
below 0.10. Precision is reported as an upper bound on hallucination, since BSTD's
annotations aren't guaranteed exhaustive.

<br/>

## 📚 &nbsp;MILU evaluation &nbsp;— newer models, with compute cost

A reproducible evaluation of **18 newer LLMs on MILU** (AI4Bharat and IBM's Multi-task Indic
Language Understanding benchmark): about 85,000 multiple-choice questions across 8 domains
and 11 Indic languages. We run it as adopters, adding models the original paper predates and
**measured GPU-hours next to every accuracy number**.

Along the way, it found a scoring-protocol bug that silently breaks four families of hybrid
"thinking" models and would have inverted two models' ranks, and shows a **16.84-point swing**
for one model (Qwen3.6-27B) from the thinking setting alone.

<br/>

## 🔡 &nbsp;Token fertility &nbsp;— what Indic languages cost to serve

How many tokens does each model's tokenizer need for the same sentence in English, Hindi,
Telugu, Kannada, and Marathi? Measured on the full **FLORES+ devtest split (1,012 aligned
sentences)** and translated into fertility (tokens per word), parity versus English, and
serving cost. Everything runs by tokenizing locally or through free token-counting endpoints,
so reproducing it costs no generation spend.

<br/>

<div align="center">

### Work in the open

Every reported figure traces back to a raw model output through the pipeline that
produced it — so results can be independently reproduced or audited, not taken on faith.

<br/>

**Interested in Indic-language evaluation, domain-specific open models, or datasets
grounded in real Indian public-service records?**

[![Get in touch](https://img.shields.io/badge/Get%20in%20touch-hello@sthanika.ai-56BF4F?style=for-the-badge&labelColor=1E281F)](mailto:hello@sthanika.ai)

</div>
