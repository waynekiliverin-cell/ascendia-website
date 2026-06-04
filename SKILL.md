---
name: ascendia-website-design-system
description: ASCENDIA 高端求职工作室网站设计系统。用于设计 ASCENDIA 官网、Landing Page、服务介绍页、导师介绍页、成功案例页、预约诊断页等任何前端页面。必须遵守 ASCENDIA Brand DNA，体现深蓝金色、高端职业咨询、外企精英感、结构化陪跑和真实 mentor 温度。
---

触发条件：当用户要求制作 ASCENDIA 相关的 HTML 网页、公司官网、Landing Page、品牌介绍页、服务介绍页、导师介绍页、成功案例页、预约诊断页、求职咨询页面、职业规划页面、个人工作室页面、品牌视觉页面、图文卡片、小红书图文、文章转卡片、pitch 页面或任何前端设计相关任务时自动触发。

## 使用方式（7步工作流）

### Step 1: 澄清需求

在开始设计前，先确认以下 5 个问题。如果用户已经提供足够信息，可以根据现有信息直接判断，不要反复追问。

1. **页面类型**  
   是 ASCENDIA 官网首页 / Landing Page / 服务介绍页 / 导师介绍页 / 成功案例页 / 预约诊断页 / 图文卡片 / 其他？

2. **目标受众**  
   是给留学生、家长、求职学员、合作方、导师候选人，还是品牌展示使用？

3. **Section 数量**  
   大概需要几屏内容？例如 5 屏、7 屏、完整官网首页、单页转化页。

4. **素材内容**  
   是否已有 logo、文案、数据、服务体系、导师信息、成功案例、二维码、联系方式？

5. **硬约束**  
   是否必须包含 ASCENDIA logo、slogan、核心数据、2v1 导师矩阵、免费 1v1 诊断 CTA、联系方式、品牌色或特定模块？

---

### Step 2: 读取规范

开始写代码前，必须先读取并遵守以下文件：

1. **必读** `brand-dna.md`  
   确认 ASCENDIA 的品牌底层规范，包括颜色、字体、气质、布局、禁忌、动效和文案语气。

2. 根据页面类型选读对应场景文件：

   - 官网首页 / 公司介绍 / 品牌页 → `references/scene-homepage.md`
   - Landing Page / 转化页 / 预约诊断页 → `references/scene-landing.md`
   - 服务介绍页 → `references/scene-services.md`
   - 导师介绍页 → `references/scene-mentors.md`
   - 成功案例页 → `references/scene-cases.md`
   - 图文卡片 / 小红书图文 / 文章转卡片 → `references/scene-cards.md`
   - App 型 / Dashboard 型 / 内部系统页 → `references/scene-app.md`

如果对应场景文件不存在，则以 `brand-dna.md` 为最高优先级，自行设计符合 ASCENDIA 风格的页面结构。

---

### Step 3: 拷贝模板

必须从 `assets/` 中选择对应模板作为起点，不要从零开始写空白 HTML。

推荐模板：

- 官网首页 → `assets/template-homepage.html`
- Landing Page / 预约诊断页 → `assets/template-landing.html`
- 服务介绍页 → `assets/template-services.html`
- 导师介绍页 → `assets/template-mentors.html`
- 成功案例页 → `assets/template-cases.html`
- 图文卡片 → `assets/template-cards.html`
- App / Dashboard → `assets/template-app.html`

**硬规则：从模板开始改，不从零写。**

如果模板不存在，可以自己创建一个完整 HTML 文件，但必须在文件中内置 ASCENDIA 的品牌变量、基础布局、响应式规则和组件样式。

---

### Step 4: 选择布局组合

从 `references/layouts.md` 中选择 3~5 种布局模式，为每个 section 分配不同布局。

**每个 section 布局必须不同，避免全站像 AI 生成的重复卡片网格。**

推荐 ASCENDIA 布局组合：

1. **Hero 左右分栏**  
   左侧品牌主张、slogan、CTA；右侧 logo、数据卡片或服务矩阵。

2. **大数字信任区**  
   展示 `200+`、`92%`、`180%`、`2v1` 等核心数据。

