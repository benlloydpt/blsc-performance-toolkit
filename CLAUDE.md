# BLSC Performance Toolkit — Claude Code Context

## Who I Am

I'm Ben Lloyd, founder of **Ben Lloyd Strength & Conditioning (BLSC)** — an online coaching business targeting athletic men aged 30–50 across hybrid training, CrossFit, HYROX, triathlon, and Olympic lifting.

This repo contains the **BLSC Performance Toolkit**: a suite of GitHub Pages-hosted lead generation tools designed to attract and convert my target audience.

---

## Brand Identity

### Colours
| Role       | Hex       | Usage                                      |
|------------|-----------|--------------------------------------------|
| Primary    | `#2d7ee0` | CTAs, headers, key UI elements             |
| Secondary  | `#ffffff`  | Text on dark, card backgrounds             |
| Accent     | `#00fff0` | Highlights, hover states, data callouts    |
| Background | `#0d0d0d` | Page background (dark mode default)        |
| Surface    | `#1a1a1a` | Cards, panels, input backgrounds           |
| Muted text | `#888888` | Labels, secondary copy                     |

### Typography
- **Font family:** Inter (Google Fonts)
- **Weights used:** 400 (body), 600 (subheadings), 700 (headings), 800 (hero/display)
- **Scale:** Base 16px. H1: 2.5rem, H2: 1.75rem, H3: 1.25rem

### Mode
- **Dark mode by default** — always build for dark backgrounds first

### Logo / Wordmark
- Use "BLSC" as the wordmark in `#2d7ee0`
- Tagline: *"Train Smarter. Perform Better."* (use sparingly)

---

## Design Principles

1. **Athlete-first UI** — clean, performance-dashboard aesthetic. No fluff.
2. **Mobile-first** — most users will be on phones. Build mobile, enhance for desktop.
3. **CTA-driven** — every tool should have a clear lead capture or next step (e.g. email opt-in, link to coaching enquiry)
4. **Consistent layout** — all tools should feel like they belong to the same product suite
5. **Fast and lightweight** — vanilla HTML/CSS/JS preferred unless a library meaningfully improves UX

---

## UI Component Standards

### Buttons
```css
/* Primary CTA */
background: #2d7ee0;
color: #ffffff;
border-radius: 6px;
padding: 12px 24px;
font-weight: 700;
font-size: 1rem;
border: none;
cursor: pointer;

/* Hover state */
background: #00fff0;
color: #0d0d0d;
```

### Cards / Panels
```css
background: #1a1a1a;
border: 1px solid #2a2a2a;
border-radius: 10px;
padding: 24px;
```

### Inputs
```css
background: #111111;
border: 1px solid #333333;
border-radius: 6px;
color: #ffffff;
padding: 10px 14px;
font-family: Inter, sans-serif;
```

### Accent highlights / result callouts
```css
color: #00fff0;
font-weight: 700;
```

---

## Page Layout Template

Every tool should follow this structure:

```
[BLSC wordmark / nav]
[Tool title + one-line description]
[Input section]
[Results / output section]
[CTA — email opt-in or coaching enquiry link]
[Footer with BLSC branding]
```

Nav and footer should be identical across all tools.

---

## The Toolkit — Tool List

| Tool                         | Status      | Slug                        |
|------------------------------|-------------|-----------------------------|
| Running Pace Calculator      | ✅ Live      | `/running-pace-calculator`  |
| Hybrid Readiness Score       | 🔧 Planned  | `/hybrid-readiness-score`   |
| Strength Standards Calculator| 🔧 Planned  | `/strength-standards`       |
| HYROX Finish Time Predictor  | 🔧 Planned  | `/hyrox-predictor`          |
| Training Age Calculator      | 🔧 Planned  | `/training-age`             |
| Zone 2 Heart Rate Finder     | 🔧 Planned  | `/zone-2-finder`            |

All tools are standalone HTML pages hosted on GitHub Pages.

---

## Tone of Voice

- **Direct and no-nonsense** — respect the user's intelligence
- **Athlete-centric** — speak to people who train seriously
- **Professional but human** — not corporate, not bro-y
- **Action-oriented** — results, improvements, next steps
- **Target audience:** Men aged 30–50, athletic mindset, data-driven about their training

### Example microcopy
- ✅ "Find your target pace." — not ❌ "Discover your amazing running pace today!"
- ✅ "Your Zone 2 ceiling is 148 bpm." — not ❌ "Great news! Here are your results!"
- ✅ "Book a free call." — not ❌ "Click here to learn more about our services!"

---

## Lead Generation

- Every tool should capture an email or direct to: **[coaching enquiry / Typeform link]**
- CTA copy: *"Want a programme built around your numbers? Book a free call."*
- Email opt-in label: *"Get your results + a free training resource"*
- Keep friction low — first name + email only

---

## Technical Standards

- **Platform:** GitHub Pages (static only — no server-side code)
- **Stack:** HTML5, CSS3, vanilla JavaScript (preferred). Use CDN libraries only if necessary.
- **No build tools required** — everything should work as flat files
- **Inter font:** Load via Google Fonts CDN
  ```html
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap" rel="stylesheet">
  ```
- **Responsive breakpoints:** Mobile < 768px, Tablet 768–1024px, Desktop > 1024px
- **File naming:** kebab-case for all files and folders
- **Shared assets:** Store shared CSS and nav/footer partials in `/assets/`

---

## Data Assets

- `blsc_strength_standards.json` — Strength standards dataset (bodyweight multipliers by lift and level). Reference this for the Strength Standards Calculator.

---

## What I'm NOT building

- No WordPress, no CMS, no backend
- No paid hosting — GitHub Pages only
- No React/Vue/Angular — keep it vanilla unless there's a compelling reason

---

## When Building a New Tool

1. Copy the layout template above
2. Use the exact colour values — no approximations
3. Load Inter from Google Fonts
4. Match nav and footer to existing tools exactly
5. Include a lead capture CTA before the closing `</body>`
6. Test on mobile width first
7. Name the file `index.html` inside the tool's slug folder

---

*Last updated: April 2026 | Ben Lloyd — BLSC*
