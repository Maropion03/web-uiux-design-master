# Track 03: Workflows — Web UI/UX Design

last_updated: 2026-05-12
locale: en + zh
methodology_count: 7
sop_step_count: 8
audience: 想入行 Web UI/UX 设计的中文学习者
信源原则：作者本人 talk / 一手书 / 官方页 / NN/g / Smashing 长稿；不引用知乎、微信公众号、百度、内容农场

> 这一轨回答一个问题：「这行的人一天到晚干什么？」
> 入门人 vs 资深人在同一个项目里走完一遍的差别在哪？
> 2024–2026 AI 工具浪潮把哪些步骤改写了？

---

## A. 入门 SOP：从「老板说要做个新功能页面」到「交付开发」

定义最小完整任务：一个产品经理找你「帮我们做个 X 功能的 web 页面」，你怎么走完整 8 步？
每步约 1–3 天（视团队节奏），新人完整跑完一遍大约 2–3 周。

---

### Step 1. Intake / 需求理解（kickoff）

**做什么**：与 PM / 业务方面对面（或异步文档）确认：
- 这个功能解决什么问题、为谁解决
- 成功指标是什么（转化？任务完成率？NPS？）
- 时间、范围、技术约束
- 已经存在的 design system / 品牌约束

**关键产出物**：
- Project brief（一页纸：问题陈述 + 用户 + 成功指标 + 约束）
- Kickoff meeting notes

**常用工具**：Notion / Confluence / FigJam（A6 sources） / Loom（异步视频）

**反模式**：
- 直接打开 Figma 开始画（最常见新人错误）
- 把"PM 说的需求"当真问题，跳过"为什么"的追问
- 不写下成功指标 → 后期争议无法仲裁

**信源**：Julie Zhuo, "Junior Designers vs. Senior Designers" — https://lookingglass.substack.com/ ；NN/g "Project Kickoff" articles — https://www.nngroup.com/

---

### Step 2. Research / 同理（discover 阶段）

**做什么**：
- Desk research：竞品 / 现有产品类比 / Mobbin 上找同类 pattern
- 用户访谈：5 人法（Jakob Nielsen 1993 提出「5 个用户足以发现 85% 可用性问题」）
- 数据查看：Hotjar / FullStory 现有数据；analytics
- Persona / Journey Map / Empathy Map（按需）

**关键产出物**：
- Research notes（Dovetail / Notion）
- 竞品扫描 board（FigJam / Miro）
- 1–3 个 problem statement（"用户在 X 场景下卡在 Y"）

**常用工具**：Mobbin (E1)、Page Flows (E2)、Dovetail (A5)、Maze (A5)、Lookback；中文圈 Pageflows 替代——直接录屏竞品

**反模式**：
- 跳过研究直接进设计（"我以为我知道用户想要什么"）
- 把 PM 给的 persona PPT 当研究结果用
- 研究做完，结论不影响设计决策（research theater）

**信源**：Nielsen 1993《Usability Engineering》5-user rule — https://www.nngroup.com/articles/why-you-only-need-to-test-with-5-users/ ；Jake Knapp《Sprint》Day 2 lightning talks

---

### Step 3. Explore / 发散（diverge）

**做什么**：
- 在纸上 / iPad / FigJam 上 sketch **多个**方案（最少 3 个，资深人常画 8–15 个 thumbnail）
- 画用户流程图（user flow）
- Lo-fi wireframe（灰度、无字体讲究、focus 结构）

**关键产出物**：
- 多方案 sketches（拍照 / 扫描）
- User flow（FigJam / Whimsical）
- Lo-fi wireframe（Figma 或纸）

**常用工具**：纸笔 / iPad + Procreate / FigJam / Whimsical / Excalidraw

**反模式**：
- 第一稿就开始上颜色 / 拼组件（hi-fi 病）
- 只画一个方案（无对比 = 无决策）
- Sketch 阶段就用 Figma 组件库——会被现成组件锁死想象力

**信源**：Jake Knapp《Sprint》(2016) Day 3 "Crazy 8s" — https://www.thesprintbook.com/ ；UK Design Council Double Diamond Discover→Develop — https://www.designcouncil.org.uk/our-resources/the-double-diamond/

---

### Step 4. Converge / 收敛与决策（define）

**做什么**：
- 把 3–8 个方案放在一起做 design critique
- 与 PM 对齐选 1–2 个方向深化
- 与开发 light touch 沟通技术可行性

**关键产出物**：
- 选定方向 + 决策理由文档
- Open questions list

