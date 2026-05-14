# Track 02: Tools — Web UI/UX Design
last_updated: 2026-05-12
tool_count: 67
locale: en + zh

> 面向想入行的学习者：一张 2026 年还在被真实从业者打开的「工具地图」。
> 选型逻辑：① 必装 canonical（≥80% 从业者）；② 中国大陆特化栈；③ 2024–2026 AI 浪潮新增层；④ 决策树；⑤ 避坑 & 预算分层。
> 标注规则：一手 = 官方页 / 厂商文档；二手 = 评测/比较文（State of CSS、State of Design、Smashing/UX Collective、a16z）。
> **活跃度**列：取最近一次有公开记录的产品发布或大版本（来自 GitHub seed 的 `pushed_at` 与官方 changelog 已交叉核对，截至 2026-05-12）。
> AI 工具部分诚实标注 ⚠️**不稳定 / 结果质量参差**。

---

## A. 必备工具（canonical layer）

### A1. 设计 / Prototype 工具

#### 1. Figma ⭐⭐⭐
- URL: https://www.figma.com（一手）
- 简介：浏览器原生的协同设计 + 原型工具；2026 年仍是行业事实标准。Adobe 收购于 2023 年初被反垄断阻止后保持独立，2024–2026 节奏更快。
- 适用：线框、高保真、原型、design system、交付（Dev Mode）
- 定价：Free（3 个 Figma file + 3 FigJam）/ Professional $15/编辑者/月 / Organization $45/月 / Enterprise $75/月（一手 https://www.figma.com/pricing/）
- 局限：复杂矢量编辑弱于 Illustrator；中国大陆访问需自备网络（Figma 国内版"特通版"功能滞后）；Dev Mode 单独计费
- 活跃度：Config 2025（2025-05）发布 Sites / Buzz / Make / Draw / Grid；2026 Config 预定 5 月底（一手 https://config.figma.com/）；core app 周级更新

#### 2. Sketch ⭐
- URL: https://www.sketch.com（一手）
- 简介：2010 年代统治者，Mac-only 原生应用；2022 后推出 Web App 与协作，但份额持续被 Figma 蚕食
- 适用：纯 macOS 团队、不需要在线协作的小工作室、维护历史 .sketch 资产
- 定价：$10/月/编辑者；Mac-only 个人 license $120/年
- 局限：跨 OS 困难（Windows/Linux 团队无法编辑）；插件生态萎缩；招聘市场已很少要求会 Sketch
- 活跃度：2025 持续维护，发布节奏放缓

#### 3. Adobe XD 🪦
- URL: https://www.adobe.com/products/xd.html（一手）
- 状态：**不再 active development**。Adobe 于 2023 官方停止销售独立版，仅向 Creative Cloud 全家桶老订户提供
- 学习者建议：**不要学**

#### 4. Penpot ⭐⭐
- URL: https://penpot.app（一手；开源 https://github.com/penpot/penpot）
- 简介：开源 Figma 替代，基于 SVG/CSS 原生格式，可自托管；2024 推出 2.0、2025 推出 Plugins API、2026-Q1 推出 AI Components
- 适用：开源敏感团队、欧盟数字主权项目、希望自托管设计文件的企业
- 定价：完全免费 + 自托管；Penpot Cloud 团队版按席位计费（约 $7/月）
- 局限：动效/原型能力仍弱于 Figma；插件生态早期；招聘市场要求会 Penpot 的岗位很少
- 活跃度：2026-Q1 发布 v2.5（一手 https://penpot.app/blog）

#### 5. Framer ⭐⭐
- URL: https://www.framer.com（一手）
- 简介：2022 起从「设计原型」转型为「设计师 no-code 建站」；2024 加入 Framer AI 自然语言生成站点
- 适用：landing page、个人 portfolio、营销站；不再适合纯 UI 设计 / app prototype
- 定价：Free / Mini $5/月 / Basic $15/月 / Pro $30/月（按站点）
- 局限：与 Figma 不在同一赛道，新人若想做 UX 设计师**不要**用 Framer 替代 Figma
- 活跃度：2026 季度发布

