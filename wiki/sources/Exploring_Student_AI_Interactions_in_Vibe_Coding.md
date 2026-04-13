---
type: source
title: "Exploring Student-AI Interactions in Vibe Coding"
summary: "论文通过 think-aloud 观察学生在 Replit 上进行 vibe coding 的过程，分析不同编程背景学生如何提示、测试、调试以及与代码交互。"
tags: [paper, vibe-coding, education, human-ai-interaction]
sources: ["raw/research_papers/third/Exploring Student-AI Interactions in Vibe Coding.pdf"]
status: growing
updated: "2026-04-12"
---

# Exploring Student-AI Interactions in Vibe Coding

## 1. Paper Metadata
- Title: 作者明确写出：Exploring Student-AI Interactions in Vibe Coding
- Authors: 作者明确写出：Francis Geng, Anshul Shah, Haolin Li, Nawab Mulla, Steve Swanson, Gerald Soosai Raj, Daniel Zingaro, Leo Porter
- Venue: 作者明确写出：February 9-13, 2026, VIC, Melbourne, Australia；会议名 Needs verification
- Year: 作者明确写出：2026
- DOI / URL: Not explicitly stated
- Source File: 本地路径说明：`raw/research_papers/third/Exploring Student-AI Interactions in Vibe Coding.pdf`
- Reading Status: semi-deep

## 2. Research Problem
- Problem: 作者明确写出：希望理解不同背景学生如何在 vibe coding 平台上构建软件，并比较交互差异。
- Why this problem matters: 作者明确写出：vibe coding 可能进一步改变学生编程方式。
- Gap in prior work: 作者明确写出：现有工作主要关注 expert/professional programmers，对学生 vibe coding 的理解不足。
- Target scenario / domain: 作者明确写出：introductory programming 和 advanced software engineering classes 中的学生使用 Replit 构建 web application。

## 3. Core Idea / Contribution
- High-level idea: 作者明确写出：通过 think-aloud、screen recordings、prompts、code changes 和 error logs 做 qualitative coding。
- Claimed contributions: 作者明确写出：构建 interaction labeling schema，刻画 prompting、testing、debugging 和 code engagement。
- What is novel compared with prior work: 我的解释：该研究把 vibe coding 放到 CS education 里做细粒度交互观察。
- My one-sentence understanding: 我的解释：这篇论文关注学生在 vibe coding 中到底“怎么和 AI 一起编程”。

## 4. Method / Design
- Input: 作者明确写出：students、Replit、think-aloud、screen recordings、prompts、code changes、error logs。
- Output: 作者明确写出：interaction labeling schema 与行为模式分析。
- Pipeline / framework: 作者明确写出：qualitative coding。
- Key components: 作者明确写出：Replit；intro vs advanced student groups。
- Key assumptions: 作者明确写出：学生的可观察交互可以反映 vibe coding 行为模式。
- Notation / terms worth remembering: 作者明确写出：closed-box testing；prompting to debug。

## 5. Experiment Setup
- Dataset(s): 作者明确写出：参与者来自两门 computing courses。
- Baseline(s): 作者明确写出：比较 introductory 与 advanced students。
- Metrics: Not explicitly stated
- Evaluation protocol: 作者明确写出：participants think-aloud while building a web app using Replit。
- Implementation details (if important): 作者明确写出：qualitatively coded artifacts。
- Reproducibility notes: Not explicitly stated

## 6. Results
- Main findings: 作者明确写出：两组学生的大部分交互都集中在测试常见情况和通过 prompts 调试；很少手动分析或编辑代码。
- Quantitative improvements: Not explicitly stated
- Qualitative findings: 作者明确写出：advanced students 更可能在 prompts 中包含相关 app features 和 codebase context，更可能与代码库交互。
- What evidence is actually convincing: 作者明确写出：结合 think-aloud 与多种交互产物做 qualitative analysis。
- What evidence is weak / insufficient: Needs verification：样本量与编码协议细节需完整复核。

## 7. Limitations
### Authors' Stated Limitations
- 作者明确写出：单一北美高校、两门课程、voluntary participation 可能引入 self-selection bias。
- 作者明确写出：研究完全基于 Replit，平台特性限制了结果的普适性。

### My Observed Limitations
- 我的解释：教育场景结果不应直接外推到专业开发者。

## 8. Hidden Risks / Unverified Risks
- What may still go wrong: 我的解释：学生行为可能受实验任务和观察环境影响。
- Does the evaluation miss important failure cases?: 我的解释：可能遗漏长期学习效果与能力迁移。
- Is there a risk of “tests pass but system is still wrong”?: 我的解释：Yes，尤其当学生主要做 closed-box testing 时。
- Possible threats to reliability / validity: 作者明确写出：self-selection bias 与 platform specificity。
- What should have been checked but was not: 我的解释：跨平台、跨学校、长期跟踪。

## 9. Relevance to My Research
- Relation to my topic: 我的解释：如果你对 vibe coding 中的人机协作与能力变化感兴趣，这篇论文高度相关。
- Useful ideas I can borrow: 我的解释：用 interaction labeling schema 观察 prompting / testing / debugging。
- Possible experiment inspired by this paper: 我的解释：比较学生、初级开发者、专业开发者在 vibe coding 中的行为差异。
- Whether it supports / challenges my current hypothesis: 我的解释：支持“测试和调试在 AI 时代依旧关键，而且 prompt 能力差异显著”。
- Priority for future revisit: high

## 10. Future Work
### Authors' Suggested Future Work
- 作者明确写出：扩展到 multiple institutions and course settings would strengthen applicability。

### Future Work Type
- [x] more data
- [x] more domains
- [ ] stronger baseline
- [ ] better evaluation
- [ ] robustness / reliability
- [ ] real-world deployment
- [x] human study
- [ ] interpretability
- [ ] causal explanation
- [ ] efficiency / scalability
- [x] other: multi-platform replication

### My Interpretation
- 我的解释：后续关键在跨平台、跨背景、跨时间的学生行为研究。

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

## 13. Linked Entities
- Needs verification

## 14. Linked Research Questions
- [[research_questions/What_limits_real_world_agentic_coding]]

## 15. Notes / Quotes
- 作者明确写出：the bulk of student interactions with Replit are closed box testing and prompting to debug.

## 16. Open Questions
- 学生使用 vibe coding 后，代码理解能力会怎样变化？
- prompt sophistication 的差异能否通过教学显著缩小？

---

## Extraction Notes
- Only write claims supported by the source.