**常用工具**：FigJam / Slack huddle / Loom 录屏让异步同事 critique

**反模式**：
- "老板拍板"——critique 退化成评分会
- 没有写下"为什么否决其他方案"，下次同样争论再来一次
- 收到非建设性反馈（"我觉得不好看"）后直接改，不追问"为什么"

**信源**：Adam Connor & Aaron Irizarry《Discussing Design》O'Reilly 2015 — https://www.oreilly.com/library/view/discussing-design/9781491902394/ ；Brad Frost "Design Critique" articles — https://bradfrost.com/blog/

---

### Step 5. Hi-fi 设计

**做什么**：
- 在 Figma 里用 design system 组件搭高保真稿
- 覆盖所有状态：default / hover / focus / disabled / loading / empty / error
- 响应式：mobile / tablet / desktop 三档
- Edge case：超长字符、0 数据、网络失败、权限不足

**关键产出物**：
- Figma file 含完整 frames + variants
- Annotation（重要交互逻辑 / 动效说明）

**常用工具**：Figma + 团队 design system + Tokens Studio + Stark a11y plugin

**反模式**：
- 只画 happy path（资深人会立刻问"loading 呢？空状态呢？错误呢？"）
- 忽略 a11y（对比度 / focus indicator / touch target ≥ 24×24）
- Pixel-perfect 但偏离已有 design system token → 后期 dev 复刻困难

**信源**：Refactoring UI by Adam Wathan & Steve Schoger — https://www.refactoringui.com/ ；Apple HIG — https://developer.apple.com/design/human-interface-guidelines/

---

### Step 6. Prototype + Validate

**做什么**：
- Figma Prototype 串接关键 flow（Smart Animate + Variables 已能覆盖 80%）
- 5 人可用性测试（remote unmoderated 用 Maze；moderated 用 Lookback / Google Meet 录屏）
- RITE 方法：测一个改一个

**关键产出物**：
- Clickable prototype
- 可用性测试报告（5 人 × 5 任务，task success rate + 主要 friction points）

**常用工具**：Figma prototype / Maze (A5) / Useberry / Lookback

**反模式**：
- 跳过验证直接交付（"等上线再看数据"——但数据无法告诉你"为什么"卡住）
- 找同事测——同事熟悉产品，结果失真
- 测了但不改——research theater 的 prototype 版

**信源**：NN/g "Why You Only Need to Test with 5 Users" — https://www.nngroup.com/articles/why-you-only-need-to-test-with-5-users/ ；Microsoft RITE Method (Medlock et al. 2002)

---

### Step 7. Handoff（交付开发）

**做什么**：
- Figma Dev Mode 整理 frame：分 ready-for-dev 状态、加 description、链接 tickets
- 标注关键交互逻辑（动效时长 / 缓动 / 触发条件）
- 与 design system 组件 Code Connect 映射（如团队启用）
- 文字 spec：copy 表格 / a11y 注释 / 边界情况

**关键产出物**：
- Figma Dev Mode 视图 + 描述
- Spec 文档（含 a11y / 边界 / 文案）
- 与 dev 半小时 walk-through（异步：Loom 录屏）

