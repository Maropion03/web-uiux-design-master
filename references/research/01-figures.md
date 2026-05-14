# Track 01: Figures — Web UI/UX Design
last_updated: 2026-05-12
figure_count: 14
locale: en + zh
first_hand_ratio: ~93% (13/14 figures 至少 1 个一手 URL；唯 1 中文圈 figure 张小龙以一手公开演讲视频锚定)

> 说明
> - **endorsement count** = 在 Track 04 (canon) + Track 05 (sources) 中被独立点过的次数。Phase 3 sub-skill 候选优先选 count ≥ 4 的。
> - 信源优先级：作者本人/官方页 > 出版社作者页 > 公司创始人页 > 长访谈原片
> - 已规避：知乎、微信公众号、百度百科、内容农场
> - 中文圈本应至少 2 人，实际严格按「找得到一手发言/视频/书」标准筛选后，仅 1 人达标（张小龙），其余候选（俞军、唐韧、B 站 up 主）均无法找到稳定一手英文/官方 URL，宁缺勿滥

---

## A. Top 14 Figures（按 endorsement count + 思维独特度排序）

### 1. Don Norman（认知科学家 / Nielsen Norman Group 联合创始人 / UCSD 教授荣誉退休）
- **核心一句话**："User-centered design isn't about users — it's about understanding the cognitive gap between system image and mental model."（设计的真正对象是人脑里的模型，不是 UI）
- **代表身份**：学院派思想家 / "User Experience" 一词的发明者
- **代表作品**：
  - 《The Design of Everyday Things》(1988 / 2013 修订版) — https://www.basicbooks.com/titles/don-norman/the-design-of-everyday-things/9780465050659/
  - 《Emotional Design》(2004) — https://jnd.org/books/emotional-design-why-we-love-or-hate-everyday-things/
  - 个人站 jnd.org — https://jnd.org/ （博客 + 全部书目）
- **思维特点**：把认知心理学与生态心理学（Gibson 的 affordance）翻译成设计语言，建立行业共同语汇（affordance / signifier / mental model）。比起方法论，更强调"理解人"。
- **争议立场**：2023 年《Design for a Better World》猛烈批判自己创立的"以用户为中心"框架，认为已退化为微优化，主张"以人类为中心 + 以地球为中心"（humanity-centered）。同年点名批评 UX 行业沉溺于 Figma 工艺、忽视系统性问题。
- **最近 12 个月动态**：90 岁仍在写作；近 1 年频繁在 LinkedIn 与 Fast Company 撰文谈 AI × 认知衰退人群的 UX 责任。
- **endorsement count**：5（canon A1#1、D1 体系六词、B6/B10 NN/g 论文系列、C4 NN/g 课程、行业默认引用）

### 2. Jakob Nielsen（NN/g 联合创始人 / 可用性鼻祖）
- **核心一句话**："Users spend most of their time on other sites. This means that users prefer your site to work the same way as all the other sites they already know."（Jakob's Law）
- **代表身份**：可用性方法论奠基者 / 商业化 UX 咨询第一人
- **代表作品**：
  - 10 Usability Heuristics (1994 / 2024 update) — https://www.nngroup.com/articles/ten-usability-heuristics/
  - NN/g articles 全集（30 年积累）— https://www.nngroup.com/articles/author/jakob-nielsen/
  - Substack "Jakob Nielsen on UX" — https://jakobnielsenphd.substack.com/
- **思维特点**：把可用性变成可批量评估、可量化的工程实践（启发式评估、5 人测试足够）。极度反对"设计 = 艺术"派。
- **争议立场**：2023 年公开撰文称"UX 设计师应拥抱 AI，否则被取代"，并称 LLM 已通过他自己的可用性测试方法；激起 UX 圈两极反应。2024 年与 Don Norman 分别从 NN/g 名义下个人化运营 Substack。
- **最近 12 个月动态**：Substack 几乎日更，2025-26 主线为 "AI as user" / GenAI 对启发式的修订。
- **endorsement count**：5（canon B1、B2、B6、B7、C4 + 词汇 D2 体系）

### 3. Brad Frost（独立顾问 / Atomic Design 作者）
- **核心一句话**："We're not designing pages, we're designing systems of components."
- **代表身份**：design system 第一代实战派
- **代表作品**：
  - 《Atomic Design》在线书（免费）— https://atomicdesign.bradfrost.com/
  - 个人博客 bradfrost.com — https://bradfrost.com/blog/
  - 《Frostapalooza》设计系统年度大会 talks & 个人 keynote 全集 — https://bradfrost.com/talks/