#### 6. 中文圈 - MasterGo
- URL: https://mastergo.com（一手）
- 简介：字节出品的国产 Figma；2023 上线 AI 设计助手；2024 与 Semi Design 深度联动
- 适用：中国大陆团队（Figma 访问慢）、字节生态
- 定价：免费团队（3 编辑者）；Pro ¥588/编辑者/年
- 局限：插件生态远不及 Figma；海外团队几乎不用
- 活跃度：2026 季度更新；曾于 2024 年改名"摹客"

#### 7. 中文圈 - 即时设计 (jsdesign)
- URL: https://js.design（一手）
- 简介：另一国产 Figma 替代，2023 起加入 AI 模块、社区资源丰富
- 适用：中国大陆中小团队、设计模板下载
- 定价：免费个人；专业版 ¥168/年/编辑者
- 局限：企业级权限/审计弱
- 活跃度：每周更新（一手 changelog）

#### 8. 中文圈 - Pixso
- URL: https://pixso.cn（万兴 Wondershare 出品；一手）
- 简介：定位接近即时设计；强调"国内云存储 + Figma 兼容文件格式"
- 适用：受合规约束（数据本地化）的中国大陆团队
- 局限：海外市场无声量
- 活跃度：2025–2026 持续迭代

#### 9. Figma 国内版（特通版）
- URL: 限企业邀请；2024 起部分企业用户可申请
- 简介：Figma 与中国合作伙伴提供的镜像服务；性能改善，但功能滞后 1–2 个版本，**不含 AI 功能**
- 学习者建议：等到企业入职后再说，自学阶段直接用 mastergo / 即时设计

---

### A2. 协作 / 标注 / Handoff

#### 10. Figma Dev Mode ⭐⭐⭐
- URL: https://www.figma.com/dev-mode/（一手）
- 简介：2023 Config 推出，2024 起从 Inspect 升级为完整 Dev Mode（task 视图、对比模式、code connect、VS Code 插件）
- 适用：所有用 Figma 的开发交付场景
- 定价：$25/开发者/月（额外费用）
- 局限：仅对付费 seat 开放；中国大陆 Figma 国内版无 Dev Mode
- 活跃度：2025 起加 Code Connect（把 Figma 组件映射到代码组件）

#### 11. 蓝湖（Lanhu） ⭐⭐
- URL: https://lanhuapp.com（一手）
- 简介：中国大陆最普及的 handoff 工具，2018–2022 几乎是事实标准；后来推出"摹客 RP / DT"形成产品矩阵
- 适用：中国大陆 PM/前端/UI 协作；上传 Sketch/Figma/XD 文件自动生成切图与标注
- 定价：免费基础版；团队版 ¥299–999/年
- 局限：海外团队/外企用不上；产品节奏慢于 Figma Dev Mode
- 活跃度：2025–2026 持续，但战略重心已偏向 MasterGo

#### 12. Zeplin 🪦?
- URL: https://zeplin.io（一手）
- 简介：2017–2020 全球 handoff 第一名；2022 起被 Figma Dev Mode 蚕食市场份额
- 适用：仍维护老 Sketch / XD 项目的团队；Jira / Slack 深度集成场景
- 定价：Free（1 项目）/ Team $8/seat/月 / Org $12
- 局限：2023 后 Figma 用户已基本流失；招聘市场鲜少要求
- 活跃度：维护态，仍有更新但无亮点功能

#### 13. Avocode 🪦
- 已于 2022 关停，**不要学**

---

### A3. 原型 / 微交互 / 动效

#### 14. Figma Smart Animate + Variables ⭐⭐⭐
- 简介：原生原型层；2024 加入 Variables / Conditional Logic 后能做到 80% ProtoPie 能做的事
- 局限：复杂传感器/手势/外部数据仍要 ProtoPie 或代码

#### 15. ProtoPie ⭐⭐
- URL: https://www.protopie.io（一手）
- 简介：高保真原型 + 真实传感器 / 多设备联动；汽车 HMI / IoT / 复杂手势是其专长
- 适用：复杂交互原型、车机/家电 HMI、用户研究需要真实手感的测试
- 定价：Free / Pro $13/月 / Enterprise quote
- 局限：学习曲线陡；对纯 web/SaaS 项目 Figma 已够用

