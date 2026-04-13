---
type: source
title: "FeatureBench: Benchmarking Agentic Coding for Complex Feature Development"
summary: "论文提出 FeatureBench，用于评估 agentic coding 在复杂 feature development 场景中的能力，并显示当前强模型在该 benchmark 上的成功率远低于 SWE-bench。"
tags: [paper, benchmark, agentic-coding, feature-development]
sources: ["raw/research_papers/first/FeatureBench- Benchmarking Agentic Coding for Complex Feature Development.pdf"]
status: growing
updated: "2026-04-12"
---

# FeatureBench: Benchmarking Agentic Coding for Complex Feature Development

## 1. Paper Metadata
- Title: 作者明确写出：FeatureBench: Benchmarking Agentic Coding for Complex Feature Development
- Authors: Needs verification
- Venue: 作者明确写出：Published as a conference paper at ICLR 2026
- Year: 作者明确写出：2026
- DOI / URL: 作者明确写出：Code / Dataset / ProjectPage links 存在；正式 DOI 未确认
- Source File: 本地路径说明：`raw/research_papers/first/FeatureBench- Benchmarking Agentic Coding for Complex Feature Development.pdf`
- Reading Status: semi-deep

## 2. Research Problem
- Problem: 作者明确写出：现有 agentic coding benchmarks 多聚焦 bug fixing 或单 PR 场景，难以覆盖 end-to-end、feature-oriented development。
- Why this problem matters: 作者明确写出：随着 agent 被用于真实开发，需要评估其复杂 feature development 的边界。
- Gap in prior work: 作者明确写出：现有 benchmarks task scope 有限，且 often rely on non-executable evaluations 或缺少可持续更新机制。
- Target scenario / domain: 作者明确写出：end-to-end, feature-oriented software development。

## 3. Core Idea / Contribution
- High-level idea: 作者明确写出：提出 FeatureBench，采用 execution-based evaluation 与 test-driven task derivation。
- Claimed contributions: 作者明确写出：构建 200 challenging tasks 和 3825 executable environments，来自 24 repositories。
- What is novel compared with prior work: 作者明确写出：从 unit tests 沿 dependency graph 追踪，自动提取 feature-level tasks。
- My one-sentence understanding: 我的解释：这篇论文想把 agentic coding 的评估从“修一个 bug”推进到“真正做一个复杂 feature”。

## 4. Method / Design
- Input: 作者明确写出：open-source repositories、unit tests、dependency graph。
- Output: 作者明确写出：feature-level coding tasks 与 executable evaluation environments。
- Pipeline / framework: 作者明确写出：test-driven method，从 unit tests 沿 dependency graph 自动识别跨 commits / PRs 的 feature tasks。
- Key components: 作者明确写出：FeatureBench，execution-based protocol。
- Key assumptions: 作者明确写出：该方法能在最小人工成本下分离出可执行 feature tasks。
- Notation / terms worth remembering: 作者明确写出：FeatureBench。

## 5. Experiment Setup
- Dataset(s): 作者明确写出：200 tasks，3825 executable environments，24 repositories。
- Baseline(s): 作者明确写出：比较 state-of-the-art agentic model，例如 Claude 4.5 Opus。
- Metrics: 作者明确写出：resolved rate。
- Evaluation protocol: 作者明确写出：在 benchmark tasks 上做 end-to-end evaluation。
- Implementation details (if important): 作者明确写出：execution-based evaluation。
- Reproducibility notes: 作者明确写出：Code, Dataset, ProjectPage 提供。

## 6. Results
- Main findings: 作者明确写出：当前 SOTA agentic model 在该 benchmark 上成功率很低。
- Quantitative improvements: 作者明确写出：Claude 4.5 Opus 在 SWE-bench 上 74.4% resolved rate，但在 FeatureBench 上只有 11.0%。
- Qualitative findings: 作者明确写出：当前模型在跨文件依赖解析和程序上下文保持上仍有明显困难。
- What evidence is actually convincing: 作者明确写出：benchmark 使用 executable environments，且任务来自真实 repositories。
- What evidence is weak / insufficient: Needs verification：完整模型列表与分项失败类型统计未在当前抽取中完全恢复。

## 7. Limitations
### Authors' Stated Limitations
- 作者明确写出：当前 LLM 在 cross-file dependency resolution 上仍有明显限制。
- 作者明确写出：模型存在“laziness”，会猜测跨文件组件接口或属性，而不是实际读取文件。

### My Observed Limitations
- 我的解释：当前 source 抽取到了 limitations 段，但未完整恢复全文结论段。

## 8. Hidden Risks / Unverified Risks
- What may still go wrong: 我的解释：benchmark 构造方法可能仍偏向某类 feature tasks。
- Does the evaluation miss important failure cases?: 我的解释：可能仍缺少更长周期、多开发者协作的 feature 流程。
- Is there a risk of “tests pass but system is still wrong”?: 我的解释：Yes，execution-based benchmark 也未必覆盖所有 UX / architecture 约束。
- Possible threats to reliability / validity: 我的解释：NameError / AttributeError 只是失败外显结果，不一定解释根因。
- What should have been checked but was not: Needs verification

## 9. Relevance to My Research
- Relation to my topic: 我的解释：如果研究 agentic coding 的真实开发能力，这篇论文高度相关。
- Useful ideas I can borrow: 我的解释：从 unit tests + dependency graph 自动构造 feature-level benchmark。
- Possible experiment inspired by this paper: 我的解释：将 feature development benchmark 与 repository memory 方法结合。
- Whether it supports / challenges my current hypothesis: 我的解释：支持“当前 agent 在复杂 feature development 上远未达到 bug-fix benchmark 所显示的水平”。
- Priority for future revisit: high

## 10. Future Work
### Authors' Suggested Future Work
- Needs verification

### Future Work Type
- [x] more data
- [x] more domains
- [ ] stronger baseline
- [x] better evaluation
- [x] robustness / reliability
- [ ] real-world deployment
- [ ] human study
- [ ] interpretability
- [ ] causal explanation
- [ ] efficiency / scalability
- [x] other: feature-level task construction

### My Interpretation
- 我的解释：FeatureBench 更像是一个平台型 benchmark，后续关键在持续扩展任务覆盖面。

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
- [[concepts/agentic_coding_benchmarks]]
- [[concepts/ai_coding_agents]]

## 13. Linked Entities
- Needs verification

## 14. Linked Research Questions
- [[research_questions/What_limits_real_world_agentic_coding]]

## 15. Notes / Quotes
- 作者明确写出：Claude 4.5 Opus succeeds on only 11.0% of FeatureBench tasks.

## 16. Open Questions
- FeatureBench 与 repository-scale PR benchmarks 的难度差异主要来自哪里？
- “laziness” 是模型问题、工具问题，还是任务设定问题？

---

## Extraction Notes
- Only write claims supported by the source.