**常用工具**：Figma Dev Mode (A2 #10) + Storybook + Code Connect；中文圈：蓝湖（已被 Dev Mode 蚕食但仍在用）

**反模式**：
- "丢个 Figma 链接给开发就完事"——dev 只看像素值，不知道意图
- 没有标响应式断点
- 没有给 a11y 标注，开发以为 "看起来没问题就行"
- Spec 文档无人读——因为没人在 PR review 时被引用过

**信源**：Figma Dev Mode 官方 — https://www.figma.com/dev-mode/ ；Brad Frost "Death to Designer-Developer Handoff" — https://bradfrost.com/blog/post/death-to-designer-developer-handoff/

---

### Step 8. Implementation QA + 上线后跟进

**做什么**：
- Dev 实现完成后，设计师对照原稿做 design QA（spacing / 字号 / 颜色 / 动效）
- 在 staging 环境跑一遍核心 flow
- 上线后看数据（转化、task success、Hotjar 录屏）
- 1–2 周后回顾：实际数据 vs 设计假设

**关键产出物**：
- Design QA bug list（标 severity）
- 上线后 review 文档（与 Step 1 brief 对照）

**常用工具**：Polypane（多视口同时看）/ axe DevTools / Lighthouse / Hotjar / FullStory

**反模式**：
- 上线即遗忘——「这个我做过的，下一个项目」
- 只看数字不看录屏（数字告诉 what，录屏告诉 why）
- 不复盘 → 同样错误第二个项目再犯

**信源**：Julie Zhuo "Hypothesis-Driven Design" — https://medium.com/the-year-of-the-looking-glass/ ；NN/g "How to Conduct a Design QA"

---

### 入门 SOP 总图

```
Intake → Research → Explore → Converge → Hi-fi → Prototype → Handoff → QA
 (1d)    (3-5d)    (2-3d)    (1-2d)    (3-5d)   (2d)       (1d)     (持续)
   ↑________________________________________________________________↓
                          反馈回环（数据 / QA bug / 用户反馈）
```

---

## B. 资深 vs 新手：8 个关键差异

| # | 维度 | 新手 | 资深 | 信源 |
|---|---|---|---|---|
| 1 | **时间分配** | 80% 时间在 Figma 视觉打磨 | 80% 时间在 Step 1–2（问问题、读数据、对齐目标）；hi-fi 只是产物 | Julie Zhuo "The Looking Glass" |
| 2 | **协作方式** | 单独闭门设计；周会上一次性出稿 | 每天 critique / Slack / 1:1 与 PM / dev / 研究员同步 | Brad Frost talks |
| 3 | **工具使用** | 追新工具（这周 v0，下周 Lovable）；插件控 | Figma 基础功能 + variables + components 玩到极致；工具是手段 | Karri Saarinen Lenny's Podcast 2024 |
| 4 | **设计稿迭代** | Hi-fi 一次到位，从开始就在抠像素 | Lo-fi → mid-fi → hi-fi 多轮收敛；前期允许丑 | Jake Knapp《Sprint》 |
| 5 | **反馈处理** | 收到反馈直接改 | 三段拆解：a) PM 个人偏好 → 协商 b) 真实用户证据 → 必改 c) 设计基本功 / a11y → 不让步 | Julie Zhuo "How to Survive a Design Review" |
| 6 | **关注层次** | 关注"这个按钮放哪好看"；单页思维 | 关注"这个 flow 在用户旅程的哪一段"；系统思维 | Don Norman 2023 LinkedIn 文章 |
| 7 | **决策依据** | "我觉得 / 老板觉得" | "数据告诉我们 / Nielsen heuristic / WCAG / 用户访谈 quote" | NN/g UX research-based articles |
| 8 | **职责边界** | 等需求 → 等反馈 → 等开发 | 主动定义问题、主动跨职能拉齐、推 design QA 进 PR | Dan Mall《Design That Scales》, Rosenfeld 2024 |

**额外两条（半数资深人会同意）**：

- **新人怕"无产出"，所以画**；资深人**怕做错事，所以问**。
- **新人觉得"我做的东西是 Figma 文件"**；资深人觉得**"我交付的是用户体验改善 + 团队的设计共识"**。

**信源**：
- Julie Zhuo《The Making of a Manager》(2019) — https://www.juliezhuo.com/book/manager/
- Brad Frost talks — https://bradfrost.com/talks/
- Dan Mall《Design That Scales》(Rosenfeld, 2024) — https://rosenfeldmedia.com/books/design-that-scales/
- 信心：⭐⭐⭐（≥3 资深 figure 公开表达过这些差异）

---

## C. 主要方法论流程（7 个）

### C1. Double Diamond — 双钻模型 ⭐⭐⭐

- **提出**：UK Design Council, 2004（2019 重新强化为 "Framework for Innovation"）
- **阶段**：Discover → Define → Develop → Deliver（发散 → 收敛 → 发散 → 收敛）
- **适用**：宏观流程脚手架；几乎所有教学课程都用它做框架
- **近期演变**：2019 Design Council 加入 "Engage" 外圈（持续与 stakeholder 协作）
- **限制**：太抽象，无法落地到具体 task；常被批"看起来都对，做起来不知怎么做"
- **信源**：https://www.designcouncil.org.uk/our-resources/the-double-diamond/ （一手）
- **信心**：⭐⭐⭐

### C2. Design Thinking — 设计思维 ⭐⭐⭐

- **提出**：IDEO / Stanford d.school（David Kelley 1990s 推广，IDEO 2000s 商业化）
- **阶段**：Empathize → Define → Ideate → Prototype → Test
- **适用**：跨学科创新项目、非软件类设计（医疗、教育、社会创新）
- **近期演变**：2020 后被部分批评为 "design theater"；IDEO 自己也在重新定位（2023 公开承认"我们卖太多 workshop 不做产品"）。Don Norman 2023 直接说"设计思维已变成微优化框架"
- **限制**：在敏捷软件团队里被嫌"太慢"；常被 Lean UX 取代
- **信源**：d.school 资源 — https://dschool.stanford.edu/resources ；IDEO U — https://www.ideou.com/
- **信心**：⭐⭐⭐

