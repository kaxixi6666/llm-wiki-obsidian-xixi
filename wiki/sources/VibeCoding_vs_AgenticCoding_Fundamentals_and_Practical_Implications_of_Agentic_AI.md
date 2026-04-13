---
type: source
title: "VibeCoding vs. Agentic Coding: Fundamentals and Practical Implications of Agentic AI"
summary: "一篇对比性综述，分析 vibe coding 与 agentic coding 在 autonomy、architectural design、developer role 等方面的差异，并讨论混合架构与未来路线。"
tags: [paper, survey, vibe-coding, agentic-coding]
sources: ["raw/research_papers/third/VibeCodingvsAgenticCoding.pdf"]
status: growing
updated: "2026-04-12"
---

# VibeCoding vs. Agentic Coding: Fundamentals and Practical Implications of Agentic AI

## 1. Paper Metadata
- Title: 作者明确写出：VibeCoding vs. Agentic Coding: Fundamentals and Practical Implications of Agentic AI
- Authors: 作者明确写出：Ranjan Sapkota, Konstantinos I. Roumeliotis, Manoj Karkee
- Venue: Needs verification
- Year: Needs verification
- DOI / URL: Not explicitly stated
- Source File: 本地路径说明：`raw/research_papers/third/VibeCodingvsAgenticCoding.pdf`
- Reading Status: semi-deep

## 2. Research Problem
- Problem: 作者明确写出：需要系统比较 vibe coding 与 agentic coding 两种新兴范式。
- Why this problem matters: 作者明确写出：二者都基于 LLM，但在 autonomy、architectural design、developer role 上有根本差异。
- Gap in prior work: 作者明确写出：需要 detailed taxonomy、comparative workflow analysis 和 practical implications。
- Target scenario / domain: 作者明确写出：AI-assisted software development。

## 3. Core Idea / Contribution
- High-level idea: 作者明确写出：提出 detailed taxonomy，比较 conceptual foundations、execution models、feedback loops、safety mechanisms、debugging strategies、tool ecosystems。
- Claimed contributions: 作者明确写出：通过 comparative workflow analysis 和 20 detailed use cases，说明 vibe systems 和 agentic systems 各自擅长的场景。
- What is novel compared with prior work: Needs verification
- My one-sentence understanding: 我的解释：这篇论文的重点是把 vibe coding 和 agentic coding 明确区分开，而不是混着谈。

## 4. Method / Design
- Input: 作者明确写出：comparative workflow analysis；20 detailed use cases。
- Output: 作者明确写出：taxonomy、未来路线图。
- Pipeline / framework: 作者明确写出：review + comparative analysis。
- Key components: 作者明确写出：autonomy、feedback loops、safety、debugging、tool ecosystems。
- Key assumptions: 作者明确写出：这两个范式在实践中各有优势，并可能走向 hybrid architectures。
- Notation / terms worth remembering: 作者明确写出：vibe coding、agentic coding、hybrid architectures。

## 5. Experiment Setup
- Dataset(s): 作者明确写出：20 detailed use cases。
- Baseline(s): 作者明确写出：vibe coding vs agentic coding。
- Metrics: Not explicitly stated
- Evaluation protocol: 作者明确写出：comparative workflow analysis。
- Implementation details (if important): Not explicitly stated
- Reproducibility notes: Not explicitly stated

## 6. Results
- Main findings: 作者明确写出：vibe systems 更适合早期原型和教育；agentic systems 更适合 enterprise-grade automation、codebase refactoring、CI/CD integration。
- Quantitative improvements: Not explicitly stated
- Qualitative findings: 作者明确写出：未来 AI software engineering 不是二选一，而是需要 harmonizing their strengths。
- What evidence is actually convincing: 作者明确写出：taxonomy + 20 use cases。
- What evidence is weak / insufficient: Needs verification：对比分析细节与 use case 选取标准需全文复核。

## 7. Limitations
### Authors' Stated Limitations
- 作者明确写出：agentic coding 存在 reduced human oversight、opaque execution logic、uncontrolled access to critical infrastructure 等风险。
- 作者明确写出：过度依赖 agents 可能导致 skill atrophy、situational awareness 降低和 silent error propagation。

### My Observed Limitations
- 我的解释：当前可恢复的是对 agentic coding 风险的论述，论文方法学细节仍需补读。

## 8. Hidden Risks / Unverified Risks
- What may still go wrong: 我的解释：二分式比较可能低估真实系统中的混合工作流。
- Does the evaluation miss important failure cases?: 我的解释：可能缺少长期团队协作和治理场景。
- Is there a risk of “tests pass but system is still wrong”?: 我的解释：Yes，特别是 silent error propagation 场景。
- Possible threats to reliability / validity: 我的解释：use case 驱动的对比分析可能受案例选择影响。
- What should have been checked but was not: Needs verification

## 9. Relevance to My Research
- Relation to my topic: 我的解释：如果你正在区分 vibe coding 与 agentic coding，这篇论文直接相关。
- Useful ideas I can borrow: 我的解释：把两种范式按 autonomy / execution / feedback / safety 系统比较。
- Possible experiment inspired by this paper: 我的解释：设计混合式 workflow，比较在真实任务中的表现。
- Whether it supports / challenges my current hypothesis: 我的解释：支持“vibe coding 与 agentic coding 不应混为一谈”。
- Priority for future revisit: high

## 10. Future Work
### Authors' Suggested Future Work
- 作者明确写出：articulate a future roadmap for agentic AI，强调 trustworthiness、explainability、collaboration 所需基础设施。

### Future Work Type
- [ ] more data
- [x] more domains
- [ ] stronger baseline
- [ ] better evaluation
- [x] robustness / reliability
- [x] real-world deployment
- [ ] human study
- [x] interpretability
- [ ] causal explanation
- [ ] efficiency / scalability
- [x] other: hybrid architectures

### My Interpretation
- 我的解释：后续重点在 hybrid architectures 与可信 agentic AI 基础设施。

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
- 作者明确写出：successful AI software engineering will rely not on choosing one paradigm, but on harmonizing their strengths.

## 16. Open Questions
- 在真实团队里，vibe coding 和 agentic coding 的最佳分工是什么？
- hybrid architectures 需要哪些治理与安全机制？

---

## Extraction Notes
- Only write claims supported by the source.

