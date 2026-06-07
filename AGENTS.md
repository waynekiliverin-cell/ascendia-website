# AGENTS.md — ASCENDIA Website Project Instructions

This repository is for designing and building the ASCENDIA website and related brand pages.

Before creating or editing any ASCENDIA webpage, always read and follow:

1. `SKILL.md`
2. `brand-dna.md`

If available, also read:

3. `references/components.md`
4. `references/layouts.md`
5. `references/checklist.md`

If any referenced file does not exist, do not fail. Instead, create a simple compliant version based on `SKILL.md` and `brand-dna.md`.

---

## Project Goal

ASCENDIA is a premium career studio for international students.

The website should communicate:

- high-end career consulting
- international student career planning
- structured job-search support
- finance / consulting / tech / business professionalism
- mentor-like guidance
- human warmth without sales pressure

ASCENDIA is not a traditional study-abroad agency, not a low-cost resume editing service, and not a generic AI-generated landing page.

---

## Core Visual Identity

Use ASCENDIA's core colors:

| Color | Hex | Usage |
|---|---|---|
| Deep Navy | `#0B1324` | Main background, navigation, hero, premium sections |
| Brand Gold | `#D6B85F` | CTA buttons, key numbers, icons, highlights, dividers |
| Silver Gray | `#E3E7EA` | Main text on dark background, lines, supporting content |
| Soft Navy | `#111B2E` | Cards, secondary sections |
| Muted Gray Blue | `#AAB3C2` | Subtitles and secondary text |
| Border Blue Gray | `#263247` | Card borders and dividers |

Gold must be used as an accent, not as a large background color.

The overall visual direction should be:

**premium navy + restrained gold + clear silver typography.**

---

## Brand Personality

The website must feel:

- professional
- premium but not cold
- structured and method-driven
- mentor-like and human
- international and career-focused
- suitable for students targeting finance, consulting, tech, data, business, marketing, and corporate roles

The design should look like a boutique career studio, not a generic SaaS landing page.

---

## Copywriting Voice

Write like an experienced mentor, not a salesperson.

The tone should be:

- clear
- calm
- credible
- structured
- supportive
- result-oriented
- never anxiety-driven

Recommended expressions:

- “把模糊的职业焦虑，变成可执行的求职路径。”
- “让每一段经历，都能被目标岗位看懂。”
- “不是制造焦虑，而是陪你看清方向、补齐能力、提高命中率。”
- “Redefine Your Limits，不是喊口号，而是通过结构化陪跑，让你的经历被更准确地看见。”

Avoid exaggerated sales copy such as:

- “保 offer”
- “100% 拿 offer”
- “逆天改命”
- “全网最强”
- “独家内幕”
- “不报就晚了”
- “碾压同龄人”

---

## Required Design Style

Prioritize:

- left-aligned layouts
- clear hierarchy
- strong editorial rhythm
- premium navy-and-gold visual system
- large trust numbers
- structured service flows
- 2v1 mentor matrix visuals
- timeline or stepper process sections
- case study cards with real context
- clear CTA sections
- subtle, restrained motion

Do not make every section centered.

Each section should use a different layout pattern when possible.

---

## Avoid

Do not use:

- blue-purple gradients
- glassmorphism
- neon effects
- generic AI-generated SaaS design
- all-centered sections
- default HTML tables, lists, or blockquotes
- random stock business photos
- overused Inter / Roboto / Arial as the main visual font
- exaggerated sales copy
- generic “Trusted by thousands” template language
- meaningless 3D illustrations
- excessive rounded cards
- cards nested inside cards
- gradient text as a main visual feature

The final page should not look like an AI-generated template.

---

## Logo Assets

Prefer these logo files when available:

- `assets/ascendia-logo-mark-transparent.png`
- `assets/ascendia-logo-card-hd.png`
- `assets/ascendia-logo-mark.svg`
- `assets/ascendia-logo-card.svg`

Logo usage rules:

- Keep enough whitespace around the logo.
- Do not stretch, distort, rotate, recolor, or add neon effects.
- Prefer placing the logo on deep navy or clean light backgrounds.
- Use transparent logo mark for navigation and hero sections.
- Use logo card for large cover or hero visuals.

---

## Default Homepage Structure

