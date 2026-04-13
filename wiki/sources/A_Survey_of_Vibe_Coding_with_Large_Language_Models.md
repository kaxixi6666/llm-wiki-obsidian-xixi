---
type: source
title: "A Survey of Vibe Coding with Large Language Models"
summary: "一篇综述论文，系统梳理 vibe coding 的定义、理论基础、开发模式、基础设施与反馈机制，并从 1000 多篇研究中总结该生态。"
tags: [paper, survey, vibe-coding, llm]
sources: ["raw/research_papers/third/A Survey of Vibe Coding with Large Language Models.pdf"]
status: growing
updated: "2026-04-12"
---

# A Survey of Vibe Coding with Large Language Models

## 1. Paper Metadata
- Title: 作者明确写出：A Survey of Vibe Coding with Large Language Models
- Authors: 作者明确写出：Yuyao Ge, Lingrui Mei, Zenghao Duan, Tianhao Li, Yujia Zheng, Yiwei Wang, Lexin Wang, Jiayu Yao, Tianyu Liu, Yujun Cai, Baolong Bi, Fangda Guo, Jiafeng Guo, Shenghua Liu, Xueqi Cheng
- Venue: Needs verification
- Year: Needs verification
- DOI / URL: Not explicitly stated
- Source File: 本地路径说明：`raw/research_papers/third/A Survey of Vibe Coding with Large Language Models.pdf`
- Reading Status: semi-deep

## 2. Research Problem
- Problem: 作者明确写出：vibe coding 作为新兴开发范式具有潜力，但其有效性、工作方式与人机协作问题仍缺乏系统理解。
- Why this problem matters: 作者明确写出：已有实证证据显示它既有变革潜力，也伴随意外的生产力损失与协作挑战。
- Gap in prior work: 作者明确写出：这是第一篇 comprehensive and systematic review of Vibe Coding with LLMs。
- Target scenario / domain: 作者明确写出：vibe coding 生态，包括 coding LLMs、coding agents、development environment、feedback mechanisms。

## 3. Core Idea / Contribution
- High-level idea: 作者明确写出：对 1000+ 研究做系统综述，建立 vibe coding 的理论基础与实践框架。
- Claimed contributions: 作者明确写出：用 constrained Markov decision process 形式化 vibe coding；提出五类 development models；给出 comprehensive taxonomy。
- What is novel compared with prior work: 作者明确写出：formalize vibe coding as a discipline and provide the first comprehensive taxonomy in this domain。
- My one-sentence understanding: 我的解释：这篇论文是把“vibe coding 到底是什么”系统化地讲清楚。

## 4. Method / Design
- Input: 作者明确写出：over 1000 research papers。
- Output: 作者明确写出：理论框架、taxonomy、development models。
- Pipeline / framework: 作者明确写出：系统综述 + theoretical formalization。
- Key components: 作者明确写出：Constrained Markov Decision Process；五类 development models。
- Key assumptions: 作者明确写出：vibe coding 可被视为 human developers、software projects、coding agents 之间的动态三方关系。
- Notation / terms worth remembering: 作者明确写出：Vibe Coding；Unconstrained Automation；Iterative Conversational Collaboration；Planning-Driven；Test-Driven；Context-Enhanced。

## 5. Experiment Setup
- Dataset(s): 作者明确写出：systematic analysis of over 1000 research papers。
- Baseline(s): Not explicitly stated
- Metrics: Not explicitly stated
- Evaluation protocol: 作者明确写出：survey / taxonomy construction。
- Implementation details (if important): Not explicitly stated
- Reproducibility notes: Not explicitly stated

## 6. Results
- Main findings: 作者明确写出：successful vibe coding depends on balancing human agency, project structure, and agent autonomy。
- Quantitative improvements: Not explicitly stated
- Qualitative findings: 作者明确写出：提出五种 development models，并综述整个 vibe coding 生态。
- What evidence is actually convincing: 作者明确写出：基于大规模 literature synthesis。
- What evidence is weak / insufficient: Needs verification：survey selection protocol 和 inclusion criteria 细节需要完整复核。

## 7. Limitations
### Authors' Stated Limitations
- Needs verification

### My Observed Limitations
- 我的解释：当前抽取更容易恢复摘要和目录结构，综述方法细节仍需全文复核。

## 8. Hidden Risks / Unverified Risks
- What may still go wrong: 我的解释：taxonomy 可能受综述选文范围影响。
- Does the evaluation miss important failure cases?: 我的解释：可能低估特定平台或社区中的反例。
- Is there a risk of “tests pass but system is still wrong”?: 我的解释：Yes，survey 型论文更容易给出概念图景而非直接因果验证。
- Possible threats to reliability / validity: 我的解释：systematic review 的检索与筛选策略需要确认。
- What should have been checked but was not: Needs verification

## 9. Relevance to My Research
- Relation to my topic: 我的解释：如果你要系统研究 vibe coding，这是基础综述。
- Useful ideas I can borrow: 我的解释：五种 development models 与 CMPD 形式化框架。
- Possible experiment inspired by this paper: 我的解释：把某类 vibe coding workflow 单独拿出来做实证比较。
- Whether it supports / challenges my current hypothesis: 我的解释：支持把 vibe coding 当作独立研究对象，而不仅是“用 LLM 写代码”。
- Priority for future revisit: high

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
- [x] human study
- [x] interpretability
- [ ] causal explanation
- [ ] efficiency / scalability
- [x] other: taxonomy refinement

### My Interpretation
- 我的解释：后续重点会是把 survey taxonomy 映射到更具体的真实工作流证据上。

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
- [[concepts/vibe_coding]]
- [[concepts/ai_coding_agents]]

## 13. Linked Entities
- Needs verification

## 14. Linked Research Questions
- [[research_questions/What_limits_real_world_agentic_coding]]

## 15. Notes / Quotes
- 作者明确写出：this survey provides the first comprehensive and systematic review of Vibe Coding with large language models.

## 16. Open Questions
- 五种 development models 在真实团队中分别适合什么条件？
- vibe coding 的人机边界应如何设计？

---

## Extraction Notes
- Only write claims supported by the source.