#### 16. Principle 🪦
- URL: https://principleformac.com
- 状态：Mac-only，2022 后基本停更；**不要学**

#### 17. Origami Studio ⭐
- URL: https://origami.design（Meta 一手）
- 简介：Meta 内部用的 patch-based 原型工具，免费 Mac 应用
- 适用：复杂动效逻辑、Meta 系生态从业者
- 局限：陡峭、文档稀少、协作弱
- 活跃度：2025 仍更新但社区小

#### 18. Rive ⭐⭐⭐
- URL: https://rive.app（一手）
- 简介：交互动画运行时；State Machine 让动画响应代码/输入；Web / iOS / Android / Flutter / Unity SDK
- 适用：产品里的真实交互动画（按钮 / 加载 / onboarding）
- 定价：Free（2 editor）/ Pro $20/月 / Org $45/月
- 局限：替代不了 After Effects 的长片头/影视动画
- 活跃度：2026-Q1 推出 Vector Feathering、Performance dashboards

#### 19. Lottie / LottieFiles ⭐⭐⭐
- URL: https://lottiefiles.com（一手）
- 简介：JSON 化 After Effects 动画；轻量、跨平台、可代码控制；几乎所有 mobile / web app 使用过 Lottie
- 适用：插画式动画、icon 动效、splash / empty state
- 定价：免费下载社区资源；Pro $25/月（私有库）
- 局限：交互响应弱（非 state machine），复杂逻辑用 Rive
- 活跃度：持续，2024 推出 dotLottie 格式（更紧凑）

#### 20. After Effects + Bodymovin
- 仍是动画师生产 Lottie 的工具链；不是 UI 设计师必学

---

### A4. 设计系统 / Component 库（来自 GitHub seed 验证）

| # | 名称 | URL | Stars (seed) | 最近 push | 适用 |
|---|------|-----|---|-----------|------|
| 21 | shadcn/ui ⭐⭐⭐ | https://ui.shadcn.com | (seed 外，但事实标准) | 周级 | 2024–2026 最猛增长；Tailwind + Radix + 复制粘贴模式 |
| 22 | Radix UI ⭐⭐⭐ | https://www.radix-ui.com | — | 持续 | unstyled accessible primitives；shadcn 的底座 |
| 23 | Material UI (MUI) | https://mui.com | 98.3k | 2026-05-12 | Google Material；最成熟 React 库；偏重 |
| 24 | Ant Design | https://ant.design | (seed 外，但行业第一中文系) | 周级 | 中国大陆 ToB / 中后台首选 |
| 25 | Tailwind UI / Catalyst | https://tailwindui.com | — | — | 付费组件 $299 one-time；Refactoring UI 作者出品 |
| 26 | Chakra UI | https://chakra-ui.com | 40.4k | 2026-05-12 | SaaS 友好；a11y 内建 |
| 27 | Mantine | https://mantine.dev | (seed 外) | 周级 | React + hooks + 文档质量极高 |
| 28 | DaisyUI | https://daisyui.com | 40.9k | 2026-05-06 | Tailwind 组件库；纯 CSS class |
| 29 | Base UI | https://base-ui.com | 9.5k | 2026-05-11 | Radix + MUI + Floating UI 团队联合作品 2024+ |
| 30 | HyperUI | https://hyperui.dev | 12k | 2026-05-11 | Tailwind v4 免费组件 |
| 31 | Flowbite | https://flowbite.com | 9.2k | 2026-04-03 | Tailwind + Figma 联动 |
| 32 | Carbon Design | https://carbondesignsystem.com | 9.1k | 2026-05-12 | IBM；企业级 |
| 33 | Primer | https://primer.style | 12.9k | 2026-05-11 | GitHub 设计系统 |
| 34 | Semi Design | https://semi.design | 9.8k | 2026-05-12 | 字节抖音；中文圈 + AI friendly + design-to-code |
| 35 | Material Web | https://material-web.dev | 10.9k | 2026-05-07 | Google 官方 Web Components |
| 36 | Reka UI (前 Radix Vue) | https://reka-ui.com | 6.4k | 2026-05-12 | Vue 用户的 Radix 等价物 |
| 37 | Storybook ⭐⭐⭐ | https://storybook.js.org | — | 周级 | 组件文档与可视化测试事实标准 |
| 38 | Tokens Studio (Figma plugin) | https://tokens.studio | — | — | 设计 token 桥接 Figma ↔ code |
| 39 | Style Dictionary (Amazon) | https://styledictionary.com | — | 持续 | token 多平台输出工具链 |
| 40 | Panda CSS | https://panda-css.com | 6k | 2026-05-08 | Chakra 团队出品，type-safe CSS-in-JS |

