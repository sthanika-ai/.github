<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/sthanika-ai/.github/main/profile/assets/banner-dark.png?v=2">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/sthanika-ai/.github/main/profile/assets/banner-light.png?v=2">
  <img alt="Sthānika AI — targeted models for the challenges of India. Built on locally rooted wisdom." src="https://raw.githubusercontent.com/sthanika-ai/.github/main/profile/assets/banner-light.png?v=2">
</picture>

<br/>
<br/>

[![Website](https://img.shields.io/badge/sthanika.ai-56BF4F?style=for-the-badge&logo=firefox&logoColor=1E281F&labelColor=1E281F)](https://sthanika.ai)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-56BF4F?style=for-the-badge&logo=huggingface&logoColor=1E281F&labelColor=1E281F)](https://huggingface.co/sthanika-ai)
[![Contact](https://img.shields.io/badge/hello@sthanika.ai-56BF4F?style=for-the-badge&logo=maildotru&logoColor=1E281F&labelColor=1E281F)](mailto:hello@sthanika.ai)

<br/>

**A research lab building specialist, fine-tuned open models —**
**released with weights, datasets, benchmarks, and papers.**

<table>
<tr>
<td align="center" width="185"><h1>11</h1><b>Indic languages</b><br/><sub>covered end to end</sub></td>
<td align="center" width="185"><h1>3</h1><b>open releases</b><br/><sub>1 model · 2 benchmarks</sub></td>
<td align="center" width="185"><h1>85</h1><b>model evaluations</b><br/><sub>across our benchmarks</sub></td>
</tr>
</table>

</div>

---

# What we've built

Three things carry the lab's work: **one fine-tuned model** and **two open benchmarks**.
Everything below is on the Hugging Face Hub, with the code that produced it on GitHub.

<br/>

## 🌱 &nbsp;gemma3-12b-kcc-advisory &nbsp;— our fine-tuned model

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
<a href="https://github.com/sthanika-ai/BKP-500-model-runs"><img alt="Runs" src="https://img.shields.io/badge/Model%20runs-1E281F?style=flat-square&logo=github&logoColor=white"></a>

*Does your model know where it is?*

A benchmark of **things every Indian knows and frontier LLMs routinely fumble** — lakh/crore
arithmetic, Indian digit grouping, state-specific land units (bigha, katha, guntha),
traditional mass units, the Indian fiscal year, crop seasons, and structural identifiers
(PAN, GSTIN, IFSC, PIN).

Every quantitative item has a **matched control twin** — arithmetically identical but framed
internationally — so the score separates *missing India-specific knowledge* from *weak
arithmetic*. That distinction is the whole point.

**1,086 items (552 core + 534 control) · 21 models evaluated · best model scores just 53.2%**

<br/>

---

# More from the lab

Supporting research — each repo stands alone, with its methodology and reproduction steps.

| Repo | What it asks |
|---|---|
| [**Indic-Agri-Benchmark-Model-Configs**](https://github.com/sthanika-ai/Indic-Agri-Benchmark-Model-Configs) | Exact run config + leaderboard for all 22 models on the agri-advisory benchmark |
| [**BKP-500-model-runs**](https://github.com/sthanika-ai/BKP-500-model-runs) | Run configuration and full leaderboard for the 21 models evaluated on BKP-500 |
| [**milu-llm-evaluation**](https://github.com/sthanika-ai/milu-llm-evaluation) | 18 newer LLMs on MILU (AI4Bharat/IBM), all 11 languages, end to end |
| [**CodeMixTax**](https://github.com/sthanika-ai/CodeMixTax) | How much answer quality do models lose on Hinglish? *Code-mixing isn't the problem — romanization is* |
| [**india-in-the-wild**](https://github.com/sthanika-ai/india-in-the-wild) | Can vision-language models read hand-painted Indian shop signage and fare boards? |
| [**token_fertility**](https://github.com/sthanika-ai/token_fertility) | How many more tokens do Indic languages cost to serve than English? |

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
