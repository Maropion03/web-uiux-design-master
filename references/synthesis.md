# Web UI/UX Design — Industry OS Synthesis

last_updated: 2026-05-12 · locale: zh + en terms · audience: 想入行的中英双语 Web UI/UX 学习者

---

## 1. 心智模型 (Mental Models)

筛选规则：跨场景复现 ≥2 + 生成力 + 排他性。最终留下 5 个。

### 1.1.  Affordance / Signifier 二分（可供性 vs 指示器）
- **一句话**：物体能做什么（affordance）和用户能否看出能做什么（signifier）是两件事；UI 上 90% 的可用性问题不是"做不到"而是"看不出来能做"。
- **跨场景**：Norman《Design of Everyday Things》(2013) 推门案例；Nielsen Heuristic #6 "Recognition over recall"；shadcn/Radix 把"按钮看起来像按钮"做成 primitive 的设计哲学。
- **生成力**：拿到"用户找不到导出按钮"的反馈→不去想"按钮放哪好看"，而是问"它有 signifier 吗（hover、icon、label）"。
- **排他性**：外行说"按钮不够显眼"，这行的人说"按钮缺 signifier，affordance 在但用户不知道"——一字之差决定改 contrast 还是改 IA。
- **局限**：纯 signifier 优化解决不了底层 IA 错误。

### 1.2.  Hypothesis-Driven, not Aesthetic-Driven（假设驱动 > 审美驱动）
- **一句话**：每个设计决策必须能被证伪——"我们认为 [改动] 会让 [用户] 在 [场景] 达到 [结果]，以 [metric] 验证"。"好不好看"不是判据。
- **跨场景**：Lean UX (Gothelf)、Julie Zhuo "The Looking Glass"、NN/g Research-based articles、Teresa Torres Continuous Discovery。
- **生成力**：拿到一个"我觉得这版更高级"的方案→立刻问"假设是什么？用什么 metric 证伪？"
- **排他性**：Dribbble 派看 hero shot；这行的资深人看假设链。Karri Saarinen 反方代表（"很多 craft 决定该由强 taste 拍板"）的存在本身证明这是个行业内立场。
- **局限**：早期产品流量不够无法 A/B；对强品牌（金融/奢侈品）过激。

### 1.3.  Atomic / Tokens 组件树思维（设计是系统，不是画布）
- **一句话**：设计的最小单位不是"页面"，是 token → primitive → component → pattern 的组件树；改一处影响全局。
- **跨场景**：Brad Frost《Atomic Design》；Nathan Curtis EightShapes token 三层架构；W3C Design Tokens stable v1 (2025-10)；shadcn registry 协议。
- **生成力**：被要求"新加一个绿色"→不是加 hex，是问"它是 primitive 还是 semantic？谁该消费它？"
- **排他性**：视觉派看页面，系统派看 token 流。Brad Frost vs Ellen Lupton 的 craft 定义分歧实证此模型属"系统派专属镜片"。
- **局限**：过度抽象会让组件 props 30+ 个没人用（Dan Mall《Design That Scales》Phantom Systems）。

### 1.4.  认知负荷工程（设计 = 减少用户脑子的工作）
- **一句话**：UI 的任务是把外在认知负荷（extraneous load）压到接近零；Krug 的"Don't Make Me Think"、Cooper 的 goal-directed、Sweller 的 cognitive load theory 是同一件事的三种表述。
- **跨场景**：Krug 2014 整本书；NN/g F-Pattern + Progressive Disclosure；Miller 7±2；张小龙"用完即走"。
- **生成力**：表单 8 个字段→问"哪些可以延迟收集（progressive disclosure）？哪些可以预填？"而不是"怎么排好看"。
- **排他性**：外行加功能，这行的人减功能。张小龙跟硅谷 craft 派在不同语境下导出同一立场是强证据。
- **局限**："减"过头变成 over-minimalism，藏了关键 affordance。