3. **服务体系阶梯式布局**  
   简历与 LinkedIn、Storybank、Mock Interview、Networking 不要做普通四宫格，要有路径感。

4. **2v1 导师矩阵结构图**  
   展示主导师 + 目标岗位导师 + 学员的陪跑关系。

5. **Timeline / Stepper 求职路径**  
   从定位、简历、Storybank、Mock、Networking 到 offer。

6. **Case Study Card**  
   成功案例要展示背景、问题、策略、结果，不做廉价战报。

7. **深蓝 CTA 区**  
   使用金色按钮，引导免费 1v1 职业诊断。

---

### Step 5: 选择组件填充

从 `references/components.md` 中选取组件填入各 section。

**硬规则：禁止使用任何 HTML 默认样式。**

以下内容必须使用自定义组件，不允许浏览器默认渲染：

- 不允许默认 `<blockquote>`
- 不允许默认 `border-left` 引用块
- 不允许无样式 `<ul>` / `<ol>`
- 不允许默认 `<table>`
- 不允许普通 Bootstrap 风格卡片
- 不允许 cards 嵌套 cards
- 不允许默认按钮样式
- 不允许默认 form 样式

如果 `components.md` 中没有合适组件，必须自行设计一个符合 ASCENDIA Brand DNA 的组件。

推荐 ASCENDIA 组件：

- `BrandHero`
- `StatStrip`
- `ServicePath`
- `MentorMatrix`
- `CaseStudyCard`
- `ProcessTimeline`
- `DiagnosisCTA`
- `PromisePanel`
- `ResumeBeforeAfter`
- `StorybankPreview`
- `NetworkingMessageCard`
- `InterviewMockPanel`
- `ProgressTracker`
- `FAQAccordion`

---

### Step 6: 自检

完成页面后，必须对照 `references/checklist.md` 检查。

如果没有 checklist 文件，则按以下 ASCENDIA 自检标准执行。

## P0 必须全过

任何一条不过，都必须修改。

1. 是否符合 ASCENDIA Brand DNA？
2. 是否使用深蓝、金色、银白作为核心视觉？
3. 是否避免蓝紫渐变、glassmorphism、neon、AI 光效？
4. 是否避免所有 section 居中？
5. 是否每个 section 布局有变化？
6. 是否没有使用浏览器默认 blockquote、ul、ol、table 样式？
7. 是否没有 Inter / Roboto / Arial 作为主字体？
8. 是否没有 AI 生成的通用 SaaS Landing Page 感？
9. 是否没有“保 offer”“逆天改命”“全网最强”等焦虑营销文案？
10. 是否移动端可读、可点、不卡、不隐藏核心内容？

## P1 应该满足

1. Hero 是否 10 秒内讲清楚 ASCENDIA 是谁、做什么、为什么可信？
2. 是否突出 `Redefine Your Limits` / 打破职场天花板？
3. 是否展示 2v1 导师矩阵？
4. 是否展示核心服务体系？
5. 是否展示关键数据和信任背书？
6. 是否有明确 CTA？
7. 是否有 mentor 陪伴感，而不是纯销售感？
8. 是否有真实工作流元素，例如简历修改、Storybank、Mock、Networking、Next Step？

## P2 加分项

1. 有轻微 consulting deck 质感。
2. 有金色细线、数据标签、进度结构等高级细节。
3. 有克制动效，如 fade in、slow reveal、number count-up。
4. 有清晰的视觉节奏和留白。
5. 页面截图不会被评价“又是 AI 做的”。
6. 用户能感受到高端、可信、专业、有人味。

---

### Step 7: 交付

最终输出必须是可直接在浏览器打开的 HTML 文件。

交付要求：

1. 输出完整 HTML。
2. CSS 可以写在 `<style>` 中，确保单文件可运行。
3. 如果有 JS，写在 `<script>` 中，避免外部依赖过多。
4. 如果使用 logo，优先使用：
   - `assets/ascendia-logo-mark-transparent.png`
   - `assets/ascendia-logo-card-hd.png`
   - `assets/ascendia-logo-mark.svg`
   - `assets/ascendia-logo-card.svg`
