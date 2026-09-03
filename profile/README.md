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
[![Contact](https://img.shields.io/badge/connect@sthanika.ai-56BF4F?style=for-the-badge&logo=maildotru&logoColor=1E281F&labelColor=1E281F)](mailto:connect@sthanika.ai)

<br/>

**A research lab building specialist, fine-tuned open models —**
**released with weights, datasets, benchmarks, and papers.**

<table>
<tr>
<td align="center" width="200"><h1>11</h1><b>Indic languages</b><br/><sub>covered end to end</sub></td>
<td align="center" width="200"><h1>18</h1><b>models evaluated</b><br/><sub>on all 11, no gaps</sub></td>
<td align="center" width="200"><h1>5,500</h1><b>benchmark rows</b><br/><sub>from real farmer calls</sub></td>
</tr>
</table>

</div>

---

## 🌾 &nbsp;Indic-KCC-Agri-Advisory-Benchmark

<a href="https://github.com/sthanika-ai/Indic-KCC-Agri-Advisory-Benchmark"><img alt="Code" src="https://img.shields.io/badge/Code-1E281F?style=flat-square&logo=github&logoColor=white"></a>
<a href="https://huggingface.co/datasets/sthanika-ai/Indic-KCC-Agri-Advisory-Benchmark"><img alt="Dataset" src="https://img.shields.io/badge/Dataset-FFD21E?style=flat-square&logo=huggingface&logoColor=1E281F"></a>
![Languages](https://img.shields.io/badge/languages-11-56BF4F?style=flat-square)
![Rows](https://img.shields.io/badge/rows-5%2C500-56BF4F?style=flat-square)

Open-ended agricultural-advisory question answering in **11 Indian languages**, built
from real farmer questions and the advisory answers given by human agents at India's
**Kisan Call Centre**.

500 questions were sampled once in English, then translated into the other 10 languages —
so every language scores the *same* 500 underlying questions. Cross-language comparisons
here are apples-to-apples, not confounded by a different question mix per language. Every
row ships with its round-trip translation-quality score, and nothing is silently dropped.

> ⚠️ **Benchmark only — not agronomic advice.** KCC references are noisy call-centre
> transcripts; do not act on any answer as farming guidance.

<br/>

## 📊 &nbsp;milu-llm-evaluation

<a href="https://github.com/sthanika-ai/milu-llm-evaluation"><img alt="Code" src="https://img.shields.io/badge/Code-1E281F?style=flat-square&logo=github&logoColor=white"></a>
![Models](https://img.shields.io/badge/models-18-56BF4F?style=flat-square)
![Coverage](https://img.shields.io/badge/coverage-11%2F11%20languages-56BF4F?style=flat-square)
![Reproducible](https://img.shields.io/badge/every%20figure-reproducible-56BF4F?style=flat-square)

A reproducible pipeline and a **completed** evaluation campaign on
[MILU](https://arxiv.org/abs/2411.02538) — AI4Bharat and IBM's Multi-task Indic Language
Understanding benchmark: 18 models, all 11 languages, end to end. Accuracy *and* real
measured cost per 1K questions, because one without the other doesn't tell you much.

| # | Model | Overall | Cost |
|---|---|---|---|
| 🥇 | Qwen3.8-Max (API) | **89.67%** | $156.60 |
| 🥈 | Qwen3.6-27B *(thinking on)* | **83.84%** | $134.83 |
| 🥉 | Sarvam-M 24B *(thinkmode)* | **82.44%** | $34.96 |

<sub>Top 3 of 18 — <a href="https://github.com/sthanika-ai/milu-llm-evaluation#1-results">full league table</a>. For reference, the original MILU paper's best score was ~74% (GPT-4o, late 2024).</sub>

Along the way we found and disclosed a scoring-protocol bug that silently breaks four
hybrid-"thinking" model families — uncorrected, it **inverts two models' rank**. Turning
thinking on for one model alone moved it **+16.84 points**.

> MILU is AI4Bharat and IBM's benchmark. We run it as adopters, not authors.

---

<div align="center">

### Work in the open

Every reported figure traces back to a raw model output through the pipeline that
produced it — so results can be independently reproduced or audited, not taken on faith.

<br/>

**Interested in Indic-language evaluation, domain-specific open models, or datasets
grounded in real Indian public-service records?**

[![Get in touch](https://img.shields.io/badge/Get%20in%20touch-connect@sthanika.ai-56BF4F?style=for-the-badge&labelColor=1E281F)](mailto:connect@sthanika.ai)

</div>
