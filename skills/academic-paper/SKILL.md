---
name: tcm-academic-paper
version: 1.0.0
description: Build transparent biomedical manuscript outlines and drafts from verified evidence, protocols, real analyses, and human-approved clinical research decisions.
---

# Academic Paper | 医学论文结构与写作

## 用途与输入

适用于临床论文、方法学论文、病例系列和综述草稿。写作前记录：研究问题、设计类型、目标期刊与报告规范、研究方案版本、伦理情况、可复核证据、真实统计输出及作者确认的主张。

**禁止**依据想象填入 Results、受试者流程、效应估计、P 值、CONSORT/STROBE 流程数字等。

## 顺序

1. **一句话问题**：明确人群、主要暴露/干预、对照、结局、时间和意义。
2. **论证骨架**：背景 → 现有证据 → 不足与冲突 → 研究目的 → 预期贡献；每段配对应的证据 ID。
3. **方法先行**：按适当报告规范（例如观察性研究 STROBE、随机试验 CONSORT、预测模型 TRIPOD+AI，具体版本先核验）组织 Methods；核对主要终点、缺失值、混杂策略和敏感性分析。
4. **结果来源锁定**：仅以研究者提交且可复核的数据/图表为依据；缺数据用 `[待填写：真实分析结果]`。
5. **讨论与约束**：按主要发现、相关文献对照、可能机制、偏倚、临床意义、局限、后续研究编排。
6. **一致性检查**：摘要/正文/图表/补充材料数值、单位、定义和引用逐一匹配。

## 建议文件

```text
manuscript/
  00_question_and_claims.md
  01_outline.md
  02_source_map.csv
  03_methods_draft.md
  04_results_placeholders.md
  05_discussion_draft.md
  06_integrity_checks.md
```

## 学术诚信关口

- 标题/摘要不得夸大因果性、临床预测效力或外部推广性。
- 每个重要结论能追溯到真实数据或已核验文献。
- 统计方法、表格与图注需与真实分析完全一致。
- AI 不能捏造被试引言、伦理审批、基金资助声明、临床试验注册号或作者贡献。
- 投稿前由所有负责人员完成确认；AI 工具使用披露遵照目标期刊现行要求。

输出：写作计划、带证据标注的段落草案、信息缺口和最终人工核查清单。