### 1.5.  Craft as a Filter（手艺是 100 个微小决策的累积）
- **一句话**：好设计与平庸设计的差距不是 1 个大决定，是 100 个 4px/100ms/缓动曲线/默认值的累积；"品味 = 默认值"。
- **跨场景**：Refactoring UI 整本（Wathan/Schoger）；Rauno Freiberg rauno.me/craft；Karri Saarinen Linear "Quality is a side effect of caring about defaults"；Joshua Comeau interactive teaching。
- **生成力**：review 一个稿子→不指出"整体不好"，而是列出 8 个具体 paper cut（hover 缺失、字号跳级、focus ring 没做、loading 时长不对）。
- **排他性**：PM/工程师看功能完成度，这行的人看 paper cuts。Design Engineering 派（Rauno/Karri/Wathan）整体作为一个流派的存在就是此模型的社会学证据。
- **局限**：纯 craft 不解决战略错位；用户调研一句"我从不来这页"打败 100 个 paper cut 修正。

> 候选但降级到 Section 2 的：「a11y 是基本面不是补丁」（重要但 2025 后是合规要求，更像决策启发式而非排他镜片）；「Friction 中性论」（Brignull 反向运用，证据偏单一）。

---

## 2. Standard Playbook（决策启发式 8 条）

1. **如果是新人挑第一款工具 → Figma Free，不要犹豫**。行业 80%+ 招聘需求；Sketch 跨 OS 坏、XD 已死、Framer 转 no-code 建站。
2. **如果初稿 hi-fi 出得太顺 → 回去做 lo-fi 三方案**。Hi-fi from day 1 是被现成组件锁死想象力，资深人会问"另外两个方向呢"。（Jake Knapp Sprint Day 2 Crazy 8s 反向证据）
3. **如果 design review 只有老板说话 → 停下来跑 5 人可用性测试**。HiPPO 病的解药是数据。Nielsen 1993 五人法则 + RITE。
4. **如果功能页超过 3 个 CTA → 砍掉 2 个**。Hick's Law 工程化；张小龙派 + 认知负荷模型双重背书。
5. **如果设计系统没人用 → 砍组件不加组件**。Dan Mall《Design That Scales》Phantom Systems：24 个月内 30% DS 死于无 ownership。先 deprecate 旧的、补 office hours，不是开新 PR。
6. **如果在中国大陆 + Figma 慢 → 转 MasterGo / 即时设计，不要等 Figma 特通版**。特通版功能滞后 1-2 版本且无 AI；蓝湖 handoff 仍主流。
7. **如果欧盟 B2C 用户 → a11y 先于视觉**。EAA 2025-06-28 已生效，WCAG 2.1 AA 是 sprint Definition of Done，不是 nice-to-have。
8. **如果 AI 工具产出 80% 完成度的稿 → 从 0 重写而非 patch**。v0/Lovable 的边际成本在 80% 后陡升；老手共识"判断力 > 出图速度"。

> 信心相对偏弱的一条：第 8 条。是 2025 年才形成的共识，证据来自 State of Design 2025 + Brad Frost 2025 系列 + 个别资深人 talk，未来 12 个月可能被新一代 AI 工具改写。

---

## 3. 工具栈与选型决策树

**学习者必备 8 件**（年更率低）：Figma Free · shadcn/ui · Radix UI · Storybook · axe DevTools 浏览器扩展 · Mobbin Free · Phosphor / Lucide · WebAIM Contrast Checker。

**场景化补充**：
- 微交互：Figma Variables 起步 → 复杂用 Rive (state machine) → 插画动画用 Lottie。
- 协作：Figma Dev Mode + Code Connect（外企）/ 蓝湖（中国大陆传统团队）。
- 研究：Maze Starter $99 + Notion；进阶 Dovetail（AI 主题提取）。
- 中国大陆：MasterGo / 即时设计 + 蓝湖 + Ant Design / Semi。
- AI 探索：v0（React）或 Figma Make——仅做 day-1 发散，不要交付。

**避坑黑名单**：Adobe XD（停更）· Sketch 在跨 OS 团队 · Principle / Magician / Avocode（停更）· Photoshop 做 UI · Framer 当 Figma 用 · Adobe 全家桶（UI 设计师不需要）· Zeplin 新项目（被 Dev Mode 取代）。