### C3. Design Sprint — 设计冲刺（5 天版）⭐⭐⭐

- **提出**：Jake Knapp at Google Ventures, 2016《Sprint》Simon & Schuster
- **阶段**（5 天）：
  - Day 1 Map（地图：长目标 + 用户旅程）
  - Day 2 Sketch（Crazy 8s 发散）
  - Day 3 Decide（投票 + storyboard）
  - Day 4 Prototype
  - Day 5 Test（5 个真实用户）
- **适用**：MVP 验证、大方向决策、新功能/新产品的 0→1
- **近期演变**：
  - 2020 后远程版本（Miro / FigJam + Zoom）
  - 2024+ AI 加速版：Day 2 用 v0 / Galileo 30 分钟生成 20 个方向；Day 5 用 Maze AI insights 异步测试 → 实际可压缩到 2-3 天
- **限制**：5 天对 enterprise 大公司"日程对齐"是奢侈品；很多团队"做减肥版 1-2 天 sprint"，但效果有损
- **信源**：thesprintbook.com — https://www.thesprintbook.com/ （一手）；GV Library — https://www.gv.com/sprint/
- **信心**：⭐⭐⭐

### C4. Lean UX — 精益 UX ⭐⭐⭐

- **提出**：Jeff Gothelf & Josh Seiden《Lean UX》O'Reilly 2013（3rd ed. 2021）
- **核心**：Build–Measure–Learn 循环 + hypothesis-driven
- **流程**：写假设（"我们相信 [改动] 会让 [用户] 达到 [结果]，我们将通过 [指标] 验证"）→ MVP → 测 → 学
- **适用**：敏捷团队（2 周 sprint）、SaaS、有数据 infra 能跑实验
- **近期演变**：2024–2026 与 continuous discovery（Teresa Torres）融合，强调"每周与用户对话 1 小时"
- **限制**：对早期产品很合适；对有强品牌一致性要求（金融、医疗、奢侈品）的产品过激
- **信源**：jeffgothelf.com — https://jeffgothelf.com/ ；3rd ed. 2021
- **信心**：⭐⭐⭐

### C5. Atomic Design — 原子化设计 ⭐⭐⭐

- **提出**：Brad Frost, 2016《Atomic Design》（免费在线书）
- **阶段（系统结构而非流程）**：atoms（按钮、输入框）→ molecules（搜索框 = 按钮+输入框）→ organisms（导航条）→ templates（页面骨架）→ pages（含真实内容的页面）
- **适用**：建 design system 的心智模型；新人理解组件层级
- **近期演变**：2020+ 与 design tokens 派融合；Brad Frost 2024 公开文章《The dark side of design systems》自我反思过度抽象问题
- **限制**：纯组件层级思维，没回答"组件如何 compose / variants 怎么管理"；W3C Design Tokens (2025 稳定 v1) 派认为"应从 token 而非组件出发"
- **信源**：atomicdesign.bradfrost.com — https://atomicdesign.bradfrost.com/ （一手免费书）
- **信心**：⭐⭐⭐

### C6. Jobs-to-be-Done (JTBD) — 用户雇佣产品的"工作" ⭐⭐

- **提出**：Clayton Christensen (HBS 2003, "milkshake" 案例)；Tony Ulwick 落地 ODI 方法（Outcome-Driven Innovation）
- **适用**：替代 persona 的另一种用户表示法；偏战略 / 产品定位
- **句式**："When [situation], I want to [motivation], so I can [outcome]"
- **近期演变**：Alan Klement《When Coffee and Kale Compete》（2016）把 JTBD 普及到 UX 圈；与 Lean UX hypothesis 融合
- **限制**：与传统 persona 派论战不休；做 mature 产品改进时不如 persona 直观
- **信源**：Clayton Christensen HBR — https://hbr.org/2016/09/know-your-customers-jobs-to-be-done ；Intercom Jobs Stories
- **信心**：⭐⭐

### C7. Hypothesis-Driven Design — 假设驱动设计 ⭐⭐

