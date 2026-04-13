---
type: research_question
title: "什么限制了真实世界中的 agentic coding？"
summary: "当前多篇论文共同指向的研究问题：在复杂 feature development、code review、repository-specific PR generation 等真实场景下，agentic coding 的核心瓶颈是什么。"
tags: [research-question, ai-coding-agents, benchmark, pull-requests]
sources: [
  "raw/research_papers/third/Code Review Agent Benchmark.pdf",
  "raw/research_papers/first/FeatureBench- Benchmarking Agentic Coding for Complex Feature Development.pdf",
  "raw/research_papers/third/Learning to Commit- Generating Organic Pull Requests via Online Repository Memory.pdf",
  "raw/research_papers/third/GLM-4.5- Agentic, Reasoning, and Coding (ARC) Foundation Models.pdf"
]
status: growing
updated: "2026-04-12"
---

# 什么限制了真实世界中的 agentic coding？

## 1. Question
- Core question: 为什么 agent 在真实软件工程场景中仍然表现不稳？
- Short version: agentic coding 的真实瓶颈是什么？
- Why it matters: 作者明确写出：真实 PR、复杂 feature development、code review 等场景比标准 benchmark 更难。
- Why it is hard: 作者明确写出：这些任务涉及 project-specific conventions、cross-file dependencies、human review expectations、repository history。

## 2. Background
- Problem context: 当前来源分别从 code review、feature development、repository memory、foundation model 报告等角度观察 agentic coding 的边界。
- Common assumptions in prior work: 我的解释：标准 benchmark 高分常被误读为真实开发能力。
- Why current evidence may be insufficient: 当前来源虽然都指出边界，但难点的相对权重仍不清楚。

## 3. Scope
- In scope: feature development、PR generation、code review、repository adaptation。
- Out of scope: 纯算法题 code generation。
- Target domain: real-world software engineering workflows。
- Key definitions / terms: [[concepts/ai_coding_agents]], [[concepts/agentic_coding_benchmarks]], [[concepts/code_review]]

## 4. Related Evidence
### Supporting
- [[sources/FeatureBench_Benchmarking_Agentic_Coding_for_Complex_Feature_Development]]：复杂 feature tasks 上成功率很低。
- [[sources/Learning_to_Commit_Generating_Organic_Pull_Requests_via_Online_Repository_Memory]]：真实 maintainer 拒绝 PR 的根因常是缺乏 organicity。
- [[sources/Code_Review_Agent_Benchmark]]：review agents 只能发现部分人类提出的问题。
- [[sources/GLM_4_5_Agentic_Reasoning_and_Coding_ARC_Foundation_Models]]：通用 ARC benchmark 高分并不直接说明真实工作流可靠性。

### Challenging
- Not explicitly stated

### Mixed / Inconclusive
- 当前来源对“是模型能力不足，还是 context / workflow 设计不足”尚无统一结论。

## 5. Current State of Understanding
- What seems supported: 真实世界任务比 benchmark 更依赖 repository context、cross-file reasoning、human preferences。
- What seems unsupported: 当前没有一个单一因素可以解释全部失败。
- What is still unclear: 代码阅读、工具使用、记忆机制、review 对齐中哪一项最关键。
- What may be overclaimed in the literature: 我的解释：把 benchmark score 直接映射成 real-world software engineering capability，风险很大。

## 6. My Current Hypothesis
- Main hypothesis: 我的解释：agentic coding 的主要瓶颈不是单点编码能力，而是 repository adaptation、cross-file coherence 和 human workflow alignment。
- Alternative hypothesis: 我的解释：更大的 foundation model 就足以解决大多数问题。
- Confidence level: medium
- Why I currently think so: 我的解释：FeatureBench、Learning to Commit、c-CRAB 都指向 workflow/context 层问题。

## 7. Missing Evidence
- Missing datasets: 更多真实 PR / feature development / review datasets。
- Missing baselines: repository-adaptive baselines。
- Missing metrics: human acceptance、organicity、maintainer satisfaction。
- Missing real-world validation: 持续部署和长期维护结果。
- Missing causal explanation: 哪类上下文缺失最致命。
- Missing failure analysis: 跨任务失败模式统一归纳。

## 8. Candidate Next Steps
- Read: 上述四篇 sources
- Compare: [[sources/FeatureBench_Benchmarking_Agentic_Coding_for_Complex_Feature_Development]] vs [[sources/Learning_to_Commit_Generating_Organic_Pull_Requests_via_Online_Repository_Memory]]
- Experiment: 引入 repository memory / stronger tools / code reading constraints 的 controlled study
- Verify: benchmark 分数与真实 maintainer acceptance 的相关性
- Build dataset / benchmark: 更真实的 repository-adaptive benchmark
- Run ablation / stress test: 去掉 memory、去掉 code reading、去掉 history，对比性能退化

## 9. Links to My Research
- Why this question matters for my thesis/project: 我的解释：它决定你研究 agent 时是在做“更强模型”还是“更真实工作流”。
- What kind of contribution may be possible: 我的解释：提出新的 benchmark、memory mechanism 或 workflow-aware evaluation。
- What would count as a useful answer: 我的解释：能定位真实瓶颈，而不是只知道“分数低”。

## 10. Linked Pages
- [[sources/Code_Review_Agent_Benchmark]]
- [[sources/FeatureBench_Benchmarking_Agentic_Coding_for_Complex_Feature_Development]]
- [[sources/Learning_to_Commit_Generating_Organic_Pull_Requests_via_Online_Repository_Memory]]
- [[sources/GLM_4_5_Agentic_Reasoning_and_Coding_ARC_Foundation_Models]]
- [[concepts/ai_coding_agents]]
- [[concepts/agentic_coding_benchmarks]]
- [[concepts/code_review]]

## 11. Open Questions
- repository history 和记忆机制能补掉多少 real-world gap？
- 真实 maintainer 接受一个 PR 的决定因素中，功能正确性占多大比重？

---

## Extraction Notes
- Distinguish clearly between source-supported evidence and my interpretation.

