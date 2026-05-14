# Track 06: Glossary — Web UI/UX Design

last_updated: 2026-05-12
term_count: 92
standard_count: 9
regulation_count: 5
language: EN + 中文对照
audience: 想入行 Web UI/UX 设计的中文学习者

调研说明：
- 优先官方定义（W3C、NN/g、ISO、Apple/Google/Microsoft 官方设计规范、原作者）
- 经典著作次之（Don Norman、Jakob Nielsen、Steve Krug、Brad Frost 等）
- 不引用知乎 / 微信公众号 / 百度百科 / 内容农场
- 过时但学习者仍会遇到的术语标记 `[deprecated]` 但保留
- 标准版本：**WCAG 2.2 (2023-10) 已为当前 W3C Recommendation；WCAG 3.0 仍为 Working Draft（2026 年未 Rec）**

---

## A. 高频黑话 / 术语词典

### A1. 设计思维 / 流程 (Design Thinking & Process)

| EN | 中文 | 1-句定义 | 出处 |
|---|---|---|---|
| **Affordance** | 可供性 / 示能 | 物体的属性暗示用户它能被如何使用（如按钮的"凸起"暗示"可按"）。 | Don Norman《The Design of Everyday Things》(1988)，原概念来自心理学家 J.J. Gibson (1977) |
| **Signifier** | 指示符 | 让 affordance 被用户感知的可见线索（如下划线 = 链接）。 | Don Norman, 后期版本 DOET (2013) 引入此词区分 affordance |
| **Mental Model** | 心智模型 | 用户脑中关于"系统如何工作"的认知模型。 | Kenneth Craik (1943); UX 语境见 Indi Young《Mental Models》(2008) |
| **Conceptual Model** | 概念模型 | 设计师在产品中呈现的"系统如何工作"的模型；目标是与用户心智模型对齐。 | Don Norman, DOET |
| **Jobs-to-be-Done (JTBD)** | 用户要完成的任务 | 用户"雇佣"一个产品来完成的功能/情感/社会"工作"。 | Clayton Christensen, HBS (2003)；Tony Ulwick 提出 ODI 方法论 |
| **Design Thinking** | 设计思维 | 以用户为中心的迭代式问题求解方法论（共情→定义→构思→原型→测试）。 | IDEO / d.school Stanford；David Kelley 推广 |
| **Double Diamond** | 双钻模型 | 设计流程的四阶段模型：Discover→Define→Develop→Deliver。 | UK Design Council (2004) |
| **Lean UX** | 精益 UX | 假设驱动、最小可行设计、快速迭代的 UX 工作方式。 | Jeff Gothelf《Lean UX》(2013, O'Reilly) |
| **Design Sprint** | 设计冲刺 | 5 天内从问题到原型到验证的结构化流程。 | Jake Knapp, Google Ventures《Sprint》(2016) |
| **Hypothesis-Driven Design** | 假设驱动设计 | 把每个设计决策写成可证伪的假设并测试。 | Lean UX (Gothelf) |
| **HCD (Human-Centered Design)** | 以人为本的设计 | 围绕人的需求、能力、行为来设计产品的方法论。 | ISO 9241-210:2019 给出正式定义 |
| **Discovery** | 需求发现 / 探索期 | 项目初期的用户与场景研究阶段。 | UK Design Council Double Diamond |

### A2. 交互 / 可用性 (Interaction & Usability)

| EN | 中文 | 1-句定义 | 出处 |
|---|---|---|---|
| **Heuristic Evaluation** | 启发式评估 | 由专家对照一组通用原则评估界面可用性。 | Jakob Nielsen (1990)，NN/g 10 Usability Heuristics |
| **Nielsen's 10 Heuristics** | 尼尔森十大可用性原则 | 系统状态可见、匹配真实世界、用户控制、一致性、防错、识别优于回忆、灵活高效、美观极简、错误恢复、帮助文档。 | Jakob Nielsen (1994, 2024 修订)，nngroup.com |
| **Usability Testing** | 可用性测试 | 让真实用户完成任务，观察可用性问题。 | Jakob Nielsen《Usability Engineering》(1993) |
| **Cognitive Load** | 认知负荷 | 用户完成任务时大脑工作记忆的占用量。 | John Sweller (1988) Cognitive Load Theory |
| **Hick's Law** | 希克定律 | 选项越多，决策时间越长（对数关系）。 | Hick (1952), Hyman (1953) |
| **Fitts's Law** | 菲茨定律 | 移动到目标的时间 = f(距离, 目标尺寸)。 | Paul Fitts (1954) |
| **Miller's Law** | 米勒定律 | 短时记忆容量约 7±2 项（常被误用作"UI 应只放 7 个选项"）。 | George Miller (1956) |
| **Gestalt Principles** | 格式塔原则 | 接近、相似、连续、闭合、共同命运等视觉组织规律。 | Wertheimer, Koffka, Köhler 等（1920s 柏林学派） |
| **F-Pattern** | F 型阅读模式 | 长文本网页用户视线呈 F 型扫读。 | Jakob Nielsen, NN/g 眼动研究 (2006) |
| **Z-Pattern** | Z 型扫读模式 | 视觉稀疏页面（如 landing page）用户视线呈 Z 型。 | UX folklore，非严格学术原始来源 |
| **Progressive Disclosure** | 渐进式呈现 | 先显示主要选项，次要选项按需展开。 | Jakob Nielsen, NN/g |
| **Microinteraction** | 微交互 | 单一目的的小型交互（点赞动效、表单校验提示）。 | Dan Saffer《Microinteractions》(O'Reilly, 2013) |
| **Dark Pattern** | 暗黑模式 / 欺骗式设计 | 故意诱导用户做出违背自身利益选择的 UI。 | Harry Brignull (2010), deceptive.design；欧盟 DSA、加州 CCPA 已立法 |
| **Friction** | 摩擦 | 阻碍用户达成目标的任何阻力（既可坏也可好，如付款确认） |UX 通用术语 |
| **Affordance Cue** | 示能线索 | 见 Signifier。 | — |
| **Error Prevention** | 防错设计 | 通过约束、确认、撤销减少用户犯错。 | Nielsen Heuristic #5 |
| **System Status Visibility** | 系统状态可见性 | 让用户随时知道系统正在发生什么。 | Nielsen Heuristic #1 |
| **Don't Make Me Think** | "别让我思考" | 网页可用性的核心口号：让操作显而易见。 | Steve Krug《Don't Make Me Think》(2000, 3rd ed. 2014) |

### A3. 视觉 / 排版 (Visual & Typography)

| EN | 中文 | 1-句定义 | 出处 |
|---|---|---|---|
| **Visual Hierarchy** | 视觉层级 | 通过大小、颜色、位置引导视线先看什么后看什么。 | 平面设计经典；Robin Williams《The Non-Designer's Design Book》(1994) |
| **Contrast** | 对比 | 通过差异（色彩、大小、形状）创造区分。 | Robin Williams CRAP 原则之一 |
| **White Space / Negative Space** | 留白 / 负空间 | 元素之间的空白区域，承担呼吸与分组功能。 | 平面设计基础；Jan Tschichold 等 |
| **Grid System** | 网格系统 | 用列与基线对齐内容的结构。 | Josef Müller-Brockmann《Grid Systems in Graphic Design》(1981) |
| **Baseline Grid** | 基线网格 | 文本基线对齐的水平线网格。 | 排印学经典 |
| **Modular Scale** | 模块化排版比例 | 按比例（如 1.25, 黄金比 1.618）派生字号体系。 | Tim Brown《Modular Scale》(2011) |
| **Kerning / Tracking / Leading** | 字距微调 / 字间距 / 行距 | 字母对间距 / 整体字间距 / 行间距。 | 排印学经典术语 |
| **x-Height** | x 字高 | 小写字母（如 x）的高度，影响可读性。 | 排印学 |
| **Color Theory** | 色彩理论 | 色相、明度、饱和度及配色关系。 | Johannes Itten《The Art of Color》(1961) |
| **HSL / HSB** | HSL/HSB 色彩模型 | Hue/Saturation/Lightness 或 Brightness——更接近人类感知。 | W3C CSS Color Module |
| **OKLCH / OKLab** | OKLCH 色彩空间 | 感知均匀的现代色彩空间，2026 年设计系统主流。 | Björn Ottosson (2020)；CSS Color 4 (W3C) |
| **Semantic Color** | 语义色彩 | 按用途命名颜色（success/danger/primary）而非视觉值。 | 设计系统通用实践，Material/Carbon/HIG 均采用 |
| **Perceived Brightness** | 感知亮度 | 人眼对亮度的非线性感知（不等于 RGB 平均）。 | 色彩科学 |
| **Optical Alignment** | 视觉对齐 | 为弥补几何对齐的视觉偏差做的微调。 | 排印学传统 |
| **Skeuomorphism** `[deprecated 但仍流行回潮]` | 拟物化 | 用现实材质模仿物理物体的视觉风格（如 iOS 6 的皮革纹）。 | iOS 6 (2012) 顶峰；2024-2026 因 Apple Liquid Glass 部分回归 |
| **Flat Design** | 扁平化设计 | 去除拟物阴影与渐变的极简风格。 | Microsoft Metro (2010), iOS 7 (2013) |
| **Neumorphism** | 新拟物 | 同色背景上用柔和阴影制造浮起感的风格。 | Michal Malewicz (2019)，Dribbble 短期流行 |

### A4. 设计系统 / 组件 (Design Systems)

| EN | 中文 | 1-句定义 | 出处 |
|---|---|---|---|
| **Design Tokens** | 设计令牌 | 命名化、可被代码消费的设计决策（色值、间距、字号等）。 | Salesforce Lightning (2014)；W3C Design Tokens Community Group spec (草案) |
| **Primitive Tokens / Semantic Tokens / Component Tokens** | 原始令牌 / 语义令牌 / 组件令牌 | 三层 token 架构：原始值 → 语义角色 → 组件专用。 | Nathan Curtis (EightShapes)；Material Design 3 体系 |
| **Atomic Design** | 原子化设计 | 把 UI 拆为 atoms / molecules / organisms / templates / pages。 | Brad Frost《Atomic Design》(2016)，atomicdesign.bradfrost.com |
| **Component Library** | 组件库 | 可复用 UI 组件的集合（代码 + 设计）。 | Storybook 等工具普及该实践 |
| **Single Source of Truth (SSOT)** | 单一可信源 | 设计令牌与组件定义在一个地方维护，被所有平台消费。 | 软件工程通用术语，设计系统沿用 |
| **Design API** | 设计 API | 把组件 props/variants 当作面向设计师的 API。 | Nathan Curtis 等 design ops 圈子用语 |
| **Design Ops** | 设计运营 | 用流程、工具、治理放大设计团队产能。 | DesignOps Summit (NN/g)；Kristin Skinner & Dave Malouf 推广 |
| **Design QA** | 设计走查 / 设计验收 | 实现完成后对照设计稿检查偏差的过程。 | 行业通用实践 |
| **Handoff** | 交付 | 设计稿交给开发的过程（Figma Dev Mode、Zeplin 等支持）。 | 行业通用 |
| **Redlines** | 红线标注 | 在设计稿上标注尺寸/间距的传统做法。 | 平面设计传统术语 |
| **Component Variants** | 组件变体 | 同一组件的不同形态（size/state/intent）。 | Figma Variants 概念普及 |
| **Slot / Composition** | 插槽 / 组合 | 让组件容纳任意子内容的模式。 | Web Components / React 等技术名词渗入设计语言 |
| **Headless UI / Unstyled Components** | 无头 UI | 提供行为但不提供视觉的组件库（Radix、Headless UI、shadcn/ui）。 | 2022-2026 主流模式 |
| **Theming** | 主题化 | 通过切换 token 让同一组件适配多品牌/暗色模式。 | Material/Carbon/Fluent 均支持 |

### A5. 信息架构 / 内容 (Information Architecture)

| EN | 中文 | 1-句定义 | 出处 |
|---|---|---|---|
| **Information Architecture (IA)** | 信息架构 | 信息的组织、标签、导航与搜索系统设计。 | Peter Morville & Louis Rosenfeld《Information Architecture for the Web》(1998, 4th ed. 2015) |
| **Card Sorting** | 卡片分类 | 让用户对内容卡片分组以揭示其心智分类。 | Donna Spencer《Card Sorting》(Rosenfeld, 2009) |
| **Tree Testing** | 树测试 | 反向验证 IA：给任务让用户在层级树中找位置。 | Optimal Workshop 推广 |
| **Taxonomy** | 分类法 | 内容的层级分类体系。 | 图书馆学；UX 沿用 |
| **Navigation Pattern** | 导航模式 | 顶栏、侧栏、抽屉、Tab、Mega-menu 等。 | UI Patterns (Welie 等模式库) |
| **Breadcrumb** | 面包屑 | 显示当前位置在层级中的路径。 | UX 模式 |
| **Mega-menu** | 大型菜单 | 一次展开多列内容的下拉菜单。 | NN/g 研究术语 |
| **Faceted Search** | 分面搜索 / 多面搜索 | 按多个属性维度过滤结果。 | 图书馆学 → 电商普及 |

### A6. 可访问性 / 包容性 (Accessibility & Inclusion)

| EN | 中文 | 1-句定义 | 出处 |
|---|---|---|---|
| **a11y** | 无障碍（缩写） | "accessibility" 的数字缩写（a + 11 letters + y）。 | 行业惯例 |
| **WCAG 2.2** | Web 内容无障碍指南 2.2 | 当前 W3C Recommendation（2023-10-05），新增 9 条 success criteria（focus appearance、dragging movement、target size 等）。 | W3C, w3.org/TR/WCAG22/ |
| **WCAG 3.0** | WCAG 3.0 草案 | 仍为 W3C Working Draft（截至 2026），引入"评分"模型替代 A/AA/AAA。 | W3C, w3.org/TR/wcag-3.0/ |
| **AA vs AAA** | 双 A / 三 A 合规级别 | WCAG 三个一致性级别：A (最低) / AA (法规通用门槛) / AAA (最高)。 | W3C WCAG |
| **ARIA (WAI-ARIA 1.2)** | 无障碍富互联网应用 | 为动态/JS 内容添加语义的属性集（role、aria-label 等）。 | W3C WAI-ARIA 1.2 (Recommendation, 2023-06) |
| **Screen Reader** | 屏幕阅读器 | 把屏幕内容朗读给视障用户（JAWS、NVDA、VoiceOver、TalkBack）。 | — |
| **Contrast Ratio** | 对比度 | 前景与背景亮度比，WCAG 2.2 AA 正文要求 ≥ 4.5:1。 | WCAG 1.4.3 |
| **APCA** | 高级感知对比度算法 | WCAG 3 草案候选的新对比度算法，更贴近人眼感知。 | Andrew Somers, github.com/Myndex/SAPC-APCA |
| **Focus Indicator** | 焦点指示器 | 键盘聚焦时的可见高亮。 | WCAG 2.4.7 + 2.4.11 (2.2 新增 Focus Not Obscured) |
| **Keyboard Navigation** | 键盘可达 | 所有功能都能纯键盘操作。 | WCAG 2.1.1 |
| **Inclusive Design** | 包容性设计 | 主动设计覆盖能力差异的用户群。 | Microsoft Inclusive Design Toolkit (2016) |
| **Universal Design** | 通用设计 | 设计可被尽可能多人使用，无需特殊改造。 | Ron Mace, NC State Center for Universal Design (1997) |
| **Alt Text** | 替代文本 | 图像的文本描述，供屏幕阅读器与图像加载失败时使用。 | HTML 标准；WCAG 1.1.1 |
| **Skip Link** | 跳转链接 | 让键盘用户跳过重复导航直达主内容。 | WCAG 2.4.1 |
| **Reduced Motion** | 减少动效 | 用户系统级偏好；CSS `prefers-reduced-motion` 媒体查询。 | W3C Media Queries Level 5 |

### A7. 响应式 / 跨端 (Responsive & Cross-Platform)

| EN | 中文 | 1-句定义 | 出处 |
|---|---|---|---|
| **Responsive Web Design (RWD)** | 响应式设计 | 用流式网格 + 媒体查询 + 弹性图片让布局适应屏幕。 | Ethan Marcotte, A List Apart (2010) |
| **Adaptive Design** | 自适应设计 | 服务端/前端按断点切换若干固定布局（区别于流式 RWD）。 | Aaron Gustafson《Adaptive Web Design》(2011) |
| **Mobile-First** | 移动优先 | 先为最小屏幕设计再向上扩展。 | Luke Wroblewski《Mobile First》(A Book Apart, 2011) |
| **Breakpoint** | 断点 | 布局切换的屏幕宽度临界值。 | RWD 术语 |
| **Fluid Grid** | 流式网格 | 用百分比/fr 而非固定像素的网格。 | Marcotte RWD |
| **Container Query** | 容器查询 | 按父容器尺寸而非视口尺寸响应。 | W3C CSS Containment 3 (2023 进入 Baseline) |
| **Viewport** | 视口 | 浏览器中网页的可视区域。 | W3C CSS Viewport |
| **Touch Target** | 触摸目标 | 可被手指点击的区域，WCAG 2.2 AA 要求 ≥ 24×24 CSS px，Apple HIG 推荐 44pt，Material 推荐 48dp。 | WCAG 2.5.8；Apple HIG；Material Design |
| **Safe Area** | 安全区 | 避开刘海/底部 home indicator 的可用区域（iOS `safe-area-inset-*`）。 | Apple HIG / CSS env() |
| **Intrinsic Web Design** | 内在式 web 设计 | 用 CSS Grid 等"内在"能力替代固定断点的响应方法。 | Jen Simmons (2018) |

### A8. 流程 / 协作 (Process & Collaboration)

| EN | 中文 | 1-句定义 | 出处 |
|---|---|---|---|
| **Wireframe** | 线框图 | 不含视觉细节、聚焦结构与布局的低保真草图。 | UX 通用 |
| **Lo-fi Mockup** | 低保真稿 | 灰度 / 占位文本的初步视觉稿。 | — |
| **Hi-fi Mockup** | 高保真稿 | 接近最终视觉的精确稿。 | — |
| **Prototype** | 原型 | 可交互的设计稿（点击 / 跳转 / 状态切换）。 | — |
| **User Flow** | 用户流程 | 用户在产品中达成目标的路径图。 | — |
| **Journey Map** | 用户旅程地图 | 跨触点、跨时间的用户体验全景（含情绪曲线）。 | Adaptive Path (Jim Kalbach《Mapping Experiences》, O'Reilly 2016) |
| **Persona** | 人物画像 | 代表目标用户群的虚构角色。 | Alan Cooper《The Inmates Are Running the Asylum》(1999) |
| **Empathy Map** | 共情地图 | Says/Thinks/Does/Feels 四象限工具。 | Dave Gray, XPLANE (2009) |
| **Jobs Story** | 任务故事 | "当 [情境] 时，我想要 [动机]，以便 [期望结果]"的格式。 | Intercom《Jobs Stories》, Alan Klement |
| **Design Critique** | 设计评审 / 设计批评 | 团队对设计稿提供结构化反馈的会议。 | Adam Connor & Aaron Irizarry《Discussing Design》(O'Reilly, 2015) |
| **Design System Governance** | 设计系统治理 | 决策谁能改 token / 加组件 / 弃用 API 的机制。 | DesignOps 圈术语 |
| **RITE Method** | RITE 方法 | Rapid Iterative Testing & Evaluation——边测边改的可用性测试。 | Medlock et al., Microsoft (2002) |

### A9. 度量 (Metrics)

| EN | 中文 | 1-句定义 | 出处 |
|---|---|---|---|
| **NPS (Net Promoter Score)** | 净推荐值 | "0-10 你会推荐 X 吗"-> 推荐者% - 贬损者%。 | Fred Reichheld, HBR (2003) |
| **SUS (System Usability Scale)** | 系统可用性量表 | 10 题 Likert 量表，得分 0-100，>68 为平均以上。 | John Brooke (1986)，公开免费 |
| **Task Success Rate** | 任务完成率 | 用户成功完成既定任务的比例。 | 可用性测试基础指标 |
| **Time on Task** | 任务耗时 | 完成任务的时长。 | 可用性测试基础指标 |
| **Error Rate** | 错误率 | 任务中出错的次数 / 比例。 | 可用性测试 |
| **Conversion Rate** | 转化率 | 完成目标行为的用户占比。 | 通用增长指标 |
| **Retention** | 留存 | 一段时间后仍使用产品的用户比例。 | — |
| **Engagement** | 参与度 | DAU/MAU、停留时长、行为深度等综合衡量。 | — |
| **North Star Metric** | 北极星指标 | 反映用户从产品获得核心价值的单一指标。 | Sean Ellis (Amplitude) |
| **HEART Framework** | HEART 框架 | Happiness/Engagement/Adoption/Retention/Task success 五维度。 | Kerry Rodden et al., Google (CHI 2010) |
| **PULSE Metrics** | PULSE 指标 | Page views/Uptime/Latency/Seven-day active users/Earnings——传统业务指标，HEART 的对照面。 | Google, 同 HEART 论文 |

---

## B. 行业标准 / 框架 (Standards & Frameworks)

| 标准 | 当前版本 (2026-05) | 维护方 | 备注 |
|---|---|---|---|
| **WCAG (Web Content Accessibility Guidelines)** | **2.2 (W3C Recommendation, 2023-10-05)** | W3C WAI | 全球无障碍法规默认引用基准；**3.0 仍为 Working Draft**，未推荐 |
| **WAI-ARIA** | **1.2 (Recommendation, 2023-06)** | W3C WAI | 动态内容的可访问语义；**1.3 在 Editor's Draft** |
| **ISO 9241-210** | **2019** | ISO | "Human-centred design for interactive systems" 国际标准 |
| **ISO 9241-11** | **2018** | ISO | 可用性正式定义：effectiveness + efficiency + satisfaction |
| **Material Design** | **Material 3 (Material You) + Material 3 Expressive (2025-05 发布)** | Google | 含动态色彩、Expressive 强调情感化排印与动效 |
| **Apple Human Interface Guidelines (HIG)** | **iOS 26 / Liquid Glass (2025-09 起)** | Apple | 引入 Liquid Glass 材质层；macOS、watchOS、visionOS 同步更新 |
| **Microsoft Fluent** | **Fluent 2 (2023 至今)** | Microsoft | Web/Windows/Office 统一 |
| **IBM Carbon** | **Carbon v11 (2024 起 maintained)** | IBM | 企业级开源设计系统，含 React/Angular/Vue/Web Components |
| **Ant Design** | **v5.x (持续更新中, 2026 主线)** | 蚂蚁集团 | 中文圈最常引用的 B 端设计语言 |
| **Arco Design** | **v2.x** | 字节跳动 | 同上 |
| **Element Plus** | **2.x** | 饿了么 / 社区 | Vue 3 生态主流 UI 库 |
| **Design Tokens W3C Spec** | **Editor's Draft (Community Group)** | W3C DTCG | tokens 跨工具互操作的 JSON 格式草案，尚未 Rec |

---

## C. 法规 / 合规 (Regulation & Compliance)

| 法规 | 生效 | 适用范围 | UX 影响 |
|---|---|---|---|
| **ADA Title III + Section 508** | ADA 1990；508 refresh 2018 | 美国公共部门 + 商业网站事实标准 | 引用 WCAG 2.0 AA（DOJ 2024 Final Rule 对州/地方政府要求 WCAG 2.1 AA） |
| **European Accessibility Act (EAA)** | **2025-06-28 已生效** | 欧盟 27 国，私营部门 B2C 数字产品 | 强制 WCAG 2.1 AA 等价水平；不合规可罚款 |
| **EN 301 549** | **v3.2.1 (2021), v4 草案中** | 欧盟公共采购及 EAA 技术依据 | 引用 WCAG 2.1，逐步过渡到 2.2 |
| **GB/T 37668-2019** | 2019 | 中国国家标准 | 信息技术 互联网内容无障碍可访问性技术要求与测试方法 |
| **GDPR** (欧盟) | 2018 | 欧盟用户数据 | 影响 cookie banner、consent UI、deceptive design 禁令（与 DSA 共同） |
| **DSA (Digital Services Act)** | **2024-02 全面适用** | 欧盟 | 明确禁止 dark patterns / deceptive design |
| **CCPA / CPRA** | 2020 / 2023 | 加州 | 含"对称选择"要求（接受与拒绝同等显眼）影响 consent 设计 |

---

## D. 认证 / 学位

| 项目 | 颁发方 | 含金量备注 |
|---|---|---|
| **NN/g UX Certification** | Nielsen Norman Group | 行业最被认可的非学位认证；需完成 5 门课 + 考试 |
| **HFI CUA (Certified Usability Analyst)** | Human Factors International | 老牌可用性认证 |
| **HFI CXA (Certified User Experience Analyst)** | HFI | CUA 的扩展版 |
| **Google UX Design Certificate** | Google + Coursera | 入门级（约 6 个月），就业市场认可度递减但适合换行 |
| **Interaction Design Foundation (IxDF) Certificates** | IxDF | 模块化课程证书 |
| **IxDA Membership** | Interaction Design Association | 行业协会会员（非考试型认证） |
| **学位** | — | CMU HCII / 华盛顿大学 HCDE / 佐治亚理工 MS-HCI / 同济大学设计创意学院 |

---

## E. 「外行听不懂 / 容易用错」红线词 Top 10

入行者最常被纠正的 10 个混淆：

1. **UI ≠ UX ≠ IxD ≠ Product Design** — UI 是视觉与组件层；UX 是端到端体验（含研究、IA、可用性、内容、视觉）；IxD（Interaction Design）专注交互行为与状态；Product Design 通常包含 UX + 业务/战略责任。简历上随意混用是面试红旗。
2. **Wireframe ≠ Mockup ≠ Prototype** — 线框=结构；mockup=视觉外观；prototype=可点击。新人最常把 Figma 高保真静态稿叫"原型"。
3. **Affordance ≠ Signifier** — Norman 2013 后明确：affordance 是物体的"行动可能性"，signifier 才是"暗示给用户的线索"。学术圈对混用很敏感。
4. **Accessibility (a11y) ≠ Usability ≠ Inclusive Design** — a11y 关注残障可访问；usability 关注所有人能否高效完成任务；inclusive design 是设计过程论（主动覆盖差异）。三者重叠但不相等。
5. **Persona ≠ User Segment ≠ Target Audience** — Persona 是基于研究的具象角色（含行为、动机）；user segment 是按属性聚类；target audience 是营销用语。把市场部 PPT 上的 audience 当 persona 用是常见错误。
6. **Card Sorting ≠ Tree Testing** — 前者让用户**生成**分类；后者**验证**已有 IA。新人在简历"做过 IA 研究"时常混。
7. **Design System ≠ Component Library ≠ Style Guide** — Style guide 是文档；component library 是可复用代码/组件；design system 包含 tokens + 组件 + 文档 + 流程 + 治理。叫法不当会让 design ops 圈子皱眉。
8. **Material Design ≠ Material UI (MUI)** — Material 是 Google 的设计规范；MUI 是一家公司基于 Material 做的 React 库（与 Google 无关）。
9. **Skeuomorphism ≠ Realism ≠ Liquid Glass** — 拟物化是 2010 年代术语；Apple 2025 的 Liquid Glass 是材质层 + 折射光学，不是拟物回归。把 Liquid Glass 称为"拟物 2.0"会被 Apple 设计师纠正。
10. **WCAG AAA 不是"越合规越好"** — W3C 明确说明 AAA 不适合作为整站统一目标（部分准则在某些内容上不可达成）；行业法规与企业 baseline 几乎全部锁 **AA**。新人误把 AAA 当"高级目标"会被无障碍专家指出。

附加易错：

- **"用户体验"≠ "用户界面"**（中文圈也常混）
- **"动效设计 / Motion Design"≠ "Microinteraction"**——前者是宽泛领域，后者是 Saffer 定义的具体单元
- **"Heuristic"** 不读 /hjuːˈrɪstɪk/ 时很容易在评审里破功

---

## 附：信源说明

主要官方与一手来源：

- W3C / WAI: https://www.w3.org/WAI/, https://www.w3.org/TR/WCAG22/
- Nielsen Norman Group: https://www.nngroup.com (Heuristics, Research-based articles)
- ISO: 9241-11:2018, 9241-210:2019
- Apple Human Interface Guidelines: https://developer.apple.com/design/human-interface-guidelines/
- Material Design 3: https://m3.material.io/
- Microsoft Fluent 2: https://fluent2.microsoft.design/
- IBM Carbon: https://carbondesignsystem.com/
- Atomic Design (Brad Frost): https://atomicdesign.bradfrost.com/
- Design Tokens Community Group: https://design-tokens.github.io/community-group/format/
- deceptive.design (Harry Brignull): https://www.deceptive.design/

经典著作（参考非必读全部）：

- Don Norman《The Design of Everyday Things》(Basic Books, 2013 修订版)
- Steve Krug《Don't Make Me Think, Revisited》(New Riders, 2014)
- Jakob Nielsen《Usability Engineering》(Academic Press, 1993)
- Brad Frost《Atomic Design》(2016)
- Jeff Gothelf《Lean UX》(O'Reilly, 2013 / 3rd ed. 2021)
- Jake Knapp《Sprint》(Simon & Schuster, 2016)
- Alan Cooper《About Face》(4th ed., Wiley 2014)
- Peter Morville & Louis Rosenfeld《Information Architecture》(4th ed., O'Reilly 2015)
- Jim Kalbach《Mapping Experiences》(2nd ed., O'Reilly 2020)
- Luke Wroblewski《Mobile First》(A Book Apart, 2011)

明确**不引用**：知乎专栏、微信公众号、百度百科、内容农场聚合站。

---

end of file.