- **提出**：Lean UX 派（Gothelf）+ Julie Zhuo（Facebook 实操）推广
- **核心**：每个设计决策都写成可证伪假设
- **句式**："我们认为 [设计改动] 会让 [用户群] 在 [场景] 达到 [结果]；我们以 [metric] > [阈值] 判断成立"
- **适用**：大厂 / 数据成熟团队；与 A/B test infra 结合
- **近期演变**：与 continuous discovery 融合（Teresa Torres《Continuous Discovery Habits》2021）；2024+ 加 AI 辅助生成假设
- **限制**：依赖足够流量做 A/B；早期产品流量不够不适用
- **信源**：Julie Zhuo "The Looking Glass" — https://lookingglass.substack.com/ ；Teresa Torres — https://www.producttalk.org/
- **信心**：⭐⭐

---

### 方法论选用决策树

```
项目类型？
├── 0→1 新产品 / 大方向探索 → Design Sprint (5d) 或 Design Thinking
├── 既有产品功能迭代 → Lean UX + Hypothesis-Driven
├── 建 design system → Atomic Design + Design Tokens 双轨
├── 用户洞察重要 / 不知道做什么 → JTBD 或 Continuous Discovery
└── 不知道选哪个 → Double Diamond 作为顶层框架，细节用上面任一种
```

---

## D. 设计系统 / Design Ops 工作流（2026 大热）

### D1. 从 0 建设计系统的 6 步

| # | 阶段 | 关键活动 | 工具 |
|---|---|---|---|
| 1 | **Audit / 现状盘点** | 截图全产品所有按钮、表单、卡片；归类发现"21 种蓝色，14 种间距" | Figma + Eight Shapes audit framework |
| 2 | **Tokens / 设计令牌** | 定义 primitive (color-blue-500) → semantic (color-action-primary) → component tokens | Tokens Studio (Figma plugin), Style Dictionary (Amazon) |
| 3 | **Primitives / 底层组件** | unstyled accessible primitives：Button、Input、Dialog、Tooltip | Radix UI / Base UI / Headless UI |
| 4 | **Components / 表层组件** | 加视觉的实际组件，含 variants / states | shadcn/ui + Tailwind / 团队自建 |
| 5 | **Docs / 文档** | 用法 / props / a11y / 反例 | Storybook + 自定义页 / Zeroheight |
| 6 | **Adoption / 推广** | 内部 office hours、新人 onboarding doc、Slack 频道、季度 release notes | Slack + Notion + Loom |

**信源**：
- Nathan Curtis (EightShapes) — https://medium.com/eightshapes-llc
- Brad Frost atomicdesign.bradfrost.com
- Dan Mall《Design That Scales》(2024) — https://rosenfeldmedia.com/books/design-that-scales/

### D2. Design system 团队的 day-in-the-life

资深 design system designer 一天大致：
- **9:30** Slack 答疑（5–10 个 PM/dev 问"我该用哪个组件"）
- **10:30** Figma：新组件 PR review（variants 是否合理 / 与 token 对齐）
- **11:30** 与一个产品团队 1:1 office hour
- **13:30** 写新组件设计稿 + Storybook story
- **15:00** Design system meeting：road map + governance 决策
- **16:00** 季度 release notes 起草 / 录 Loom demo

**信源**：Dan Mall LinkedIn long posts 2024；Brad Frost daily logs

### D3. 现代 Handoff 方式（2026）

```
Figma file (design)
    │
    ├── Dev Mode (设计意图) + Code Connect (Figma 组件 ↔ React 组件)
    │
    ├── Design tokens (Tokens Studio → JSON → Style Dictionary)
    │       ├── CSS variables
    │       ├── Tailwind config
    │       └── iOS/Android tokens (跨端)
    │
    └── Storybook (代码 source of truth + 文档 + 可视化测试)
```

**信源**：Figma Dev Mode 官方 — https://www.figma.com/dev-mode/ ；Brad Frost "Death to Designer-Developer Handoff"

### D4. Governance / 治理

谁能改 token？谁能加新组件？怎么 deprecate？典型成熟团队 3 层：

| 层 | 谁能改 | 例 |
|---|---|---|
| **Tokens（最严）** | 仅 design system 团队 + design lead | 改 color-action-primary 会影响全产品 |
| **Components（中）** | DS 团队 + 提案 RFC 通过 | 加新 Drawer 组件 |
| **Patterns（开放）** | 产品团队自治 | 把现有组件组合出 Settings 页 pattern |

**反模式：**
- 没有 RFC → 每个团队都加组件 → 库膨胀失控
- 治理太严 → 产品团队"绕过 DS 自建"
- 没有 deprecation 协议 → 老组件残留几年

**信源**：Nathan Curtis — https://medium.com/eightshapes-llc ；DesignOps Summit (NN/g) — https://www.nngroup.com/