If the user does not specify a structure, use this default ASCENDIA homepage structure:

1. Navigation
   - Logo
   - Services
   - Method
   - Cases
   - Mentors
   - Free Diagnosis CTA

2. Hero
   - `Redefine Your Limits`
   - `打破职场天花板`
   - 留学生专属高端求职陪跑工作室
   - CTA: 预约 1v1 职业诊断
   - Right side: logo, trust numbers, or mentor matrix preview

3. Trust Numbers
   - `200+` successful cases
   - `92%` success rate
   - `180%` average offer rate
   - `2v1` mentor matrix

4. Student Pain Points
   - unclear direction
   - weak resume positioning
   - scattered interview stories
   - difficulty with networking
   - lack of execution structure

5. Service System
   - Resume & LinkedIn rebuild
   - Storybank development
   - Mock Interview
   - Networking strategy and execution

6. 2v1 Mentor Matrix
   - Main mentor: long-term planning and execution
   - Target-role mentor: industry depth and interview practice
   - Student: execution, feedback, iteration

7. Process Timeline
   - Diagnose
   - Position
   - Rebuild
   - Practice
   - Connect
   - Convert

8. Case Studies
   - Background
   - Problem
   - Strategy
   - Result

9. Promise / Service Guarantee
   - First-call deliverables within 3 days
   - Response within 3 working hours
   - Next Step confirmed after every meeting
   - Progress warning and tracking system

10. Final CTA
   - Free 1v1 career diagnosis
   - Ask user for school, year, and target direction
   - CTA: 获取定制化破局方案

11. Footer
   - Logo
   - Slogan
   - Contact information
   - Disclaimer

---

## Component Rules

Do not use browser default styles for important content.

Custom style or build components for:

- buttons
- cards
- lists
- tables
- blockquotes
- forms
- accordions
- timelines
- statistics
- CTA sections

Recommended component types:

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

If `references/components.md` exists, use it as a starting point. If not, create compliant components from scratch.

---

## CSS Variables

Every standalone HTML page should include ASCENDIA brand variables similar to the following:

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

## Responsive Rules

The website must be responsive.

Use these breakpoints when appropriate:

- `1024px`: three-column layouts become two-column layouts
- `900px`: two-column layouts become single-column layouts
- `600px`: reduce font sizes, spacing, and button sizes carefully

Mobile behavior:

- Rearrange content instead of simply shrinking it.
- Do not hide core content on mobile.
- Keep CTA sections visible and easy to access.
- Make navigation simple and usable.
- Keep text readable without horizontal scrolling.

---

## Motion Rules

Recommended motion:

- subtle fade in
- slow reveal
- card hover lift
- underline slide
- number count-up
- progress bar fill
- timeline step reveal

Avoid:

- bounce
- elastic motion
- neon glow
- infinite floating animation
- fast flashing
- large parallax effects
- layout-shifting animations

Always include reduced-motion support:

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

## Delivery Rules

When asked to create or modify a webpage:

1. Directly edit or create the relevant files.
2. Do not paste a full long HTML file in the chat unless explicitly requested.
3. After editing, summarize which files were changed.
4. Ensure the page is responsive.
5. Respect `prefers-reduced-motion`.
6. Include hover and focus states.
7. Make sure the result can be opened directly in a browser.
8. Do not leave placeholders unless the user explicitly asks for a template.
9. Do not create a half-finished structure.

---

## Quality Checklist

Before finishing, verify:

1. Does the page feel like a premium career studio?
2. Does it use ASCENDIA's deep navy and gold identity clearly?
3. Does it avoid generic AI-template visual patterns?
4. Does the hero explain who ASCENDIA is, what it does, and why it is credible within 10 seconds?
5. Does the page show a clear method, not just vague service claims?
6. Does the copy sound like a mentor rather than a salesperson?
7. Are there clear CTAs?
8. Is the page responsive?
9. Are default browser styles avoided for key components?
10. Would a screenshot of this page avoid the comment “又是 AI 做的”？

---

## Final Principle

ASCENDIA's visual identity must always be:

**professional, premium, structured, mentor-like, international, and human.**

The goal is not to make a flashy website. The goal is to make students and parents feel:

> “This team understands my career problem, has a clear method, and feels trustworthy enough to talk to.”