> seed 中还出现的同类候补：grommet / elastic EUI / Stencil / Rebass（已停更）/ React95（玩具）/ 98.css（玩具）— 不列入主推。

---

### A5. 用户研究 / 可用性

#### 41. Maze ⭐⭐⭐
- URL: https://maze.co（一手）
- 简介：无 moderation 的远程可用性测试；2024 加入 AI insights、2025 与 Figma 集成 prototype 测试
- 适用：早期产品验证、A/B prototype 测试、卡片分类
- 定价：Free / Starter $99/月 / Org $208/月
- 局限：定性深访仍要 Lookback / Dovetail

#### 42. UserTesting (含 Useberry) ⭐⭐
- URL: https://www.usertesting.com（一手）
- 简介：行业老牌；提供 panel + 录屏 + 分析
- 定价：报价制（中型团队约 $25k/年起），学习者用不起
- 局限：贵；学习者只能看公开案例

#### 43. Hotjar ⭐⭐
- URL: https://www.hotjar.com（一手；已被 Contentsquare 收购，2024 起整合）
- 简介：热力图 + 录屏 + 调研三合一
- 定价：Free（35 sessions/day）/ Plus $32/月 / Business $80/月
- 局限：录屏取样有上限；Pro 以下数据保留期短

#### 44. FullStory / LogRocket ⭐⭐
- URL: https://www.fullstory.com、https://logrocket.com
- 简介：行为录屏 + console replay；偏开发/产品分析
- 定价：均为企业报价，FullStory ~$1.5k/月起
- 学习者建议：开 trial 体验即可

#### 45. Lookback ⭐⭐
- URL: https://www.lookback.com（一手）
- 简介：moderated 远程访谈录制 + 标记
- 定价：Freelancer $25/月起；Insider $99/月
- 局限：2024 后 Dovetail / Maze 蚕食份额

#### 46. Dovetail ⭐⭐⭐
- URL: https://dovetail.com（一手）
- 简介：研究 repository + AI 标签自动化；2024 推出 Dovetail AI（auto tagging / theme extraction）
- 定价：Free / Pro $39/编辑者/月 / Team $79
- 活跃度：a16z 与 NN/g 多次点名为 2025 研究工具榜首

#### 47. Optimal Workshop
- URL: https://www.optimalworkshop.com（一手）
- 简介：卡片分类、树测试、first-click 测试老牌
- 定价：Free / Individual $208/月 / Team $278/月（年付）
- 局限：UI 老化但功能扎实

#### 48. Notion / Airtable
- 研究档案 + insight repository 的低成本起步方案
- 定价：Notion Free / Plus $10/月；Airtable Free / Team $20/月

---

### A6. Accessibility / a11y 测试

#### 49. axe DevTools ⭐⭐⭐
- URL: https://www.deque.com/axe/（一手）
- 简介：Deque 出品，事实标准；Chrome / Firefox / Edge / CLI / CI 全套
- 定价：浏览器扩展免费；Pro $40/月（智能引导测试）
- 活跃度：周级；2025 推出 axe DevTools Linter

#### 50. Stark (Figma plugin) ⭐⭐
- URL: https://www.getstark.co（一手）
- 简介：Figma 内对比度 / a11y 检查；2024 推出 AI a11y review
- 定价：Free / Pro $15/月 / Team $50/月

#### 51. WAVE
- URL: https://wave.webaim.org（一手 WebAIM）
- 简介：免费在线 a11y 评估；学院派