### D5. Design system 反模式

- **过度抽象**：组件 props 30 个，没人记得住（Dan Mall 多次点名）
- **没人用 / Phantom DS**：建好但 PM 绕过自找现成 npm 包
- **PM 当 DS 团队的 backlog**：组件请求队列堆 200 个，DS 团队疲于奔命
- **没文档 / 文档过时**：Storybook 半年没更，开发不信任
- **过度对标 Material / Carbon**：照搬大厂体系，自己产品不需要
- **Figma 与代码偏离**：变成"两个 design system"，每周对账

**信源**：Brad Frost "The Dark Side of Design Systems"（2024 blog）— https://bradfrost.com/blog/ ；Dan Mall《Design That Scales》

---

## E. 2024–2026 工作流变化（master skill 的核心时效价值）

> ⚠️ 本节快速演变中，半年后部分细节可能变化；趋势方向相对稳定。

### E1. AI 介入早期探索（最大的一项）

**节奏变化**：
- 旧：设计师手画 3 稿 / 3 天
- 新：30 分钟用 v0 / Figma Make / Lovable 生成 20 个方向 → 人筛 3 个深化 → 1 天完成

**机制**：把"发散"成本压到接近零；瓶颈从"想出方案"变成"分辨好坏"。

**适用步骤**：A3（Explore）+ A5（Hi-fi 初稿）

**信源**：
- State of Design 2025 (uxtools.co/survey) — 41% 从业者已在工作流中用 AI 设计工具
- Figma Config 2025 keynote — https://config.figma.com/
- Brad Frost 2025 "Design System v2" series

**信心**：⭐⭐⭐（已是共识趋势，但工具具体输出**仍参差**）

---

### E2. Design Engineering 边界融合

**节奏变化**：
- 旧：设计师交 Figma → 开发实现 → QA → 上线（2–3 周）
- 新：design engineer 在 Cursor + shadcn + Tailwind 里直接出 PR，handoff 退化（5–7 天）

**关键人物**：Rauno Freiberg (Vercel)、Karri Saarinen (Linear)、Brad Frost、Adam Wathan

**核心主张**："Code as source of truth"——Figma 仅作思考媒介，代码才是产品

**信源**：
- rauno.me/craft — https://rauno.me/craft
- Vercel Geist Design System
- Linear engineering blog — https://linear.app/blog/
- Brad Frost "Death to Designer-Developer Handoff" — https://bradfrost.com/blog/post/death-to-designer-developer-handoff/

**信心**：⭐⭐⭐（在前沿团队已落地；传统企业仍传统 handoff）

---

### E3. Figma 平台化（一站式）

**变化**：
- 2025 Config 发布 Sites / Slides / Buzz / Make / Draw / Grid
- 设计师可在 Figma 内覆盖：UI 设计 → 网站发布 → 演示文稿 → 营销素材
- 边界扩张到"创意/营销"和"前端工程"两个方向

**影响**：
- 中小团队不再需要 Webflow / Canva / Notion 多工具
- Adobe / Canva 应对压力上升

**信源**：Figma Config 2025 — https://config.figma.com/ ；2026 Config 5 月底举办

**信心**：⭐⭐⭐

---

### E4. 用户研究 AI 化

**变化**：
- 旧：1 个研究员 1 周转录 + 编码 5 场访谈
- 新：Dovetail AI / Maze AI insights 自动转录 + 主题提取 + quote 检索 → 1 个研究员可处理 3–5 倍样本

**配比新常态**："1 个研究员 + AI" 替代过去的"3–5 人研究小组"

**风险**：AI 标签的"主题"经常合并掉关键洞察的细节；resilient 研究员仍 manual sanity check

**信源**：
- Dovetail AI — https://dovetail.com
- Maze AI Insights
- NN/g "A Research Agenda for Generative AI in UX" (2025) — https://www.nngroup.com/articles/genai-ux-research-agenda/

**信心**：⭐⭐（方向明确，但 AI 主题提取**仍易漏 nuance**）

---

### E5. a11y 上升为合规要求

**变化**：
- **European Accessibility Act (EAA) 2025-06-28 已生效** → 欧盟 27 国 B2C 数字产品必须 WCAG 2.1 AA 等价水平
- 不合规可罚款；过往是"应该做"，现在是"必须做"
- a11y 从 nice-to-have 进入 sprint definition of done
- Stark Figma plugin / axe DevTools 使用率激增