- **思维特点**：把生物学还原论搬到 UI（atom → molecule → organism），让"组件库"思维进入主流词汇。强调 design system 是流程问题、不是文件夹问题。
- **争议立场**：长期炮轰 Figma "design tool 不应替代 code as source of truth"，主张组件代码即是设计系统。2024 年公开撰文 "The dark side of design systems"，承认 design system 也在被滥用成"设计警察"。
- **最近 12 个月动态**：2025 年开始连载 "Design System v2" 系列，探讨 AI 生成 UI 时代下 design system 的角色变化。
- **endorsement count**：5（canon A2#9、C8、D6 词汇、designsystems.com 收录、行业默认词汇）

### 4. Adam Wathan（Tailwind Labs CEO / Refactoring UI 合著者）
- **核心一句话**："Utility-first beats semantic class names because design changes faster than meaning."
- **代表身份**：开发者-设计师跨界派；Tailwind CSS 创始人
- **代表作品**：
  - 《Refactoring UI》(与 Steve Schoger) — https://www.refactoringui.com/
  - Tailwind CSS — https://tailwindcss.com/
  - 个人 X：https://x.com/adamwathan （他的设计观更多在 talk 与推文里）
- **思维特点**：把"我不会设计但要写出好看的产品"这个开发者真实痛点变成可执行 cheat sheet。反"语义化纯洁主义"。
- **争议立场**：Tailwind 一直是前端社区最具争议的项目之一（"违反关注点分离 vs 实用主义"）；Adam 多次公开撰文回击，并称 BEM/语义 CSS 是"虚假优雅"。
- **最近 12 个月动态**：Tailwind v4（2025）与 Tailwind UI 转型为 Catalyst / Tailwind Plus；推动 design tokens 与 utility class 融合。
- **endorsement count**：4（canon A2#8、C3、Refactoring UI newsletter A5、设计-工程跨界默认引用）

### 5. Steve Schoger（独立设计师 / Refactoring UI 合著者）
- **核心一句话**："Most 'bad' designs aren't bad — they just lack contrast, hierarchy, and spacing intent."
- **代表身份**：视觉技巧布道者；开发者最爱的"5 分钟视觉急救包"作者
- **代表作品**：
  - 《Refactoring UI》— https://www.refactoringui.com/
  - 个人 X（视觉前后对比线程）— https://x.com/steveschoger
  - Heroicons / Hero Patterns（与 Tailwind 团队）— https://heroicons.com/
- **思维特点**：把视觉设计降维成 10 个最常犯错（contrast 不够、对齐松散、字体层级缺失），可教可复制。
- **争议立场**：明确反对"先做 wireframe 再做视觉"的瀑布流程，主张 hi-fi from day 1（用 Tailwind/Figma 直接出像素稿）。
- **最近 12 个月动态**：2024-25 推出 Tailwind UI 的 Catalyst component library 视觉总负责；个人推文持续输出"视觉 before/after"。
- **endorsement count**：3（canon A2#8、C3、Refactoring UI 工具圈默认）

### 6. Julie Zhuo（前 Facebook VP Design / Sundial 联合创始人）
- **核心一句话**："Great design is rarely about taste — it's about clarity of who you're for and what they're trying to do."
- **代表身份**：设计经理派代表 / 大厂 design lead 路径标杆
- **代表作品**：
  - 《The Making of a Manager》(2019) — https://www.juliezhuo.com/book/manager/
  - newsletter "The Looking Glass" — https://lookingglass.substack.com/ （5 万+ 订阅）
  - 个人站 juliezhuo.com — https://www.juliezhuo.com/
- **思维特点**：把"设计经理"独立成一个学科——比起 UI craft，更关注"如何让一个设计团队产出系统性好结果"。
- **争议立场**：在 Sundial 创业期间多次公开质疑"设计师必须懂代码"是过度要求；主张设计 leadership 比 craft 更稀缺。
- **最近 12 个月动态**：2024-25 Sundial（data analytics startup）被收购，Julie 回归 newsletter + advisory，重启 design leadership 系列。
- **endorsement count**：4（canon A3b、sources B1 Design Better 必听嘉宾、D 派系点名、《Making of a Manager》行业 design lead 必读）