#### 52. Lighthouse a11y audit
- 内嵌于 Chrome DevTools；最低门槛 a11y baseline

#### 53. Polypane ⭐⭐
- URL: https://polypane.app（一手）
- 简介：开发者向多视口同步浏览器，内建 a11y / SEO / 性能 audit
- 定价：Personal $9/月 / Team $29/月

#### 54. Contrast (color checker)
- URL: https://usecontrast.com（macOS app）
- WebAIM Contrast Checker https://webaim.org/resources/contrastchecker/（免费在线）

---

### A7. 灵感 / Reference

#### 55. Mobbin ⭐⭐⭐
- URL: https://mobbin.com（一手）
- 简介：500+ app + web 流程截图库，按 pattern 检索；2024 加入 AI 搜索
- 定价：Free（限量）/ Pro $39/月 / Team $69
- 学习者必装：找 onboarding / pricing / empty state 真实参考最快

#### 56. Land-book / Httpster
- URL: https://land-book.com、https://httpster.net
- 免费 landing page / 站点设计 inspiration

#### 57. Page Flows ⭐⭐
- URL: https://pageflows.com（一手）
- 简介：完整 user flow 视频；标注每一步触发条件
- 定价：Pro $42/月

#### 58. Refero / Calltoidea
- URL: https://refero.design、https://www.calltoidea.com
- 按 UI element 检索

#### 59. Awwwards / SiteInspire
- URL: https://www.awwwards.com、https://www.siteinspire.com
- 视觉/创意站点榜单；偏 marketing 站

---

### A8. AI 设计工具（2024-2026 新增层，⚠️不稳定）

> ⚠️ **诚实警告**：本节工具迭代极快，本节内容可能在 3–6 个月后大幅变化；结果质量参差，**适合早期探索，不适合代替细节打磨**。

#### 60. v0 by Vercel ⭐⭐⭐
- URL: https://v0.dev（一手）
- 简介：文字 prompt → React + Tailwind + shadcn 代码；2024 起从纯 UI 生成扩展到全栈
- 定价：Free / Premium $20/月 / Team $30/编辑者/月
- 适用：开发者快速搭组件；设计师做 hi-fi 探索
- 局限：⚠️ 设计师视角下"看起来对"的代码常需大量手调；非 React 团队收益小
- 活跃度：周级；2025 推出 v0 chat、2026-Q1 推出 v0 fullstack

#### 61. Lovable ⭐⭐
- URL: https://lovable.dev（一手；前身 GPT Engineer App）
- 简介：自然语言 → 完整 web app（含数据库 Supabase）；2024-Q4 爆红
- 定价：Free / Starter $20/月 / Launch $50/月
- 局限：⚠️ 适合 MVP demo，不适合生产级；UI 趋同 (shadcn 风)
- 活跃度：周级

#### 62. Bolt.new (StackBlitz) ⭐⭐
- URL: https://bolt.new（一手）
- 简介：浏览器内 AI full-stack；in-browser WebContainer 直接跑
- 定价：Free / Pro $20/月 / Pro 50 $50/月
- 活跃度：2024 末爆红后保持快速迭代

#### 63. Figma Make / Figma AI ⭐⭐
- URL: 内嵌于 Figma；2025 Config 推出 Make Designs / First Draft / Visual Search
- 适用：Figma 用户直接在编辑器内 prompt 出初稿
- 定价：包含在 Figma 订阅
- 局限：⚠️ 2024 曾下线 Make Designs（被发现复制现有 app）；2025 复出 + Make
- 活跃度：随 Figma Config 节奏

#### 64. Galileo AI (现并入 Google Stitch) ⭐
- URL: https://stitch.withgoogle.com（一手）
- 简介：2024 被 Google 收购，并入 Stitch (Google Labs)；text → UI 设计 + 导出 Figma
- 状态：仍 Labs 阶段；⚠️ 不稳定

#### 65. Uizard ⭐
- URL: https://uizard.io（一手）
- 简介：手绘草图 → UI / wireframe → mockup；2024 加入 Autodesigner 2.0
- 定价：Free / Pro $19/月 / Business $39/月
- 局限：⚠️ 输出质量低于 v0；适合早期 wireframe