5. 页面必须响应式。
6. 页面必须尊重 `prefers-reduced-motion`。
7. 所有链接、按钮、表单、卡片必须有 hover / focus 状态。
8. 不允许交付半成品结构或伪代码。
9. 不允许只给设计建议，必须给最终可运行 HTML。

---

## 场景类型速查

| 类型 | 场景文件 | 模板 |
|------|----------|------|
| 官网首页 | `references/scene-homepage.md` | `assets/template-homepage.html` |
| Landing Page / 预约诊断页 | `references/scene-landing.md` | `assets/template-landing.html` |
| 服务介绍页 | `references/scene-services.md` | `assets/template-services.html` |
| 导师介绍页 | `references/scene-mentors.md` | `assets/template-mentors.html` |
| 成功案例页 | `references/scene-cases.md` | `assets/template-cases.html` |
| 图文卡片 / 小红书图文 | `references/scene-cards.md` | `assets/template-cards.html` |
| App / Dashboard | `references/scene-app.md` | `assets/template-app.html` |

---

## ASCENDIA 核心品牌原则

### 1. 深蓝金色是品牌识别核心

页面必须围绕：

- 深海军蓝 `#0B1324`
- 品牌金 `#D6B85F`
- 银白灰 `#E3E7EA`

展开设计。金色只做强调，不做大面积铺底。

---

### 2. 设计要像高端 career studio

ASCENDIA 不是普通留学中介，也不是低价简历修改工作室。页面应该体现：

- 高端
- 专业
- 可信
- 外企感
- 金融 / 咨询感
- 结构化
- 有陪伴感

---

### 3. 文案要像 mentor，不像销售

文案需要克制、真实、有判断力。

推荐表达：

- “把模糊的职业焦虑，变成可执行的求职路径。”
- “让每一段经历，都能被目标岗位看懂。”
- “不是制造焦虑，而是陪你看清方向、补齐能力、提高命中率。”
- “Redefine Your Limits，不是喊口号，而是通过结构化陪跑，让你的经历被更准确地看见。”

禁止表达：

- “保 offer”
- “逆天改命”
- “全网最强”
- “独家内幕”
- “不报就晚了”
- “100% 拿 offer”
- “碾压同龄人”

---

### 4. 页面必须体现方法论

ASCENDIA 的差异化不是“服务很多”，而是“路径清楚”。

页面中应优先展示：

- 2v1 导师矩阵
- 简历与 LinkedIn 重塑
- Storybank 搭建
- Mock Interview
- Networking 实战
- Next Step 追踪
- 进度预警
- Offer-oriented path

---

### 5. 设计不能像 AI 模板

避免以下 AI 模板特征：

- 蓝紫渐变
- 玻璃拟态
- 霓虹光效
- 大量圆角矩形卡片
- 每个 section 都居中
- 无意义 3D 图形
- stock photo 商务人物
- 渐变大标题
- 过度均匀的卡片网格
- 过度使用 emoji
- 模板化 “Trusted by thousands” 风格

---

## 推荐页面结构：ASCENDIA 首页

如果用户没有提供具体页面结构，默认使用以下官网首页结构：

1. **Navigation**
   - Logo
   - Services
   - Method
   - Cases
   - Mentors
   - Free Diagnosis CTA

2. **Hero**
   - Redefine Your Limits
   - 打破职场天花板
   - 留学生专属高端求职陪跑工作室
   - CTA：预约 1v1 职业诊断
   - 右侧：logo / 数据卡片 / 2v1 mentor visual

3. **Trust Numbers**
   - `200+` 成功辅导案例
   - `92%` 上岸率
   - `180%` 人均 offer 率
   - `2v1` 导师矩阵

4. **Problem Section**
   - 留学生求职常见痛点
   - 方向模糊
   - 简历表达弱
   - 面试故事散
   - Networking 不会推进

5. **Service System**
   - 简历与 LinkedIn 重塑
   - Storybank 搭建
   - Mock Interview
   - Networking 实战

