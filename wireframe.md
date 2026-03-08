# Single-Page Web Portfolio — Wireframe & Content Plan

> **Document Type:** Text-Based Wireframe & Content Blueprint
> **Layout:** Single-page, vertically scrolling, fully responsive
> **Target:** Clean, professional, accessible (WCAG 2.1 AA)

---

## Visual Wireframe (ASCII)

```
┌──────────────────────────────────────────────────────────┐
│                       NAVIGATION BAR                     │
│  Logo / Name              About | Skills | Projects | Contact │
│  (sticky on scroll)                                      │
├──────────────────────────────────────────────────────────┤
│                                                          │
│                      HERO SECTION                        │
│                                                          │
│             "Hello, I'm [INSERT YOUR NAME]"              │
│              Web Developer · Hybrid Athlete              │
│                                                          │
│              [ View My Work ]  (CTA button)              │
│                                                          │
├──────────────────────────────────────────────────────────┤
│                                                          │
│                    ABOUT / BIO SECTION                   │
│                     (#about)                             │
│                                                          │
│   ┌──────────┐  "I am a web developer based in Egypt.   │
│   │  Profile  │   When I'm not writing code, I'm a      │
│   │  Image    │   hybrid athlete currently training for  │
│   │ Placeholder│  my first Hyrox race, balancing a       │
│   └──────────┘   strict routine of running and strength  │
│                  training."                              │
│                                                          │
├──────────────────────────────────────────────────────────┤
│                                                          │
│                     SKILLS SECTION                       │
│                      (#skills)                           │
│                                                          │
│   ┌────────────────────────────────────────────────┐     │
│   │         [INSERT TECH SKILLS HERE]              │     │
│   │                                                │     │
│   │  Displayed as a responsive grid of cards/tags  │     │
│   │  e.g. HTML, CSS, JavaScript, Python, React...  │     │
│   └────────────────────────────────────────────────┘     │
│                                                          │
├──────────────────────────────────────────────────────────┤
│                                                          │
│                    PROJECTS SECTION                      │
│                     (#projects)                          │
│                                                          │
│   ┌──────────────┐  ┌──────────────┐  ┌──────────────┐  │
│   │  Project 1   │  │  Project 2   │  │  Project 3   │  │
│   │  Thumbnail   │  │  Thumbnail   │  │  Thumbnail   │  │
│   │              │  │              │  │              │  │
│   │  Title       │  │  Title       │  │  Title       │  │
│   │  Description │  │  Description │  │  Description │  │
│   │  [Live] [Code]│ │  [Live] [Code]│ │  [Live] [Code]│ │
│   └──────────────┘  └──────────────┘  └──────────────┘  │
│                                                          │
│   [INSERT PROJECT DETAILS HERE]                          │
│                                                          │
├──────────────────────────────────────────────────────────┤
│                                                          │
│                    CONTACT SECTION                       │
│                     (#contact)                           │
│                                                          │
│   "Let's work together."                                 │
│                                                          │
│   [INSERT EMAIL ADDRESS HERE]                            │
│   [INSERT LINKEDIN URL HERE]                             │
│   [INSERT GITHUB URL HERE]                               │
│                                                          │
│   Optional: simple contact form                          │
│   [ Name ] [ Email ] [ Message ]                         │
│   [ Send Message ]                                       │
│                                                          │
├──────────────────────────────────────────────────────────┤
│                        FOOTER                            │
│   © 2026 [INSERT YOUR NAME]. All rights reserved.        │
└──────────────────────────────────────────────────────────┘
```

---

## Content Plan — Section by Section

### 1. Navigation Bar
- **Purpose:** Persistent site navigation via anchor links.
- **Elements:**
  - Logo or name (text-based)
  - Links: About, Skills, Projects, Contact
- **Behaviour:** Sticky positioning; hamburger menu on mobile.
- **Accessibility:** `<nav>` landmark, `aria-label="Main navigation"`, keyboard-navigable.

### 2. Hero Section
- **Purpose:** Immediate visual hook; communicates identity.
- **Heading:** `[INSERT YOUR NAME]`
- **Subheading:** "Web Developer · Hybrid Athlete"
- **CTA Button:** "View My Work" → scrolls to `#projects`
- **Design:** Full-viewport height, subtle gradient background, fade-in animation.

### 3. About / Bio Section
- **Purpose:** Personal story and professional identity.
- **Content (provided):**
  > "I am a web developer based in Egypt. When I'm not writing code, I'm a hybrid athlete currently training for my first Hyrox race, balancing a strict routine of running and strength training."
- **Layout:** Two-column on desktop (image + text), single-column on mobile.
- **Image:** Placeholder slot for profile photo.
- **Accessibility:** `alt` text on image, heading hierarchy.

### 4. Skills Section
- **Purpose:** Showcase technical competencies at a glance.
- **Content:** `[INSERT TECH SKILLS HERE]` — rendered as a grid of pill-shaped tags or cards.
- **Layout:** Responsive grid (auto-fill, min 120 px).
- **Accessibility:** Semantic list (`<ul>`), sufficient colour contrast on tags.

### 5. Projects Section
- **Purpose:** Portfolio evidence — what you've built.
- **Content:** `[INSERT PROJECT DETAILS HERE]` — three project card placeholders, each with:
  - Thumbnail image placeholder
  - Project title
  - Short description
  - "Live Demo" link placeholder
  - "Source Code" link placeholder
- **Layout:** Three-column grid on desktop → single-column on mobile.
- **Accessibility:** Descriptive link text, card structure via `<article>`.

### 6. Contact Section
- **Purpose:** Clear call-to-action for outreach.
- **Content:**
  - `[INSERT EMAIL ADDRESS HERE]`
  - `[INSERT LINKEDIN URL HERE]`
  - `[INSERT GITHUB URL HERE]`
- **Optional:** Simple form (Name, Email, Message, Submit).
- **Accessibility:** `<form>` with `<label>` elements, focus indicators.

### 7. Footer
- **Content:** Copyright line with name placeholder.

---

## Design Principles

| Principle        | Implementation                                              |
|------------------|-------------------------------------------------------------|
| **Clean**        | Generous whitespace, limited colour palette, readable fonts |
| **Professional** | Neutral tones accented with one brand colour                |
| **Responsive**   | CSS Grid + Flexbox, mobile-first breakpoints                |
| **Accessible**   | Semantic HTML5, ARIA labels, focus styles, colour contrast  |

---

## Colour Palette (planned)

| Token             | Value       | Usage                      |
|--------------------|-------------|----------------------------|
| `--clr-bg`         | `#0f172a`   | Page background (dark)     |
| `--clr-surface`    | `#1e293b`   | Card / section background  |
| `--clr-text`       | `#e2e8f0`   | Primary text               |
| `--clr-text-muted` | `#94a3b8`   | Secondary / muted text     |
| `--clr-accent`     | `#38bdf8`   | Links, buttons, highlights |
| `--clr-accent-hover`| `#7dd3fc`  | Hover state                |

---

## Typography (planned)

| Role     | Font                | Weight  |
|----------|---------------------|---------|
| Headings | Inter (Google Fonts)| 700     |
| Body     | Inter (Google Fonts)| 400     |
| Code     | monospace fallback  | 400     |

---

## File Inventory (planned)

| File                | Purpose                                       |
|---------------------|-----------------------------------------------|
| `wireframe.md`      | This document — wireframe & content plan      |
| `index.html`        | Portfolio page markup                         |
| `index.css`         | All styles                                    |
| `manual.md`         | Step-by-step instructional guide for beginners |
| `README.md`         | Submission cover sheet with file list          |
