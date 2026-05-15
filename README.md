# Web UI/UX Design Master OS

> 一份为 Claude Code 蒸馏的 **Web UI/UX 设计行业操作系统** —— 覆盖 220+ 来源、14 位关键人物、72 款工具、92 条术语、7 维 agentic 协议，帮你从零到专业设计师思维。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Version](https://img.shields.io/badge/version-1.0-blue.svg)](./meta.json)
[![Sources](https://img.shields.io/badge/sources-220%2B-green.svg)](./references/)
[![Claude Code](https://img.shields.io/badge/host-Claude%20Code-purple.svg)](https://claude.ai/code)
[![Generator](https://img.shields.io/badge/generator-master--skill%20v0.6-orange.svg)](https://github.com/voidborne-d/master-skill)

---

## 这是什么

本 skill 由 [master-skill](https://github.com/voidborne-d/master-skill) 框架生成，是一份可装载到 Claude Code 的**行业知识 OS**。装载后，Claude 会以资深 UI/UX 设计师的思维模式回答你的设计问题——从组件粒度的取舍到系统级的信息架构决策。

### 核心内容

| 维度 | 数量 | 说明 |
|------|------|------|
| 研究来源 | 220+ | 60% 一手资料（官方文档/演讲/采访） |
| 关键人物 | 14 人 | Norman、Frost、Wathan 等行业定义者 |
| 工具覆盖 | 72 款 | 含决策树：何时用 Figma vs Framer vs 代码 |
| 术语表 | 92 条 + 12 项标准 + 7 项法规 | 含 WCAG / EN 301 549 / ADA |
| 经典书单 | 38 本 | 含精读优先级标注 |
| 社区/Newsletter | 42 个 | 持续跟踪信息源 |
| 心智模型 | 5 个 | 设计师决策底层逻辑 |
| Playbook 规则 | 8 条 | 可执行的行业最佳实践 |
| Agentic 协议维度 | 7 个 | AI 辅助设计工作流规范 |

---

## 安装

```bash
# 克隆到 Claude Code skills 目录
git clone https://github.com/Maropion03/web-uiux-design-master.git \
  ~/.claude/skills/web-uiux-design-master
```

无需额外配置。Claude Code 会在对话中自动检测并激活 skill。

---

## 触发方式

以下关键词会自动激活 skill：

**英文：** `UI design` · `UX design` · `interaction design` · `design system` · `design tokens` · `usability` · `wireframe` · `prototype` · `accessibility` · `a11y` · `WCAG` · `Figma` · `shadcn` · `Tailwind` · `atomic design` · `affordance` · `user research` · `design critique`

**中文：** `信息架构` · `设计系统` · `设计评审`

---

## CLI 工具树

skill 自带可执行的 bash 工具，可独立运行，无需 Claude：

```bash
# 7 维 agentic 协议参考
bash cli/protocol/agentic.sh --help
bash cli/protocol/agentic.sh --json      # JSON 输出，供脚本消费
bash cli/protocol/agentic.sh --explain   # 展开每维度说明

# 工具选择决策树
bash cli/decision/figma.sh              # Figma vs Framer vs 代码？
bash cli/decision/component.sh          # 组件拆分粒度决策
bash cli/decision/data.sh               # 数据密集 UI / 信息架构
bash cli/decision/general-playbook.sh   # 通用 playbook 速查
```

---

## 目录结构

```
web-uiux-design-master/
├── SKILL.md                        # 主技能文件（Claude Code 装载入口）
├── meta.json                       # 机器可读元数据
├── README.md                       # 本文件
├── LICENSE                         # MIT
│
├── cli/                            # 可执行 bash CLI 工具树
│   ├── protocol/
│   │   └── agentic.sh              # 7 维 agentic 协议
│   ├── decision/
│   │   ├── figma.sh                # 工具选择决策树
│   │   ├── component.sh            # 组件/DS 决策树
│   │   ├── data.sh                 # 数据/IA 决策树
│   │   └── general-playbook.sh     # 通用 playbook
│   ├── lib/
│   │   └── common.sh               # 共享 helper
│   └── README.md
│
├── references/
│   ├── synthesis.md                # 行业 OS 综合提炼（17K）
│   └── research/
│       ├── 01-figures.md           # 14 位关键人物（93% 一手 URL）
│       ├── 02-tools.md             # 72 款工具
│       ├── 03-workflows.md         # 7 大方法论 + 5 个工作流变化
│       ├── 04-canon.md             # 38 本经典书单
│       ├── 05-sources.md           # 42 个社区/Newsletter/播客/会议
│       ├── 06-glossary.md          # 92 术语 + 12 标准 + 7 法规
│       └── seeds/                  # Wave 1 研究种子（RSS/GitHub）
│
└── sub-skills/                     # Person sub-skills（待补全，见下方）
```

---

## Sub-skills 状态

以下 3 位人物的 person sub-skill 因 API 限额在生成时中断，计划补全：

| Figure | Slug | 状态 |
|--------|------|------|
| Don Norman | `don-norman` | ⚠️ 待补全 |
| Brad Frost | `brad-frost` | ⚠️ 待补全 |
| Adam Wathan | `adam-wathan` | ⚠️ 待补全 |

补全方法（需安装 [nuwa-skill](https://github.com/alchaincyf/nuwa-skill)）：

```bash
# 在 Claude Code 中执行
/master-skill 补全 web-uiux-design-master 的 sub-skills
```

---

## 知识衰减周期

| 轨道 | 建议更新频率 |
|------|------------|
| 工具 (02) | 3–6 个月 |
| 工作流 (03) | 3–6 个月 |
| 心智模型 | 1–2 年 |
| 经典书单 | 1–2 年 |

---

## 生成方式

本 skill 由 [master-skill v0.6](https://github.com/voidborne-d/master-skill) 框架通过以下流程生成：

1. **Phase 1** — 行业定义 + 受众画像 intake
2. **Phase 2** — 6 轨并行研究（figures / tools / workflows / canon / sources / glossary），Wave 1→2→3 依赖拓扑
3. **Phase 3** — 综合提炼 → SKILL.md 写入 → CLI 工具树生成
4. **Phase 4** — 结构验证（`skill_writer.py validate: true`）+ 自检通过
5. **Phase 5** — 双 agent 精炼（部分延期）

研究数据收集于 2026-05-12，110 条 RSS 条目 + 22 个 GitHub 仓库作为种子。

---

## License

[MIT](./LICENSE) © 2026 Maropion03