6. **2v1 Mentor Matrix**
   - 主导师：长期规划与推进
   - 目标岗位导师：行业深度与面试实战
   - 学员：执行、反馈、迭代

7. **Process Timeline**
   - Diagnose
   - Position
   - Rebuild
   - Practice
   - Connect
   - Convert

8. **Case Studies**
   - 背景
   - 问题
   - 策略
   - 结果

9. **Promise**
   - 首次 call 后 3 天内交付
   - 工作时间 3 小时内响应
   - 每次会议确认 next step
   - 进度预警表追踪

10. **Final CTA**
   - 免费 1v1 顶层设计诊断
   - 输入：学校 + 年级 + 目标方向
   - CTA：获取定制化破局方案

11. **Footer**
   - Logo
   - Slogan
   - 联系方式
   - 免责声明

---

## 推荐 CSS 变量

每个 HTML 文件都应该内置以下变量：

```css
:root {
  --color-navy: #0B1324;
  --color-navy-soft: #111B2E;
  --color-navy-light: #1B2740;
  --color-gold: #D6B85F;
  --color-gold-soft: #F1D884;
  --color-silver: #E3E7EA;
  --color-white: #F8FAFC;
  --color-muted: #AAB3C2;
  --color-border: #263247;
  --color-success: #2FAE7B;
  --color-danger: #D94C4C;

  --gradient-hero: linear-gradient(135deg, #0B1324 0%, #111B2E 55%, #1B2740 100%);
  --gradient-gold: linear-gradient(135deg, #D6B85F 0%, #F1D884 100%);

  --font-serif-en: "Fraunces", "Playfair Display", "Cormorant Garamond", Georgia, serif;
  --font-serif-cn: "Noto Serif SC", "Source Han Serif SC", "Songti SC", serif;
  --font-sans-cn: "Noto Sans SC", "Source Han Sans SC", -apple-system, BlinkMacSystemFont, "PingFang SC", "Helvetica Neue", sans-serif;
  --font-data: "IBM Plex Sans", "Fira Code", monospace;

  --section-space: clamp(88px, 12vh, 160px);
  --block-space: clamp(40px, 6vw, 96px);
  --card-padding: clamp(28px, 3vw, 44px);
  --gap: clamp(24px, 3vw, 48px);
  --max-width: 1280px;
}
```

---

## 响应式规则

必须满足：

- `1024px`：三栏变两栏
- `900px`：两栏变单栏
- `600px`：字号和按钮微缩
- 移动端重新排列，不是简单缩小
- 移动端不隐藏核心内容
- CTA 在移动端必须靠前
- 导航移动端简洁，不做复杂动画菜单

---

## 动效规则

推荐：

- fade in
- slow reveal
- card hover lift
- underline slide
- number count-up
- progress bar fill
- timeline step reveal

禁止：

- bounce
- elastic
- neon glow
- 无限漂浮动画
- 快速闪烁
- 大面积 parallax
- animate width / height 导致 layout shift

必须包含：

```css
@media (prefers-reduced-motion: reduce) {
  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    scroll-behavior: auto !important;
    transition-duration: 0.01ms !important;
  }
}
```

---

## 最终交付底线

每次生成 ASCENDIA 页面前，必须问自己：

1. 这个页面像不像高端 career studio？
2. 这个页面有没有 ASCENDIA 的深蓝金色识别感？
3. 这个页面有没有外企 / 金融 / 咨询感？
4. 这个页面有没有真实 mentor 陪跑的温度？
5. 这个页面有没有清楚表达服务方法论？
6. 这个页面有没有避免 AI 模板感？
7. 用户打开后，能不能马上知道 ASCENDIA 能帮他做什么？

只有全部通过，才能交付。

---

## 重要禁忌

严格遵守 `brand-dna.md` 的禁忌清单，不在此重复。核心底线：

**页面截图发出去，不能被评论“又是 AI 做的”。**

ASCENDIA 的视觉必须是：

**专业可信 · 高端但不装 · 外企精英感 · 结构化陪跑 · 结果导向 · 有 mentor 温度**
