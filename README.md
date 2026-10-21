# TCM Clinical Research Skills | 中医临床科研 AI Skills

> **Version:** v1.0.0 · **Language:** 中文优先 / English metadata · **Status:** reusable prompt-based workflows (not validated software)

用于中医及中西医结合临床科研的、由研究者审核的 AI 工作流程。以**证据可追溯、统计方法恰当、患者隐私保护、人工最终判断**为核心原则。适用于临床观察性研究、临床试验方案准备、医学论文、基金申报与系统综述的准备工作。

**This repository provides portable instruction files, not autonomous literature-search or clinical decision-making software.** Results depend on the AI client's available tools, source access, and human review.

## Skills

| Skill | 解决什么问题 | 输出 |
|---|---|---|
| [Deep Research](skills/deep-research/SKILL.md) | 结构化检索、证据分级和研究空白定位 | 可复现检索式、证据矩阵、核验记录 |
| [Academic Paper](skills/academic-paper/SKILL.md) | 从研究问题到医学论文初稿 | 论文逻辑图、IMRaD 章节、来源映射 |
| [Academic Reviewer](skills/academic-reviewer/SKILL.md) | 临床、方法学、统计和学术诚信的模拟审查 | 分级问题清单、修订记录 |

另提供 [统一科研规则](SKILL.md)、[质量闸门](docs/QUALITY_GATES.md) 与 [隐私及医学安全规范](docs/SAFETY_AND_PRIVACY.md)。

## 5 分钟开始

1. 阅读 [SKILL.md](SKILL.md) 确认通用科研原则。
2. 在支持自定义指令 / Skills 的 AI 环境中加载所需的 `skills/<name>/SKILL.md`；不同客户端的自动发现与触发规则不同。
3. 描述您的研究问题和**已有的、可分享的非敏感资料**，例如“研究对象、研究类型、终点、希望得到的交付物”。
4. 参考 [examples/QUICKSTART.md](examples/QUICKSTART.md) 的命令范例逐阶段使用。
5. 由研究者检查原文、数据、伦理和统计判断后才用于正式研究。

**示例：**

```text
请读取 skills/deep-research/SKILL.md 并按它执行。
课题：某中医证候量表的测量学评价（教学假设场景）。
交付：PECO/研究问题、PubMed 检索式草案、待核验的证据矩阵、潜在偏倚。
如果没有真实检索工具，请明确说明，不能伪造已检索的文章。
```

## 仓库结构

```text
TCM-Clinical-Research-Skills/
├── SKILL.md
├── skills/
│   ├── deep-research/SKILL.md
│   ├── academic-paper/SKILL.md
│   └── academic-reviewer/SKILL.md
├── docs/
│   ├── QUALITY_GATES.md
│   └── SAFETY_AND_PRIVACY.md
├── examples/QUICKSTART.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── LICENSE
└── README.md
```

## 使用边界

- **不要上传**患者姓名、完整出生日期、电话、证件号、影像 DICOM 原始标识等可识别信息，或未经授权的院内资料。
- 不得伪造文献、DOI/PMID、伦理批件、临床试验注册、样本量、分析结果或审稿决定。
- 未进行实际检索时，应将“推荐检索式”和“已完成检索”严格区分。
- AI 模拟审稿不是正式同行评审，也不能取代临床研究者、统计人员、伦理委员会与期刊审核。

## 项目来源与许可

这套说明文件为本项目独立编写的工作流，受公开的学术 AI 工作流思想启发，包括：

- [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills)
- [HKUSTDial/Supervisor-Skills](https://github.com/HKUSTDial/Supervisor-Skills)

未复制上述项目的源代码、提示词文件或其受许可约束的内容。该项目自身原创内容采用 [MIT License](LICENSE)；引用、复用外部项目内容须分别遵守其原有许可。

欢迎提交 Issue 或 Pull Request。任何改动应优先提升证据可核验性、临床科研方法透明性和使用安全性。

## Related Skill: Investment Monitor

本仓库另含独立的投资监控工作流，覆盖 BTC/ETH、黄金、纳斯达克100与标普500、国内宽基/A股、债券及宏观风险观察。它采用官方来源优先、重要信息交叉核验、指标计算透明、允许“观望”的原则。

- [Investment Monitor Skill](skills/investment-monitor/README.md)
- [Core instructions](skills/investment-monitor/SKILL.md)
- [Example configuration](skills/investment-monitor/config.example.yaml)
- [Daily report template](skills/investment-monitor/examples/daily-report-template.md)
- [Privacy checklist](skills/investment-monitor/PRIVACY.md)

该 Skill 是通用的信息整理与决策辅助工作流，不是实时行情服务、自动交易程序或收益保证。请勿在公开仓库中提交个人资产、账户、交易记录或密钥。
