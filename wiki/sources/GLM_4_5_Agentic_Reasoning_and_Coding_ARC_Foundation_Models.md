---
type: source
title: "GLM-4.5: Agentic, Reasoning, and Coding (ARC) Foundation Models"
summary: "模型报告型论文，介绍 GLM-4.5 与 GLM-4.5-Air 两个 MoE 模型，并报告其在 agentic、reasoning、coding 多类 benchmark 上的表现。"
tags: [paper, model-report, reasoning, coding, ai-coding-agents]
sources: ["raw/research_papers/third/GLM-4.5- Agentic, Reasoning, and Coding (ARC) Foundation Models.pdf"]
status: growing
updated: "2026-04-12"
---

# GLM-4.5: Agentic, Reasoning, and Coding (ARC) Foundation Models

## 1. Paper Metadata
- Title: 作者明确写出：GLM-4.5: Agentic, Reasoning, and Coding (ARC) Foundation Models
- Authors: 作者明确写出：GLM-4.5 Team, ZhipuAI & Tsinghua University
- Venue: Needs verification
- Year: Needs verification
- DOI / URL: 作者明确写出：https://github.com/zai-org/GLM-4.5
- Source File: 本地路径说明：`raw/research_papers/third/GLM-4.5- Agentic, Reasoning, and Coding (ARC) Foundation Models.pdf`
- Reading Status: skim

## 2. Research Problem
- Problem: 作者明确写出：需要同时提升 agentic、reasoning 和 coding 三类核心能力，以支持更通用的 problem-solving model。
- Why this problem matters: 作者明确写出：这些能力是提升真实生产力和解决复杂专业任务的关键。
- Gap in prior work: 作者明确写出：现有模型往往在某一能力上突出，但未必统一兼顾 ARC 三类能力。
- Target scenario / domain: 作者明确写出：agentic, reasoning, and coding tasks。

## 3. Core Idea / Contribution
- High-level idea: 作者明确写出：提出 GLM-4.5 与 GLM-4.5-Air 两个 open-source MoE models。
- Claimed contributions: 作者明确写出：multi-stage training on 23T tokens；hybrid reasoning method；公开模型、代码与信息。
- What is novel compared with prior work: 作者明确写出：支持 thinking 和 direct response 两种模式，并在 ARC benchmarks 上取得强性能。
- My one-sentence understanding: 我的解释：这是一篇综合型 foundation model 报告，目标是同时覆盖 agentic、reasoning、coding。

## 4. Method / Design
- Input: 作者明确写出：23T tokens training data。
- Output: 作者明确写出：GLM-4.5 和 GLM-4.5-Air。
- Pipeline / framework: 作者明确写出：multi-stage training + comprehensive post-training + expert model iteration + reinforcement learning。
- Key components: 作者明确写出：MoE architecture；hybrid reasoning。
- Key assumptions: 作者明确写出：ARC 三能力可以作为 generalist model 的关键衡量维度。
- Notation / terms worth remembering: 作者明确写出：ARC, GLM-4.5, GLM-4.5-Air。

## 5. Experiment Setup
- Dataset(s): Not explicitly stated
- Baseline(s): 作者明确写出：与多个 evaluated models 比较。
- Metrics: 作者明确写出：TAU-Bench, AIME24, SWE-bench Verified scores。
- Evaluation protocol: 作者明确写出：跨 agentic、reasoning、coding benchmarks 报告。
- Implementation details (if important): 作者明确写出：355B total / 32B activated for GLM-4.5；106B for GLM-4.5-Air。
- Reproducibility notes: 作者明确写出：模型权重与代码公开。

## 6. Results
- Main findings: 作者明确写出：GLM-4.5 在 ARC tasks 上表现强劲。
- Quantitative improvements: 作者明确写出：70.1% on TAU-Bench；91.0% on AIME24；64.2% on SWE-bench Verified。
- Qualitative findings: 作者明确写出：GLM-4.5 overall ranks 3rd and 2nd on agentic benchmarks among evaluated models。
- What evidence is actually convincing: 作者明确写出：跨多类 benchmark 汇报结果。
- What evidence is weak / insufficient: Needs verification：具体对手模型、评测条件和 ranking 口径需完整复核。

## 7. Limitations
### Authors' Stated Limitations
- Not explicitly stated

### My Observed Limitations
- 我的解释：作为 model report，当前可见内容更偏性能汇报，局限性表述较少。

## 8. Hidden Risks / Unverified Risks
- What may still go wrong: 我的解释：benchmark 强不代表真实软件工程场景稳定。
- Does the evaluation miss important failure cases?: 我的解释：可能缺少长期 agent workflow 与维护型任务。
- Is there a risk of “tests pass but system is still wrong”?: 我的解释：Yes，尤其在 coding benchmarks 外。
- Possible threats to reliability / validity: 我的解释：cross-benchmark ranking 可能依赖具体 benchmark 选择。
- What should have been checked but was not: Needs verification

## 9. Relevance to My Research
- Relation to my topic: 我的解释：如果研究 agentic/coding foundation models 的综合能力，这篇论文相关。
- Useful ideas I can borrow: 我的解释：把 ARC 作为统一能力框架。
- Possible experiment inspired by this paper: 我的解释：比较 foundation models 在真实 repository tasks 与 ARC benchmark 上的一致性。
- Whether it supports / challenges my current hypothesis: 我的解释：支持“大模型能力需要跨 agentic、reasoning、coding 联合看”。
- Priority for future revisit: medium

## 10. Future Work
### Authors' Suggested Future Work
- Not explicitly stated

### Future Work Type
- [ ] more data
- [ ] more domains
- [ ] stronger baseline
- [ ] better evaluation
- [x] robustness / reliability
- [ ] real-world deployment
- [ ] human study
- [ ] interpretability
- [ ] causal explanation
- [x] efficiency / scalability
- [ ] other:

### My Interpretation
- 我的解释：后续应看这类模型在真实 agent workflow 中的可靠性。

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
- [[concepts/ai_coding_agents]]
- [[concepts/agentic_coding_benchmarks]]

## 13. Linked Entities
- Needs verification

## 14. Linked Research Questions
- [[research_questions/What_limits_real_world_agentic_coding]]

## 15. Notes / Quotes
- 作者明确写出：GLM-4.5 achieves 70.1% on TAU-Bench, 91.0% on AIME24, and 64.2% on SWE-bench Verified.

## 16. Open Questions
- ARC benchmark 的高分能否迁移到真实 repository tasks？
- hybrid reasoning mode 在不同任务上如何调度最有效？

---

## Extraction Notes
- Only write claims supported by the source.