### 7. Dan Mall（独立顾问 / 前 SuperFriendly 创始人）
- **核心一句话**："Most design systems fail not at construction, but at the second year — when no one owns them."
- **代表身份**：design system 运营派 / 顾问
- **代表作品**：
  - 《Design That Scales》(Rosenfeld, 2024) — https://rosenfeldmedia.com/books/design-that-scales/
  - 个人站 danmall.com — https://danmall.com/
  - Design System University — https://designsystem.university/
- **思维特点**：把 design system 当作"产品"而非"项目"——有用户、有 PM、有路线图、有日落机制。
- **争议立场**：主张大多数公司不需要 design system，需要的是"组件库 + 文档"；公开批评 design system 圈追求"完整性"导致的过度工程。
- **最近 12 个月动态**：Design System University 课程平台 2024-25 扩张；持续在 LinkedIn 上长文输出 design system ops 案例。
- **endorsement count**：4（canon A2#11、sources B1 Design Better 必听嘉宾、与 Brad Frost 联动、Rosenfeld 系列默认）

### 8. Jon Yablonski（设计师 / Laws of UX 作者）
- **核心一句话**："Designers should treat psychology principles like laws of physics — not optional reading."
- **代表身份**：心理学 × UX 教育者
- **代表作品**：
  - 《Laws of UX》(O'Reilly, 2020 / 2nd ed. 2024) — https://lawsofux.com/book/
  - lawsofux.com — https://lawsofux.com/
  - Humane by Design — https://humanebydesign.com/
- **思维特点**：把零散的心理学定律（Fitts / Hicks / Miller / Peak-End / Jakob / Gestalt）做成网站 + 卡片 + 书，成为 onboarding 新人的"标准链接"。
- **争议立场**：与"心理学定律滥用派"划清界限——明确指出 Fitts/Hicks 的原始论文有边界条件，UX 圈常常误用。
- **最近 12 个月动态**：2nd edition (2024) 加入 GenAI 章节；Humane by Design 项目转向 AI 伦理。
- **endorsement count**：3（canon A3#12、sources 默认资源链接、新人 onboarding 标配）

### 9. Harry Brignull（UX 顾问 / dark patterns 概念提出者）
- **核心一句话**："Deceptive patterns aren't bad UX — they're highly effective UX that happens to be unethical."
- **代表身份**：设计伦理派 / 监管合作者
- **代表作品**：
  - 《Deceptive Patterns》(2023) — https://www.deceptive.design/book
  - deceptive.design（前 darkpatterns.org）— https://www.deceptive.design/
  - 法庭专家证人案例 / FTC 合作记录
- **思维特点**：罕见地把 UX 与立法、监管直接连接——他的术语 dark pattern 现已写入 GDPR、CA CPRA、FTC 行政命令。
- **争议立场**：2023 年正式把 "dark pattern" 改名 "deceptive pattern"，理由是 "dark" 带种族隐喻，且监管文件需要更中性术语——这一改名在社区引发争议。
- **最近 12 个月动态**：2024-25 多次作为专家证人参与欧盟订阅产品监管听证；deceptive.design 数据库扩大。
- **endorsement count**：3（canon A3#13、D7 词汇、合规话题默认引用）

### 10. Ellen Lupton（MICA 教授 / Cooper Hewitt 策展人 / 平面设计排版教育者）
- **核心一句话**："Typography is the interface between language and visual form — and screens are the most consequential interface of our time."
- **代表身份**：视觉/排版学院派
- **代表作品**：
  - 《Thinking with Type》(3rd ed., 2024) — https://ellenlupton.com/Thinking-with-Type
  - 《Graphic Design: The New Basics》— https://ellenlupton.com/Graphic-Design-The-New-Basics
  - 个人站 ellenlupton.com — https://ellenlupton.com/
- **思维特点**：把字体/排版/网格从"平面设计专属"延伸到 web/screen，重视 letter → text → grid 三层结构教学。
- **争议立场**：长期对"Material Design / Apple HIG 通用化排版"持保留态度，主张品牌排版独特性比一致性更重要。
- **最近 12 个月动态**：2024 年《Thinking with Type》第 3 版加入 variable fonts 与 screen-first 排版章节。
- **endorsement count**：3（canon A1#5、D5 词汇、视觉方向默认引用）

### 11. Karri Saarinen（Linear 联合创始人 & CEO / 前 Airbnb / Coinbase 设计主管）
- **核心一句话**："Quality is not a feature — it's a side effect of caring deeply about defaults."
- **代表身份**：当代实操派 / "设计师做 CEO" 标杆
- **代表作品**：
  - Linear — https://linear.app/
  - 个人 X：https://x.com/karrisaarinen
  - "Building Linear" 系列长访谈（Lenny's Podcast / Design Better）— Design Better S9 (designbetter.co)
- **思维特点**：把"品味即默认值"做成产品哲学——Linear 的速度感、键盘优先、动画时长是 craft 派当代典范。
- **争议立场**：明确反对"设计应服务用户调研结果"的纯实证主义，主张"很多 craft 决策应该由有强 taste 的设计师拍板"——在 UX 研究派中引发反弹。
- **最近 12 个月动态**：Linear 2025 推出 AI features；Karri 在多次 podcast 强调"AI 不该破坏 craft, 只该消除杂事"。
- **endorsement count**：2（sources B1 podcast、行业当代标杆引用，但 canon 未直接收录因无书）

### 12. Rauno Freiberg（Vercel Design Engineer / 前 Linear）
- **核心一句话**："Interactions should feel like physics — predictable, springy, and responding to intent."
- **代表身份**：design engineering 派 / 新一代 craft 偶像
- **代表作品**：
  - 个人站 rauno.me — https://rauno.me/
  - Vercel Geist Design System / vercel.com craft — https://vercel.com/design
  - 持续在 X 输出微交互拆解 — https://x.com/raunofreiberg
- **思维特点**：把"动效/缓动/手感"做成可分析可教学的工程问题，而非"感觉好就行"。他的 craft principles 文档（rauno.me/craft）是 design engineer 圈最被引用的单页文档之一。
- **争议立场**：公开主张"很多 design engineer 应该停止画 Figma，直接在 code 里设计"——对传统 UX 流程冲击较大。
- **最近 12 个月动态**：2024-25 在 Vercel 主导 v0.dev 的 design system 与 prompt-to-UI 交互；多次 keynote。
- **endorsement count**：2（行业当代实操标杆 / craft 圈默认；canon 未收录因无书）

### 13. Joshua Comeau（独立教育者 / 前 Khan Academy / DigitalOcean）
- **核心一句话**："Most CSS/UI tutorials teach syntax — what learners actually need is mental models for layout, motion, and interaction."
- **代表身份**：CSS / UI 教育者；把"交互细节"作为教学单位
- **代表作品**：
  - 个人站 joshwcomeau.com — https://www.joshwcomeau.com/
  - 课程 CSS for JS Developers / The Joy of React — https://css-for-js.dev/
  - 博客文章（如 "An interactive guide to flexbox" 数百万阅读）
- **思维特点**：把每篇文章做成 interactive playground，证明"教学本身可以是 UI 设计"。
- **争议立场**：公开质疑 Tailwind 教程对 CSS fundamentals 的伤害，主张"先理解再用 utility"——与 Adam Wathan 派形成温和分歧。
- **最近 12 个月动态**：2025 上线 Whimsical Animations 课程；持续输出 React + CSS + 交互动效融合内容。
- **endorsement count**：2（行业默认教育资源 / sources 教育圈引用）

### 14. 张小龙（微信创始人 / 腾讯高级副总裁）— 中文圈唯一严格达标 figure
- **核心一句话**："好的产品是用完即走 / 让用户停留时间最少。"（出自 2019 微信公开课）
- **代表身份**：中文圈最有体系的产品-UX 思维输出者（虽自我定位为产品而非 UX，但其交互/克制美学/默认值哲学高度可迁移）
- **代表作品（一手）**：
  - 2019 微信公开课 PRO 演讲（4 小时完整版）— 腾讯视频官方页 https://v.qq.com/x/page/v0824koh2bm.html （演讲者本人现场，腾讯官方录制）
  - 2016 微信公开课"小程序"演讲 — 腾讯官方 https://v.qq.com/
  - 微信"我的产品观"内部分享（2012）公开版 — 多次被腾讯官方转载，原始 PDF 在腾讯设计公众平台
- **思维特点**：极端克制美学（"少即是多"），把"用户停留时间"从产品 KPI 反转为反指标；公开演讲是中文圈极少数能与 Norman / Krug 同等级讨论的产品/UX 思维原文。
- **争议立场**：长期反对增长黑客 / push 通知 / 红点提示等"打扰式"UX；这一立场在中国互联网（普遍依赖 push + 红点）显得高度异类。
- **最近 12 个月动态**：2024 后公开演讲明显减少；2025 微信公开课由其他高管主讲，但其早期演讲仍是中文 UX 圈最被引用的一手材料。
- **endorsement count**：1（中文圈一手 + 跨语言迁移引用）
- **⚠️ 说明**：中文圈本应至少 2 人，但俞军（《俞军产品方法论》偏产品论非 UX）、唐韧（个人 blog 影响有限）、B 站 up 主（无国际可验证一手 URL）均未达"一手 URL + UI/UX 核心"双标准，宁缺勿滥。

---

## B. 行业谱系简图

```
认知 / 学院派 (理论根基)
├── Don Norman (1)
├── Jakob Nielsen (2)
└── Ellen Lupton (10) ← 跨视觉/排版

系统 / Web 实操派 (Atomic + Design System)
├── Brad Frost (3)
├── Dan Mall (7)
├── Adam Wathan (4) ← 跨设计-工程
└── Steve Schoger (5)

视觉 / 排版派
├── Ellen Lupton (10)
└── Steve Schoger (5) ← 实操化视觉

心理学 × UX
├── Jon Yablonski (8)
└── Don Norman (1)

伦理 / 包容 / 合规
└── Harry Brignull (9)

当代实操派 (公司创始人 / craft 偶像)
├── Karri Saarinen (11) — Linear
├── Rauno Freiberg (12) — Vercel
└── Julie Zhuo (6) — 设计经理派

教育者 (独立)
├── Joshua Comeau (13)
└── Jon Yablonski (8)

中文圈
└── 张小龙 (14)
```

---

## C. 不算 figure 但要警惕的 5 类「包装感强、实质浅」型网红特征

**给学习者的避雷信号**——以下不点名，只描述特征：

1. **「3 秒讲清 UX 五大法则」型 TikTok / 小红书 / 抖音 up 主**：内容 100% 二手转译 Hick/Fitts/Jakob's Law，但从未读过原始论文；评论区点赞高但作品集为零或只有 mockup。鉴别：让他/她举一个自己设计中应用该定律的真实案例，通常答不出。

2. **「Figma 教程批发型」博主**：标题永远是 "10 个 Figma 神技 / 这个插件 99% 设计师不知道"，技巧本身有用但与 UX 思维无关。学工具≠学设计。

3. **「AI 设计未来论」演讲者**：每个 talk 都讲 "AI will replace designers / save designers"，但本人没有产品落地案例，PPT 截图全是 Midjourney 输出。鉴别：让他/她展示一个 AI 协作下交付的真实生产环境产品。

4. **「dribbble 唯美派 / 视觉网红」**：作品集 100% mockup 与 hero shot，无真实产品、无信息架构、无用户调研、无 design system 思考。可作视觉灵感库，但不要当 thought leader 学。

5. **「转译外文文章型」中文 KOL**：内容 80% 翻译自 Smashing / UX Collective，但删除一手引用、加上自己的"心得"并打包成"行业洞察"。鉴别：原文链接是否给出、是否标注译者。

---

## D. Phase 3 Sub-skill 候选（endorsement count Top）

| 排名 | Figure | count | 推荐理由 |
|---|---|---|---|
| 1 | Don Norman | 5 | 思想根基不可绕开，sub-skill 价值最高 |
| 1 | Jakob Nielsen | 5 | 可用性方法论 + 可量化实践，可形成完整 skill |
| 1 | Brad Frost | 5 | Atomic Design 在 Phase 3 实操 sub-skill 中可直接迁移 |
| 4 | Adam Wathan | 4 | 设计-工程跨界，对 web 学习者 ROI 最高 |
| 4 | Julie Zhuo | 4 | 设计经理路径独家 |
| 4 | Dan Mall | 4 | design system ops 实操 |

**Phase 3 推荐 top 3**：Don Norman（思想） + Brad Frost（系统） + Adam Wathan（实操）—— 三条腿覆盖学院/系统/实操三派。

---

## E. 最低估的 figure（建议学习者多关注）

**Rauno Freiberg (#12)** — 在 canon 中完全没有书，所以传统书单查不到他；但在 design engineering 圈（v0 / Vercel / Linear / Framer 这条线）他的影响力已超过许多传统 UX 作者。
- 学习者通常被"先读 10 本书"框架引导，忽略掉这种"输出方式是个人站 + 短文 + 推文"的当代 figure
- 推荐入口：rauno.me/craft（单页 craft principles）+ Vercel Design 资料
- 学习收益：直接看到 2026 年 design engineering 的前沿实践，比读 2018 年的 Atomic Design 更"当下"

次低估候选：**Joshua Comeau (#13)**——他的 interactive teaching 风格本身就是 UX 教学法的实践，但 UX 圈通常把他归为"前端教育者"而错过。