#### 66. Magician for Figma ⭐
- URL: https://magician.design（一手）
- 简介：Figma 插件，AI 生成 icon / copy / image
- 定价：one-time $14
- 状态：2023 起未更新，⚠️ 接近停滞

#### 67. Visily ⭐
- URL: https://www.visily.ai（一手）
- 简介：sketch / screenshot → editable wireframe / mockup
- 定价：Free / Pro $9/月
- 局限：⚠️ 适合 PM 出原型沟通，不适合做交付

#### 68. Cursor + Tailwind workflow ⭐⭐⭐
- URL: https://www.cursor.com（一手）
- 简介：不是设计工具，但 2024–2026 已成 design engineer 标配；与 shadcn + Tailwind 配合实现"prompt → polished UI"
- 定价：Free / Pro $20/月 / Business $40/月
- 学习者建议：UI 设计师转 design engineer 的捷径

---

### A9. 字体 / Icon

#### 69. Google Fonts
- URL: https://fonts.google.com — 免费、CDN、Variable Fonts 支持

#### 70. Adobe Fonts (Typekit)
- URL: https://fonts.adobe.com — 包含在 Adobe CC 订阅

#### 71. Icon 库（全部免费 + 开源）
- Phosphor https://phosphoricons.com — 6 weight；设计师友好
- Lucide https://lucide.dev — Feather 分叉；shadcn 默认
- Heroicons https://heroicons.com — Tailwind 团队
- Tabler Icons https://tabler.io/icons — 5000+ outline / filled
- Remix Icon https://remixicon.com — 中文圈最常用
- SF Symbols https://developer.apple.com/sf-symbols/ — Apple 平台

#### 72. 中文字体
- 思源系列（Source Han Sans / Serif）— Adobe + Google 开源
- 阿里巴巴普惠体 — 阿里官方开源
- 站酷字体（Quanyi）— 商用免费
- 霞鹜文楷 — 开源中文衬线

---

## B. 选型决策树（8 条）

1. **新人第一款工具 → Figma Free**
   理由：行业 80%+ 招聘需求；社区资源最多；浏览器即开；不要犹豫。

2. **团队设计系统 → Figma + Tokens Studio + Storybook (+ shadcn/ui 如果是 React)**
   理由：Tokens Studio 桥接 Figma 与代码；Storybook 是组件文档事实标准；shadcn 让团队拥有源码不被锁定。

3. **Solo freelancer (~$30/月) → Figma Pro $15 + Mobbin Pro $39（任选一）+ axe 免费**
   理由：客户协作必须 Pro；Mobbin 是接单时的"看了别人怎么做"加速器。

4. **中国大陆团队（Figma 访问慢）→ 即时设计 / MasterGo + 蓝湖**
   理由：网络稳定；中文模板与 ICP 合规友好；handoff 在国内开发链路里仍多用蓝湖。

5. **协作给开发 → Figma Dev Mode + Storybook + Code Connect**
   理由：Dev Mode 让开发看到组件而非图像；Code Connect 直接把 Figma 组件映射代码组件。

6. **微动效 / 复杂交互 → 先用 Figma Variables，复杂时升级 Rive 或 ProtoPie**
   理由：80% 场景 Figma 已够；动画交付到产品里用 Rive（state machine）；纯插画动画用 Lottie。

7. **用户研究 budget < $100 → Maze Starter $99 + Notion 免费档案**
   理由：远程 unmoderated 测试覆盖 80% 需求；deep research 暂用 Google Meet 录屏 + Notion 笔记。

8. **AI 加速早期探索 → v0 (React) 或 Figma Make**
   理由：30 分钟生成 5 个方向比手工搭快；但 **不要** 让 AI 替代细节打磨与可用性测试。

---

## C. 新兴 / 实验（近 12 个月）

