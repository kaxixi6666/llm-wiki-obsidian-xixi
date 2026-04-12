---
created: 2026-04-08T14:41
updated: 2026-04-12T16:20
type: guide
tags:
  - schema
  - wiki
  - knowledge-management
  - paper-reading
  - research
  - anti-hallucination
  - git
summary: "面向论文学习、研究积累与可复用比较分析的个人 wiki schema；真实性优先，支持结构化论文抽取、研究问题沉淀与 schema 自动版本管理"
---

# Wiki Schema for Paper Learning and Research

## 0. 目标与边界

> [!info] 核心目标
> 维护 `wiki/` 目录，将其打造为**可复利的研究知识层**，帮助我系统学习论文、积累研究问题、比较方法，并逐步形成自己的研究判断。

- **目标**：
  - 维护本仓库中的 `wiki/` 目录，把它变成一个可复利的研究知识层
  - 不只是记录论文内容，还要帮助我：
    - 理解论文在解决什么问题
    - 抽取方法、实验与证据
    - 识别局限性与隐藏风险
    - 追踪未来研究方向
    - 提取关键参考文献与知识脉络
    - 沉淀与我自己课题相关的研究问题、比较和实验想法

- **边界**：
  - 原始资料（`raw/`）是唯一事实来源，**只读不改**
  - 只在 `wiki/` 中创建、修改 Markdown 页面
  - 不要修改其它目录，除非明确属于 schema 版本管理或日志更新
  - 对原文不确定时，必须明确标记，不要编造

---

## 0.1 真实性优先原则（Anti-Hallucination Policy）

> [!warning] First rule
> Never fabricate. If the source does not clearly support a claim, say so explicitly and keep the statement uncertain.

> [!warning] 核心原则
> 不知道就是不知道。不要猜，不要补，不要把推测写成事实。

- 所有内容必须以 `raw/` 中可验证的信息为依据
- 若原文没有明确说明，就不要擅自补全
- 若信息不足，必须明确写出：
  - `Not explicitly stated`
  - `Insufficient evidence`
  - `Needs verification`
  - `I don't know based on the current source`
- 不允许：
  - 编造作者观点
  - 编造实验设置、数据集、指标、结果
  - 编造 future work
  - 编造参考文献内容
  - 把常识性推测写成论文原文事实
- 可以做推断，但必须显式标注为：
  - `My interpretation`
  - `Possible inference`
- 当原文表述模糊、缺页、OCR 不完整、图表难以辨认时，优先保守，不要强行总结

---

## 0.2 执行优先级

当“完整性”与“真实性”冲突时，永远优先真实性。

- 宁可少写，不可胡写
- 宁可留空，不可伪造
- 宁可标注 uncertain，不可装作确定
- 不允许为了“填满模板”而猜测内容

---

## 1. 目录结构约定

### 原始资料层
- `raw/`：原始资料（PDF、网页 Markdown、图片等），**只读**

### Wiki 维护层
`wiki/` 由你维护，建议包含以下子目录：

| 目录 | 用途 |
|------|------|
| `wiki/sources/` | 单篇论文 / 单个来源的结构化摘要页 |
| `wiki/concepts/` | 方法、理论、模型、术语等概念页 |
| `wiki/entities/` | 人物、作者、数据集、工具、项目、机构、benchmark、模型等实体页 |
| `wiki/research_questions/` | 研究问题页，用于沉淀某个长期追踪的问题 |
| `wiki/comparisons/` | 两篇或多篇论文 / 方法 / 数据集的比较页 |
| `wiki/experiments/` | 我的实验想法、设计草案、验证方案 |
| `wiki/overview/` | 某个主题的综述、综合总结、阶段性理解 |
| `wiki/templates/` | 页面模板（可选） |

### 根目录文件
- `wiki/index.md`：wiki 索引页
- `wiki/log.md`：操作日志
- `wiki/reading_queue.md`：待读论文清单（可选）
- `wiki/glossary.md`：高频术语表（可选）
- `wiki/schema.md`：当前 schema 文件本体（推荐）

---

## 2. 页面类型与基本格式

所有 wiki 页面使用 Markdown，并包含 frontmatter。

### 2.0 通用 frontmatter 模板

```yaml
---
type: "source|entity|concept|research_question|comparison|experiment|overview"
title: ""
summary: ""
tags: []
sources: []
status: "seed|growing|stable"
updated: "2026-04-12"
---