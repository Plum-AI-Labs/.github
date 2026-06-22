<div align="center">

<img width="1200" height="300" alt="banner" src="https://github.com/user-attachments/assets/dc94867d-2efd-427a-b6bd-2c024f99810c" />

<br/><br/>

[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-4285F4?style=flat&logo=google-scholar&logoColor=white)](https://scholar.google.com/citations?view_op=list_works&hl=en&hl=en&user=x1gThJwAAAAJ)
[![License](https://img.shields.io/badge/License-MIT-2D9B5E.svg)](https://opensource.org/licenses/MIT)

</div>

---

We study how safety alignment in open-weight language models holds up under pressure — fine-tuning attacks, prompt framing, deployment-style conditions — and publish what we find, including the results that don't confirm our hypotheses.

Founded in 2025 by [Hamda Aden](https://github.com/hydrangeas20), an independent AI safety researcher and ML systems engineer.

<br/>

<div align="center">

| 96% | κ = 1.00 | <$0.10 |
|:---:|:---:|:---:|
| **Attack success rate** achieved after 50 LoRA fine-tuning steps — from a 20% baseline | **Judge reliability** on TamperBench's automated LLM-as-judge evaluation pipeline | **Cost per experiment** — every finding reproducible on a single T4 GPU |

</div>

<br/>

## Research Focus

- **Fine-tuning attack resistance** — how easily does safety alignment degrade under adversarial fine-tuning, and what does that reveal about whether alignment is learned as a robust property or a surface-level pattern?
- **Evaluation robustness** — do safety evaluations measure what we think they measure, or do they systematically overestimate model safety at category boundaries?
- **Behavioural evaluation under varying conditions** — how does model behaviour shift across prompt framings, oversight signals, and deployment-style contexts?

## Publications

| Paper | Summary | Links |
|---|---|---|
| **TamperBench** (2026) | 100-prompt benchmark across 5 harm categories measuring LoRA fine-tuning attack resistance. Safety alignment degraded from 20% → 96% attack success rate in 50 steps, for under $0.10 of compute. | [Paper](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=x1gThJwAAAAJ&citation_for_view=x1gThJwAAAAJ:9yKSN-GCB0IC) · [Code](https://github.com/Plum-AI-Labs/tamper-bench) |
| **Prompt-Framing Effects** (2026) | 600-response study examining alignment-relevant behaviour across 4 prompt conditions. Null result on the primary hypothesis, with a 5-dimensional continuous scoring framework revealing condition-level differences binary labels missed. | [Paper](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=x1gThJwAAAAJ&citation_for_view=x1gThJwAAAAJ:d1gkVwhDpl0C) · [Code](https://github.com/Plum-AI-Labs/prompt-framing) |

## Why publish null results

Most of what gets published in AI safety is positive findings. We think that's a problem. A null result, reported honestly with the right statistical rigor, is still evidence — and the field needs more of it to avoid mistaking the absence of contrary findings for the absence of risk.

## Methodology

Every project follows the same standard:

- **Automated, reusable pipelines** — every experiment is scriptable end-to-end, so findings can be reproduced or extended by anyone
- **LLM-as-judge validation against human labels** — judge reliability is measured, not assumed (Cohen's κ = 1.00 on TamperBench)
- **Pre-registered statistical thresholds** — Bonferroni correction, Wilson confidence intervals, and effect sizes reported alongside p-values
- **Low-resource by design** — every experiment runs on consumer-accessible hardware (T4 GPU), because safety research shouldn't require an industrial compute budget to verify

## Get Involved

We're a small, independent lab. If you're working on adjacent problems — fine-tuning attack resistance, evaluation robustness, open-weight model safety — we'd like to hear from you.

- Open an issue on any repo with questions, replications, or extensions
- Reach out via [LinkedIn](https://linkedin.com/in/hamda-aden)

---

<div align="center">
<sub>Plum AI Labs is an independent research lab. All work is self-funded and open-source.</sub>
</div>