**AI 工具诚实告诫**：v0 / Lovable / Bolt.new / Figma Make 同质化竞争（State of Design 2025: 41% 已用）；但**输出质量参差 + 3-6 月迭代**；用作早期发散加速器（"30 分钟 20 个方向"），不用作交付。Decay 标记：本节 tools 6 月内可能 30% 失效。

---

## 4. 工作流 / Pipeline

**入门 SOP 8 步**（精炼）：Intake (1d) → Research (3-5d, 5 user 法则) → Explore (lo-fi 多方案) → Converge (critique 决策) → Hi-fi (含 hover/focus/disabled/loading/error/empty + 响应式 + a11y) → Prototype + 5 人测试 → Handoff (Dev Mode + a11y annotation + 文案 spec) → Implementation QA + 上线后数据回顾。

**资深 vs 新手 5 条关键差异**：
1. **时间分配**：新人 80% 在 Figma 视觉；资深 80% 在 Step 1-2（问问题、读数据、对齐）。
2. **反馈处理**：新人收到就改；资深三段拆解（个人偏好→协商 / 真实用户证据→必改 / a11y 基本功→不让步）。
3. **关注层次**：新人想"这按钮放哪"；资深想"这 flow 在用户旅程哪段"。
4. **决策依据**：新人"我觉得"；资深"用户访谈 quote + Nielsen + WCAG"。
5. **职责边界**：新人等需求等反馈；资深主动定义问题、推 design QA 进 PR。

**2024–2026 工作流变化 5 条**（按影响力降序）：
1. **AI 把发散成本压到接近零**——瓶颈从"画"变成"分辨"。
2. **Design Engineering 边界融合**——handoff 在前沿团队（Vercel/Linear）正在消失，Cursor + shadcn + Tailwind 取代部分传统流程。
3. **a11y 从应该做变必须做**——EAA 2025-06 生效。
4. **Figma 平台化**——Sites/Slides/Buzz/Make/Draw/Grid 蚕食 Webflow/Canva。
5. **用户研究 AI 化**——1 个研究员 + Dovetail AI 替代过去 3-5 人小组。

---

## 5. 行业表达 DNA

**高频用语（中英对照）**：pixel-perfect（像素级精确）· ship it（发出去）· dogfood / dogfooding（自家产品自己用）· smell test（直觉嗅探）· paper cut（细小毛刺）· north star（北极星指标）· polish pass（打磨轮）· design debt（设计债）· edge case（边界情况）· happy path / sad path（顺利路径 / 失败路径）· golden path（黄金路径）· hi-fi / lo-fi（高保真 / 低保真）· hand-off（交付）· source of truth（单一可信源）· a11y（无障碍）· token（设计令牌）· variant（变体）· source-of-truth-drift（设计稿与代码偏离）· phantom system（无人用的设计系统）。

**Register 差别**：
- **Critique 严肃**："这里的 affordance 不够强，hover 没 signifier；状态覆盖 happy path 但缺 empty 和 error；这版的假设是什么、怎么证伪？"
- **闲聊轻松**："这玩意儿太 dribbble 了 / 给开发递这版要被骂 / 又一个 phantom DS / 这家是 v0 出的吧"。

**内部 vs 外部沟通**：
- 对 PM：用 metric + hypothesis 语言（"假设 conversion +5%"）。
- 对工程：用 token + component + state 语言（"这是 semantic token，请走 Code Connect"）。
- 对客户：用 outcome + risk 语言，不堆"affordance / heuristic"。
- 对用户：去黑话，纯任务语言。
- 对同行：直接黑话上，"这是 anti-pattern"够了。

**5 个外行常见破绽**：
1. 把"UI"当"UX"用，简历写"擅长 UI/UX 设计"无区分。
2. 把 Figma 高保真静态稿叫"原型"。
3. 把 dribbble shot 当作品集，无 edge case / 真实数据。
4. 说"WCAG AAA 是高级目标"（实际行业锁 AA）。
5. "Heuristic" 念错（/hjuːˈrɪstɪk/）+ "ARIA / a11y" 念法离谱。

