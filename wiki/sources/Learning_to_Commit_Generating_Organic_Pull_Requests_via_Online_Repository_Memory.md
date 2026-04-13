---
type: source
title: "Learning to Commit: Generating Organic Pull Requests via Online Repository Memory"
summary: "论文提出 Learning to Commit，通过 Online Repository Memory 从历史 commits 中蒸馏 repository-specific skills，提升生成 PR 的 organicity。"
tags: [paper, pull-requests, repository-memory, ai-coding-agents]
sources: ["raw/research_papers/third/Learning to Commit- Generating Organic Pull Requests via Online Repository Memory.pdf"]
status: growing
updated: "2026-04-12"
---

# Learning to Commit: Generating Organic Pull Requests via Online Repository Memory

## 1. Paper Metadata
- Title: 作者明确写出：Learning to Commit: Generating Organic Pull Requests via Online Repository Memory
- Authors: 作者明确写出：Mo Li, L.H. Xu, Qitai Tan, Ting Cao, Yunxin Liu
- Venue: Needs verification
- Year: Needs verification
- DOI / URL: Not explicitly stated
- Source File: 本地路径说明：`raw/research_papers/third/Learning to Commit- Generating Organic Pull Requests via Online Repository Memory.pdf`
- Reading Status: semi-deep

## 2. Research Problem
- Problem: 作者明确写出：LLM-based coding agents 虽然在 benchmark 上表现好，但生成的 PR 往往缺乏“organicity”，因此被真实维护者拒绝。
- Why this problem matters: 作者明确写出：问题不只是 functional incorrectness，而是忽略 project-specific conventions、internal APIs 和隐式架构约束。
- Gap in prior work: 作者明确写出：仅暴露 repository snapshot 不够，因为 snapshot 不反映 repository-specific change patterns。
- Target scenario / domain: 作者明确写出：真实仓库中的 pull request generation。

## 3. Core Idea / Contribution
- High-level idea: 作者明确写出：提出 Learning to Commit，通过 Online Repository Memory 从历史 commits 反思并积累 skills。
- Claimed contributions: 作者明确写出：让 agent 从 repository evolution 中学习 style、internal API usage、architectural invariants。
- What is novel compared with prior work: 作者明确写出：用 strict chronological split，让 agent 在 earlier commits 上做 supervised contrastive reflection 并积累可复用 skills。
- My one-sentence understanding: 我的解释：这篇论文想让 agent 不只是“会写代码”，而是“写得像这个仓库的人”。

## 4. Method / Design
- Input: 作者明确写出：repository with strict chronological split，historical issues / commits。
- Output: 作者明确写出：带有 Online Repository Memory 的 PR generation framework。
- Pipeline / framework: 作者明确写出：blindly attempt historical issue；compare prediction against oracle diff；distill gap into skills；new PR 时基于这些 skills 生成。
- Key components: 作者明确写出：Online Repository Memory，contrastive reflection，skills。
- Key assumptions: 作者明确写出：repository 的历史演化能显式提供 project-specific coding patterns。
- Notation / terms worth remembering: 作者明确写出：Learning to Commit, Online Repository Memory, organicity。

## 5. Experiment Setup
- Dataset(s): 作者明确写出：evaluation 在 expert-maintained repository with rich commit history 上进行。
- Baseline(s): Needs verification
- Metrics: 作者明确写出：functional correctness, code-style consistency, internal API reuse rate, modified-region plausibility。
- Evaluation protocol: 作者明确写出：在 genuinely future, merged pull requests 上评估。
- Implementation details (if important): 作者明确写出：strict chronological split。
- Reproducibility notes: Not explicitly stated

## 6. Results
- Main findings: 作者明确写出：historical adaptation improves file localisation, reduces patch bloat, and improves organicity on future tasks。
- Quantitative improvements: Needs verification
- Qualitative findings: 作者明确写出：repository memory helps align generated contributions with expert maintainers' expectations。
- What evidence is actually convincing: 作者明确写出：evaluation on genuinely future merged PRs。
- What evidence is weak / insufficient: Needs verification：当前抽取未恢复完整实验表格与多仓库范围。

## 7. Limitations
### Authors' Stated Limitations
- Needs verification

### My Observed Limitations
- 我的解释：当前证据看起来依赖单个或少量高质量仓库，外部泛化性需要复核。

## 8. Hidden Risks / Unverified Risks
- What may still go wrong: 我的解释：历史 memory 可能固化 repository 中已有的次优模式。
- Does the evaluation miss important failure cases?: 我的解释：可能遗漏多维护者冲突和快速演化仓库场景。
- Is there a risk of “tests pass but system is still wrong”?: 我的解释：Yes，organicity 与长期可维护性仍不是同一件事。
- Possible threats to reliability / validity: 我的解释：若只在少数仓库验证，结果可能过拟合于特定 repo culture。
- What should have been checked but was not: Needs verification

## 9. Relevance to My Research
- Relation to my topic: 我的解释：如果研究 repository-adaptive agents、PR generation 或 human preference alignment，这篇论文高度相关。
- Useful ideas I can borrow: 我的解释：通过历史 commits 蒸馏 repository-specific skills。
- Possible experiment inspired by this paper: 我的解释：将 repository memory 与 feature development benchmark 结合。
- Whether it supports / challenges my current hypothesis: 我的解释：支持“benchmark 成绩好不等于真实 PR organicity 高”。
- Priority for future revisit: high

## 10. Future Work
### Authors' Suggested Future Work
- 作者明确写出：As a foundational step, this work naturally opens several avenues for future research.
- Needs verification：具体 future work 条目在当前抽取片段中未完整恢复。

### Future Work Type
- [x] more data
- [x] more domains
- [ ] stronger baseline
- [x] better evaluation
- [x] robustness / reliability
- [x] real-world deployment
- [ ] human study
- [ ] interpretability
- [ ] causal explanation
- [ ] efficiency / scalability
- [x] other: repository adaptation

### My Interpretation
- 我的解释：后续重点应在跨仓库泛化与真实 maintainer acceptance。

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
- 作者明确写出：The root cause is not functional incorrectness but a lack of organicity.

## 16. Open Questions
- repository memory 在不同规模和文化的仓库中是否同样有效？
- “organicity” 能否被更稳定地量化？

---

## Extraction Notes
- Only write claims supported by the source.