**对工作流影响**：
- Step 5 hi-fi 必须做 a11y 自检
- Step 7 handoff 含 a11y annotation
- Step 8 QA 跑 axe / Lighthouse / 手动键盘 + screen reader

**信源**：
- EAA 官方 — https://ec.europa.eu/social/main.jsp?catId=1202
- W3C WCAG 2.2 — https://www.w3.org/TR/WCAG22/
- Deque axe — https://www.deque.com/axe/

**信心**：⭐⭐⭐

---

### E6. 远程 / 异步协作成默认

**变化**：
- FigJam 取代白板
- Loom 录屏 critique 取代会议（一段 5 分钟 Loom 比 30 分钟 Zoom 高效）
- 跨时区团队不再要求"同步会议"，async DM + Loom + Figma comment 三件套

**信源**：Smashing Magazine 2024–2025 remote workflow articles — https://www.smashingmagazine.com/ ；Khoi Vinh subtraction.com 多篇

**信心**：⭐⭐⭐

---

### E7. Design system 进入"产品化"阶段

**变化**：
- Dan Mall《Design That Scales》(2024) 把 DS 当产品运营（roadmap、internal customer、release notes、sunset）
- DesignOps 角色独立成 job title
- W3C Design Tokens Spec 2025-10 达到 stable v1，工具互操作时代开启

**信源**：
- Design That Scales — https://rosenfeldmedia.com/books/design-that-scales/
- W3C DTCG — https://www.w3.org/community/design-tokens/2025/10/28/design-tokens-specification-reaches-first-stable-version/

**信心**：⭐⭐⭐

---

## F. 不同场景的 workflow 变体

| 场景 | 重心 | 流程特点 | 关键工具 |
|---|---|---|---|
| **B2B SaaS** | Design system + ops；复杂权限/状态/表单 | Lean UX + design tokens + Storybook | Figma + shadcn + Tokens Studio + Storybook |
| **B2C 产品** | 用户研究 + 转化 funnel | Hypothesis-driven + A/B test 重度 | Figma + Maze + Hotjar + Amplitude/Mixpanel |
| **创意 / agency** | Visual concept + 提案能力 | Moodboard → 3 方向 hi-fi → 客户选 | Figma + Framer + Webflow + Photoshop |
| **Freelancer / solo** | 快速产出 + 客户管理 + 报价 | 1 人压缩版 Double Diamond；轻文档 | Figma + Notion + 合同模板 + Mobbin |
| **初创 / MVP** | Speed + 验证 | Design Sprint 压缩为 1–2 天；hi-fi from day 1 | Figma + v0 + Cursor + shadcn |
| **中国大陆大厂** | 视觉精度 + KPI 配合 + B 端中后台 | 阶段评审制；视觉评审重；蓝湖 handoff | MasterGo / 即时设计 + 蓝湖 + Ant Design / Arco / Semi |
| **欧盟 B2C** | a11y 合规 + 隐私 (GDPR) | DS 标准化 + a11y QA 强制 | Figma + Stark + axe + Penpot（自托管选项） |

**信源**：UX Tools Survey 2025 (uxtools.co/survey)；State of Design 2025；行业从业者公开 talk 综合

---

## G. 反模式 / 团队雷区

学习者要避开的 10 个工作流陷阱：

1. **「Pixel-perfect 但没人用过」**——不做研究 / 不验证。资深人第一反应："你测过几个用户？"
2. **「Design review 变成老板评分」**——HiPPO 病（Highest Paid Person's Opinion）。Critique 需要结构化反馈框架，否则退化。
3. **「研究做完不影响决策」**——research theater；做给 stakeholder 看的合规动作，与最终设计无关联。
4. **「设计系统建好后没人维护」**——24 个月内 30% 的 DS 沦为 phantom（Dan Mall）。没有 ownership + release cadence 就死。
5. **「过度依赖 AI 工具」**——v0 出的 UI "看似可行"，但 a11y / 状态 / 边界全不覆盖；新人若 skip 基本功，3 年后失业风险高。
6. **「Handoff 文档无人看」**——开发只看 Figma 像素值，spec 文档堆积。修法：把 a11y / 文案 / 状态写进 Figma frame 描述，不开外部文档。
7. **「直接抄 dribbble」**——dribbble shot 是"hero shot"，不含 edge case、a11y、真实数据。抄完发现下不去手。
8. **「过度发散，从不收敛」**——做 50 个方向但不敢选；Jake Knapp Sprint 强制"独立投票 + 一锤定音"治这病。
9. **「视觉派 vs 研究派内耗」**——团队没有共识"craft 与 data 哪个重"——参考 Karri Saarinen / Julie Zhuo 公开辩论。
10. **「沉默的设计师」**——只画不说。资深人有义务在 product / engineering 决策会上发声，否则被边缘化。

