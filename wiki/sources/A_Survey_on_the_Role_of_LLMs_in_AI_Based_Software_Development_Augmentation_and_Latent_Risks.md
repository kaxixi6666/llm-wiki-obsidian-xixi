---
type: source
title: "A Survey on the Role of LLMs in AI-Based Software Development: Augmentation and Latent Risks"
summary: "一篇聚焦软件开发与安全的综述，讨论 LLM 如何同时增强 SDL / DevSecOps / code review / threat modeling 等实践，并引入 latent security risks。"
tags: [paper, survey, software-security, llm]
sources: ["raw/research_papers/second/A_Survey_on_the_Role_of_LLMs_in_AI-Based_Software_Development_Augmentation_and_Latent_Risks.pdf"]
status: growing
updated: "2026-04-12"
---

# A Survey on the Role of LLMs in AI-Based Software Development: Augmentation and Latent Risks

## 1. Paper Metadata
- Title: 作者明确写出：A Survey on the Role of LLMs in AI-Based Software Development: Augmentation and Latent Risks
- Authors: 作者明确写出：Md Bajlur Rashid, Mohammad Shafayet Jamil Hossain, Mohammad Ishtiaque Khan, Sharaban Tahora, Aiasha Siddika, Mahmudul Islam Prakash, Sharmin Yeasmin, Hossain Shahriar
- Venue: Needs verification
- Year: Needs verification
- DOI / URL: Not explicitly stated
- Source File: 本地路径说明：`raw/research_papers/second/A_Survey_on_the_Role_of_LLMs_in_AI-Based_Software_Development_Augmentation_and_Latent_Risks.pdf`
- Reading Status: skim

## 2. Research Problem
- Problem: 作者明确写出：LLMs 在 AI-based software development 中具有双重角色，一方面增强实践，另一方面引入 latent risks。
- Why this problem matters: 作者明确写出：这些风险会影响 long-term reliability 与 compliance。
- Gap in prior work: 作者明确写出：需要整合 2020-2025 研究，对 augmentation 与 latent risks 同时评估。
- Target scenario / domain: 作者明确写出：SDL、DevSecOps、code review、threat modeling、supply chain security。

## 3. Core Idea / Contribution
- High-level idea: 作者明确写出：通过 survey consolidating empirical findings、benchmarking studies、sector-specific applications。
- Claimed contributions: 作者明确写出：同时梳理 secure coding acceleration 与 unsafe pattern propagation。
- What is novel compared with prior work: Needs verification
- My one-sentence understanding: 我的解释：这篇论文想把“LLM 帮了什么忙”和“它又带来了什么安全债”一起讲清楚。

## 4. Method / Design
- Input: 作者明确写出：recent studies from 2020-2025。
- Output: 作者明确写出：关于 LLM augmentation and latent risks 的综合结构化视图。
- Pipeline / framework: 作者明确写出：survey + case studies。
- Key components: 作者明确写出：SDL/DevSecOps、Code Review、Threat Modeling、Supply Chain。
- Key assumptions: 作者明确写出：LLM 作用 inherently dual。
- Notation / terms worth remembering: 作者明确写出：augmentation, latent risks。

## 5. Experiment Setup
- Dataset(s): Not explicitly stated
- Baseline(s): Not explicitly stated
- Metrics: Not explicitly stated
- Evaluation protocol: 作者明确写出：survey 2020-2025 studies。
- Implementation details (if important): Not explicitly stated
- Reproducibility notes: Not explicitly stated

## 6. Results
- Main findings: 作者明确写出：LLM 同时加速 secure coding / vulnerability detection，也会引入 insecure suggestions、data leakage、adversarial misuse。
- Quantitative improvements: Needs verification
- Qualitative findings: 作者明确写出：在 SDL / DevSecOps 中可加速 detection，但 false positives 高；在 code review 中可 flag CWEs，但许多 fixes 不安全或过度简化；threat modeling 深度仍不及 STRIDE / PASTA。
- What evidence is actually convincing: 作者明确写出：case studies 和 sector-specific synthesis。
- What evidence is weak / insufficient: Needs verification：survey protocol、覆盖范围和量化对比需要全文复核。

## 7. Limitations
### Authors' Stated Limitations
- 作者明确写出：high false positives、uneven precision、context gaps、ineffective patches 等问题。

### My Observed Limitations
- 我的解释：当前抽取更像 survey summary 和 limitation table 片段，完整方法学需要补读。

## 8. Hidden Risks / Unverified Risks
- What may still go wrong: 我的解释：survey 可能把不同任务和模型能力混合总结。
- Does the evaluation miss important failure cases?: 我的解释：可能缺少工业组织中的深层合规场景。
- Is there a risk of “tests pass but system is still wrong”?: 我的解释：Yes，特别是在 security review 中。
- Possible threats to reliability / validity: 我的解释：latent risks 的频率和严重性未必可直接横向比较。
- What should have been checked but was not: Needs verification

## 9. Relevance to My Research
- Relation to my topic: 我的解释：如果你关注 LLM coding agents 的安全性与风险，这篇论文很相关。
- Useful ideas I can borrow: 我的解释：把 augmentation 与 latent risks 放在同一分析框架下。
- Possible experiment inspired by this paper: 我的解释：选一个具体 security workflow 做实证而不是泛泛 survey。
- Whether it supports / challenges my current hypothesis: 我的解释：支持“developer aid 可以快速转化为 security debt”。
- Priority for future revisit: medium

## 10. Future Work
### Authors' Suggested Future Work
- Needs verification

### Future Work Type
- [x] more data
- [x] more domains
- [ ] stronger baseline
- [ ] better evaluation
- [x] robustness / reliability
- [x] real-world deployment
- [ ] human study
- [ ] interpretability
- [ ] causal explanation
- [ ] efficiency / scalability
- [x] other: compliance and security workflows

### My Interpretation
- 我的解释：后续重点在更细粒度地分解安全收益与安全风险。

## 11. Key References
### References by Publication Year
| Year | Citation | Why it matters |
|------|----------|----------------|
|      |          | Needs verification |

### References by Citation Order in This Paper
1. Needs verification

### Most Relevant References for My Topic
- Needs verification

## 12. Linked Concepts
- [[concepts/software_security]]
- [[concepts/ai_coding_agents]]

## 13. Linked Entities
- Needs verification

## 14. Linked Research Questions
- [[research_questions/What_limits_real_world_agentic_coding]]

## 15. Notes / Quotes
- 作者明确写出：Their role is inherently dual.

## 16. Open Questions
- 在实际 DevSecOps 流程中，augmentation 与 latent risk 的边界在哪里？
- 开发者过度依赖 LLM 是否会加剧安全债的积累？

---

## Extraction Notes
- Only write claims supported by the source.