---

## 6. 质量基准 + 反模式

### 6.1 「好」的 5 条具体可验证基准

1. **5 秒测试通过**：5 个未见过产品的人，5 秒内能说出主要功能 / 主操作。
2. **状态覆盖完整**：default / hover / focus / active / disabled / loading / empty / error / 长内容 / 0 数据，10 态俱全。
3. **a11y baseline**：axe DevTools 零 violation + 纯键盘可完成所有任务 + 对比度 ≥ 4.5:1（正文）/ 3:1（大字）+ touch target ≥ 24×24 CSS px（WCAG 2.5.8）+ focus indicator 可见。
4. **视觉 hierarchy 通过眯眼测试**：眯起眼睛看，主操作仍跳出来。
5. **响应式 320px–1920px 不破**：在 Polypane 或浏览器多视口下，无横向滚动条 / 无重叠 / 无被截断 CTA。

### 6.2 反模式（10 条）

1. 把视觉精修当全部，忽略 IA / user flow。
2. 抄 Dribbble 不考虑业务约束与 edge case。
3. Pixel-perfect 但缺 loading / empty / error。
4. 设计系统过度抽象（30 个 props 没人记得）。
5. 收到反馈不分析直接改 / 不问"为什么"。
6. 用色靠感觉不靠 token / 不分 primitive vs semantic。
7. 把 a11y 当合规复选框（不做键盘测试 + 不挂 screen reader）。
8. 拿 v0 / Lovable 输出当成品（看似可行 80% → 100% 暴雷）。
9. Research theater：做了研究但结论不影响最终决策。
10. 沉默的设计师：只画不说，决策会缺席被边缘化。

---

## 7. 智识谱系

### 流派 1: 认知 / 学院派
奠基：Don Norman、Jakob Nielsen；当代：NN/g 团队、Susan Weinschenk、Jon Yablonski。核心主张：UX 是认知科学的应用，可用性可被启发式评估、五人测试足以发现 85% 问题。

### 流派 2: 系统 / Web 派
奠基：Brad Frost、Adam Wathan；当代：Dan Mall、Nathan Curtis、Steve Schoger。核心主张：设计是组件树 + token 流，code as source of truth。

### 流派 3: 视觉 / 排版派
奠基：Ellen Lupton、Josef Müller-Brockmann；当代：Khoi Vinh、独立 agency 圈、Awwwards 生态。核心主张：品牌排版独特性 > 通用一致性；craft 包含 letter→text→grid 三层。

### 流派 4: 当代实操 / 产品派
代表：Julie Zhuo、Karri Saarinen (Linear)、Rauno Freiberg (Vercel)。核心主张：设计 leadership 与"品味即默认值"双重；hypothesis-driven。

### 流派 5: 伦理 / 包容派
代表：Harry Brignull (deceptive patterns)、Microsoft Inclusive Design 团队、a11y 圈。核心主张：UX 必须与立法/监管对话；包容设计是过程论。

### 流派 6: Design Engineering 派（2023+ 新流派）
代表：Rauno Freiberg、Karri Saarinen、Brad Frost（晚期立场）、shadcn 作者。核心主张："Death to designer-developer handoff"；Figma 仅作思考媒介，PR is the deliverable。

**关键分歧**：
- 系统派 vs 视觉派：craft 定义不同（系统派 = 一致性 & token；视觉派 = 品牌独特性）。
- 实证派 (Nielsen/Zhuo) vs Taste 派 (Saarinen)：用户测试结果 vs 设计师 taste 谁拍板。
- Atomic Design vs Design Tokens：组件层级 vs token 优先；2025 W3C DTCG stable v1 后两者在融合。
- Hooked (Nir Eyal) vs Deceptive Patterns (Brignull)：行为设计被武器化 vs 被监管。

---

## 8. 诚实边界