**信源**：
- Don Norman 2023 "UX is broken" Fast Company — https://www.fastcompany.com/
- Brad Frost "Dark Side of Design Systems" 2024
- Julie Zhuo "How to Survive a Design Review"
- Dan Mall《Design That Scales》Ch. "Phantom Systems"

---

## 调研收尾：信心 / 缺口 / 给学习者

### 最有信心的 3 个发现

1. **资深 vs 新手的核心差异不是工具，是时间分配**：80/20 颠倒——资深人 80% 时间在"问问题、对齐、读数据"，新人 80% 时间在 Figma。这一点 3 份独立来源（Julie Zhuo, Brad Frost, Dan Mall）都直接表达过。⭐⭐⭐
2. **2026 年 handoff 模型正在崩塌**：design engineering 派（Rauno / Karri / Brad Frost）已在前沿团队把"设计 → 开发"两个角色合并为一个 PR-owner；Figma Dev Mode + Code Connect + shadcn 是工具基础。⭐⭐⭐
3. **a11y 已从"应该做"变"必须做"**：EAA 2025-06 生效让欧盟 B2C 强合规；这是 master skill 时效里**最具法律确定性**的变化。⭐⭐⭐

### 2024–2026 工作流变化中最大的一项

**「AI 把发散成本压到接近零，瓶颈从"画"变成"分辨"」**——这是过去 12 个月最深刻的变化。具体表现：
- v0 / Lovable / Figma Make 让"30 分钟出 20 个方向"成为可能
- 但 AI 输出的"看起来可行"的稿 80% → 100% 完成度成本陡升
- 新人技能要求重排：**判断力 > 出图速度**

但需诚实标注：**结果质量参差，2026 年仍处于 hype peak 末期**。

### 入门 SOP 最易卡住新人的 bottleneck

**Step 4 Converge / 决策环节**。理由：
- Step 1–3 都是收集 + 发散，新人能"靠勤奋"完成
- Step 4 需要判断力——"为什么这个方案优于那个"——这是经验密集型能力
- 新人在 Step 4 卡住的典型表现：等老板拍板 → 老板拍板 → 进入返工循环 → 自信瓦解
- 资深人在 Step 4 主导，是其价值最高的时刻

破解方法：
- 强制写"决策日志"（即使 5 行）
- 学会 Adam Connor《Discussing Design》的反馈框架
- 在 critique 中练习"我的方案选 A 因为…"的语言能力

### 中文圈 vs 英文圈 workflow 显著差别

| 维度 | 英文圈 | 中文圈 |
|---|---|---|
| **方法论原书** | 直接读 Sprint / Lean UX / Atomic Design 一手 | 多读译本 + 公司内训演绎；公开演讲层一手输出少（张小龙是例外） |
| **Handoff 工具** | Figma Dev Mode → Code Connect → Storybook | **蓝湖**仍是主流（虽 Dev Mode 在蚕食）；Storybook 在大厂普及 |
| **Design system** | Material / Carbon / Polaris + 独立 DS 团队 | Ant Design / Arco / Semi / TDesign + 大厂中后台导向 |
| **a11y** | 合规驱动（EAA / ADA） | GB/T 37668-2019 存在但执行弱；多为大厂自驱（信通院） |
| **B 端比重** | B2B SaaS 与 B2C 并重 | **B 端中后台占比明显高于英文圈**（阿里/字节/百度系基础设施 + ToG） |
| **节奏** | Sprint / 双周迭代 | 大厂"季度 + 大版本"；外加"快速试错"两极分化 |
| **AI 落地** | Cursor + v0 + Lovable 已常见 | MasterGo AI / 即时设计 AI / 蓝湖 AI 国产替代落后 6–12 个月，但追赶很快 |
| **设计师晋升路径** | individual contributor (IC) 与 manager 双 ladder 清晰（Julie Zhuo 体系） | 多数公司晋升仍偏 manager 轨；IC 高级别 senior designer 头衔稀缺 |

**最大差异**：英文圈"craft + data" 双驱动相对成熟，中文圈"中后台 + 业务赋能" 更重；但 2024–2026 在 AI 工具上中文圈正在快速对齐。

**信源**：UX Tools Survey 2025；IXDC 议题历年综合；阿里 UCAN 公开议题；张小龙 2019 微信公开课。

---

end of file.