- **shadcn 生态爆炸**：registry 系统（2024-Q4）让任何团队可以发布自己的 component registry；2026 已成 React design system 的"分发协议"，类似 npm 之于包
- **Design-to-Code 浪潮**：v0 / Lovable / Bolt.new / Figma Make 同质化竞争；State of Design 2025 报告显示 41% 的从业者已在工作流中使用至少一款
- **Figma 平台化**：2025 Config 发布 Sites / Slides / Buzz / Draw / Grid / Make，从单工具变多产品矩阵；2026 Config 预定 5 月底
- **Penpot 与开源替代**：2.x 系列 + AI Components 让自托管设计成为欧盟数字主权的现实选项
- **DESIGN.md 规范化**：VoltAgent/awesome-design-md（seed: 75k stars, 2026-03 创建）— 把品牌设计系统写成 DESIGN.md 文件喂给 coding agent，"vibe-design" 新兴
- **Base UI**：Radix + MUI + Floating UI 团队 2024 合并产物；2026 已成新一代 unstyled primitives 候选
- **Dovetail AI**：研究 repository + 自动主题提取，2024–2026 抢占 Lookback / Notion 笔记的市场

---

## D. 避坑清单

1. **不要学 Adobe XD**：2023 已停止 active development，所有招聘已转 Figma
2. **不要从 Photoshop 入手做 UI**：Photoshop 不是 UI 工具，2010 年代后行业共识；用 Figma
3. **不要在跨 OS 团队选 Sketch**：Windows/Linux 同事打不开 .sketch
4. **蓝湖**在外企 / 海外团队**用不上**：要么 Figma Dev Mode 要么 Storybook
5. **ProtoPie 学习曲线**远高于 Figma Smart Animate：大多场景 Figma Variables 已够，不要为了"高级"花 40 小时学 ProtoPie
6. **AI 工具适合早期探索，不适合细节打磨**：v0 / Lovable 的输出在 80% 完成度后边际成本陡升
7. **不要选 Principle / Magician / Avocode 等停更工具**：2022–2023 已被时间淘汰
8. **不要把 Framer 当 Figma 用**：Framer 已是 no-code 建站工具，不是 UI 设计工具
9. **不要为了"工具齐全"上 Adobe 全家桶**：UI 设计师仅需 Figma + 1–2 个补丁工具，月费可控
10. **不要相信"Figma 国内版完全等价"**：功能滞后 + 无 AI；正式工作前再说

---

## E. 工具栈预算分层

### E1. 学习者 / 学生（$0/月）
- Figma Free
- shadcn/ui + Storybook（开源）
- axe DevTools 浏览器扩展
- Mobbin Free（限量浏览）
- Phosphor / Lucide / Heroicons
- Google Fonts
- Notion Free（研究笔记）
- WebAIM Contrast Checker

### E2. Solo freelancer（~$30/月）
- Figma Professional $15
- Mobbin Pro $39（任选一周期付 / 月付）—— 或 Page Flows
- Stark Pro $15 / Polypane $9
- LottieFiles Free
- Cursor Free
- 合计：~$30–60/月

### E3. 小团队 ($200-500/月，5 人)
- Figma Org $45 × 5 + 1 Dev Mode = ~$250
- Maze Starter $99
- Hotjar Plus $32
- Dovetail Pro $39 × 2 = $78
- Stark Team $50
- Storybook（开源）+ Cursor Pro $20
- 合计：~$500/月

### E4. 企业 / 设计系统团队（$2k+/月）
- Figma Enterprise $75 × N
- Dovetail Team $79 × N
- axe DevTools Pro $40 × QA
- UserTesting / FullStory（企业报价 $1.5k+）
- Tokens Studio Pro / Specify
- Polypane / Storybook hosting (Chromatic) $149+

---

## 信源附录

**一手**（官方页 / 厂商）：所有 URL 上标注（一手）的条目；GitHub seed 数据。

**二手**：
- a16z 2024–2025 Generative AI Market Map (consumer & creative)
- State of Design 2025 (UX Tools Survey by Taylor Palmer & Jordan Bowman, https://uxtools.co/survey)
- Smashing Magazine tools roundups（一手编辑 + 调研，2024–2026）
- UX Collective 年度工具盘点
- Brad Frost / Khoi Vinh 等业内人 blog 评论

**黑名单**：本文档**未引用**知乎、微信公众号、百度、CSDN（除作者本人专栏）、SEO 内容农场。