- **信息截止 2026-05-12**。
- **衰减最快**（3–6 月）：AI 设计工具（v0 / Lovable / Figma Make）、Figma 平台化产品矩阵、AI × 研究工具。本 OS 的 tools 章节预计 6 个月内 ~30% 失效。
- **衰减中等**（1–2 年）：workflow 变体、Design Engineering 边界、design system 治理实践、Figma Config 节奏。
- **衰减最慢**（数年）：5 个 mental models、Nielsen heuristics、WCAG 框架、Norman / Krug / Cooper 核心论点。
- master skill 不能替代真实项目实战——本 OS 是脚手架不是文凭。
- **中文圈一手素材稀薄**：14 figures 仅 1 个中文圈达"一手 URL"标准（张小龙）；中文 podcast / newsletter 头部稳定信源缺失。
- **HCI 学术经典覆盖偏轻**：Bill Buxton《Sketching User Experiences》、Saul Greenberg、HCI CHI papers 主线未深入抓取。
- **成功者发声偏差**：公开材料多来自大厂存活下来的人，失败案例（DS 死掉、设计师转行、伦理翻车）样本不足。
- **6 轨调研可能漏掉小众但重要的 figure / tool**：尤其是欧洲、日本、东南亚的本地化 figure 与工具几乎未覆盖。

---

## 9. Agentic Protocol — 行业人面对新问题的 7 个研究维度

拿到一个新的 Web UI/UX 设计问题，行业资深人会默认按这 7 个维度查功课：

### 9.1 用户目标 + JTBD

- **看什么**：为什么用户来这里、解决什么 job、当前怎么解决
- **在哪看**：跑 5 人用户访谈（Nielsen 1993 法则）
- **输出格式**：用 JTBD 句式"When [situation], I want to [motivation], so I can [outcome]"；查现有 Hotjar / FullStory 录屏 30 分钟

### 9.2 同类 reference + pattern 扫描

- **看什么**：别人怎么做这个
- **在哪看**：Mobbin / Page Flows 找 5-10 个同类 flow
- **输出格式**：Refero / Calltoidea 查组件级别参考；记录 3 个最像 + 3 个最不一样的

### 9.3 数据密度与 IA 判断

- **看什么**：主屏要承载多少 metric、何频率刷新、要 drill-down 吗、内容树多深
- **在哪看**：Card sorting / tree testing 决定层级
- **输出格式**：眯眼测试 hierarchy；F-Pattern vs Z-Pattern 评估扫读路径

### 9.4 响应式与设备

- **看什么**：主要用户在桌面/平板/手机、多窗口吗、touch 还是 hover
- **在哪看**：看 analytics 设备分布
- **输出格式**：Polypane 多视口同步设计；touch target ≥ 24×24 / Apple HIG 44pt / Material 48dp 选档

### 9.5 设计系统选型 + token 边界

- **看什么**：公司有没有 DS、选 shadcn/MUI/Carbon/Ant Design/自建、token 三层是否齐备
- **在哪看**：Audit 现有产品 21 种蓝色 14 种间距
- **输出格式**：查 W3C Design Tokens spec 兼容性；评估 shadcn registry / Tokens Studio 接入成本

### 9.6 a11y baseline + 合规要求

- **看什么**：目标用户 / 地域有合规要求吗（EAA / ADA / GB/T 37668 / DSA）；WCAG AA 各条是否覆盖
- **在哪看**：跑 axe DevTools + Lighthouse
- **输出格式**：纯键盘走一遍；screen reader 抽查；查 WCAG 2.2 understanding 文档对应条款

### 9.7 AI 探索预算 + 决策证据链

- **看什么**：能不能用 v0 / Figma Make 撒 20 个方向再选；这个设计的关键决定要 PM / 工程 / 用户研究中的哪个证据来支撑
- **在哪看**：v0 / Figma Make 30 分钟跑 10-20 个方向→筛 3 个→人工深化
- **输出格式**：写 hypothesis 卡片"我们认为 [改动] 会让 [用户] 在 [场景] 达到 [结果]，以 [metric] 验证"；建决策日志（哪怕 5 行）

