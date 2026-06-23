# LogX — Design System

> **Inspire like a maison. Operate like a machine.**

This repository is the brand & design system for **LogX**, distilled from the official pitch deck
(`uploads/LogX_Pitch_May25v2.pdf`, May 2025 v2). It contains the colour system, typography, visual
foundations, reusable components, and a faithful recreation of the pitch-deck slide template so that
any agent or designer can produce on-brand LogX artefacts.

---

## 1. Company & product context

**LogX** is a B2B SaaS venture by **OSS Ventures** (an "IA venture studio"). It is an **orchestration
layer for luxury-maison distribution networks** — it sits *on top of* a brand's existing stack
(POS · ERP · Buying tool · Planning/Anaplan/APS · WMS · field signals) and connects
**forecast → buy → assortment → replenishment → rebalancing** into a single continuous, signal-driven
loop. It is explicitly **not** a new system of record, a planning tool, a BI dashboard, or a multi-year
custom build.

**The pitch in one line:** recover ~10 points of sell-through without changing your systems, by turning
four disconnected silos (forecast, assortment, replenishment, rebalancing) into one real-time loop owned
by a maison's distribution architects.

**Product architecture (4 layers, from the deck):**
1. **Dashboards UI** — what stakeholders see (Management · Merchandising · Distribution · Retail).
2. **Operator UI** — planning architects configure rules, validate edges, improve.
3. **Orchestration** — the *LogX Loop* + *Maison Knowledge Graph*: signal capture, loop logic,
   auto-execution within rules, edge prioritisation.
4. **Systems of record** — the customer's existing stack (untouched).

**Audience / tone:** sold to Tier-1 luxury maisons (the deck references door-level EMEA pilots,
permanent + seasonal SKU mixes). The deck targets COMEX sponsors and merchandising/distribution leads.

**Team (from the deck, marked "to fill in"):** Jean-Philippe Stouff (co-founder, GTM & operator),
Aurore Malmenayde (co-founder, luxury merchandising — ex Louis Vuitton, Saint Laurent), and OSS Ventures
(the studio — 22 companies, 3,800+ clients, €34m ARR portfolio).

### Sources given
- `uploads/LogX_Pitch_May25v2.pdf` — 16-page pitch deck. The **only** source asset.
  - Fully vector/text (no embedded raster images or logos — the "LOGX" wordmark is set type).
  - No codebase, Figma, or product screenshots were provided. **No live product UI exists in the
    materials** — the product is pre-pilot ("in discussion", "two seats open").

> ⚠️ Because no product UI, codebase, or Figma was provided, the **slide template** (`slides/`) is the
> primary, faithful deliverable. The UI kit (`ui_kits/logx-console/`) is a *disciplined extrapolation*
> of the product described in the deck's architecture slide, built strictly from the deck's established
> visual language. It is clearly disclaimed as such — see its README.

---

## 2. Content fundamentals — how LogX writes

The copy is **editorial, confident, and consultative** — closer to a luxury strategy memo than a
typical SaaS site. Specifics:

- **Voice & person:** addresses the client directly as **"you / your"** ("your distribution network",
  "your systems", "your people investment"). LogX refers to itself in the third person ("LogX is…",
  "What we deliver", "Our part"). First-person plural ("we") for the team's commitments.
- **Casing:** **Sentence case** for headlines and body. **UPPERCASE** reserved for eyebrow/kicker
  labels and metric captions (`THE NEW EDGE`, `OWNER`, `KPI`, `TOOL`, `OF REVENUE, MISSED EVERY SEASON`).
  Section tags in the top corners are uppercase (`WHY US`, `THE P&L COST`, `WHAT LOGX IS — AND ISN'T`).
- **Headlines** are short, declarative, often two-part and provocative:
  *"The rules just changed. Missed opportunity is no longer affordable."*
  *"Past a certain size, your distribution network stops being pilotable."*
  *"This isn't an operational problem. It's a P&L problem."*
- **Rhythm:** heavy use of **short fragments and triads** — "One loop. Everyone aligned.",
  "Four silos. Four KPIs. No one owns the network.", "Scope, team, pacing." Em dashes and middots (·)
  separate list items inline.
- **The arrow `→`** is a signature glyph for the loop and transitions: `forecast → buy → assortment →
  replen → rebalancing`, `3 → 20+ weeks`, `Today / Tomorrow`.
- **Numbers carry the argument:** big, specific, range-based stats (`1,000+`, `20 – 40%`, `+5 – 10 pts`,
  `−10 – 15%`, `2 – 4%`). Ranges use a spaced en-dash ` – `.
- **Domain register:** fluent in both luxury ("maison", "doors", "sell-through", "carryover",
  "seasonals") and finance/ops ("Comex metric", "weeks of coverage", "working capital", "P&L impact",
  "service rate"). This duality is the brand.
- **No emoji. No exclamation marks** (except the closing "Let's go?"). No emoji ever.
- **Vibe:** measured, premium, a little severe — "operate like a machine." Confidence without hype.

---

## 3. Visual foundations

**Overall impression:** a quiet-luxury / "maison memo" aesthetic — deep forest green, warm ivory paper,
and champagne gold, set in a single clean geometric-humanist sans (Lexend). Editorial, generous
whitespace, hairline rules, almost no shadow or gradient. It reads like a high-end consulting document.

### Colour
- **Primary:** Deep pine green `#1f3a2e` (dark slide backgrounds, feature cards). Near-black green
  `#14211b` is the ink colour on light and the darkest fills.
- **Paper:** Ivory `#faf7f1` (the default light background) and sand `#efe9dc` (highlight panels /
  active rows / quote blocks).
- **Accent:** Champagne gold `#d6c89a` — used for eyebrow labels and accent words on dark, and the
  second line of the cover headline. On light backgrounds gold is darkened to `#a8884a` for legibility.
- **Text grey:** muted sage `#5a6660` for subheads and body on light.
- **Vibe of palette:** warm, desaturated, organic. No bright/saturated colours, no blue-purple,
  no neon. Two backgrounds max per deck (pine dark + ivory light).

### Typography
- **Single family: Lexend** (weights 300/400/500/600/700). Loaded from Google Fonts — this is the
  deck's *actual* typeface, not a substitution.
- **Headlines:** Lexend **Bold (700)**, large (≈48–60px on a 1280-wide slide), very tight line-height
  (~1.04), slight negative tracking. Sentence case.
- **Big stats:** Lexend **Light (300)**, very large, used for the hero numerals.
- **Subheads/body:** Lexend Regular (400), 16–20px, sage grey, relaxed line-height (~1.5).
- **Eyebrows / kickers:** Lexend SemiBold (600), ~11px, UPPERCASE, letter-spacing ~0.16em.
- **Italic** is used for pull-quotes and accent phrases ("*Without changing your systems*", testimonial
  quotes, team bios).

### Spacing & layout
- **8-pt spacing scale.** Generous margins; content sits in a wide centred column with large top/left
  padding. Headlines hang at the top-left; supporting content fills below in 2–3 columns.
- **Fixed slide furniture:** tiny `LOGX PITCH` wordmark top-left; optional section tag top-right;
  page number `NN / 15` bottom-right; all in the eyebrow style. Cover adds a bottom-left footer
  ("A new venture by OSS Ventures").
- **Grids:** 3-column feature rows; horizontal "layer table" rows; side-by-side 2-up comparisons.

### Backgrounds
- **Flat colour only** — ivory or pine. **No photography, no gradients, no textures, no illustration,
  no pattern.** Imagery is entirely typographic/diagrammatic. (If a future asset needs a photo, treat
  it as warm, muted, editorial.)

### Borders, dividers, cards, elevation
- **Hairlines do the work, not shadows.** 1px rules in sand `#d8d0ba` separate sections; a slightly
  heavier rule (often gold-tinted) tops the layer table.
- **Cards:** white fill + 1px sand border, barely-rounded corners (**~4px radius**), generous padding.
  A **feature card** inverts to a pine-green fill with cream text. A **highlight panel** uses sand fill
  (`#efe9dc`) with no border.
- **Chips/tags:** small, 1px sand border, sentence or UPPERCASE micro-text, dark ink, ~4px radius.
- **Elevation:** essentially flat. Shadows are reserved for transient UI (menus, popovers) in the
  console kit, never on the deck. Corner radii stay small (2–8px); nothing is pill-rounded except
  optional toggles/chips.

### Motion
- The deck is static. For interactive recreations, keep motion **restrained and editorial**: short
  fades and 150–250ms ease-outs (`cubic-bezier(0.2, 0.6, 0.2, 1)`), subtle. **No bounce, no spring, no
  decorative looping animation.** Hover = slight darkening / border emphasis; press = ~1–2% scale-down
  or a step darker. Respect `prefers-reduced-motion`.

### Transparency & blur
- Used sparingly. On dark, gold hairlines are gold at ~28% alpha (`--line-dark`). No glassmorphism /
  heavy blur in the source — avoid unless building modern console chrome, and keep it subtle.

---

## 4. Iconography

The pitch deck contains **no icon set, no icon font, and no SVG/PNG icon assets** — it is purely
typographic and diagrammatic. The brand's "iconography" is therefore:

- **Typographic glyphs as icons:** the arrow **`→`** (loop steps, transitions), the **middot `·`** and
  **em dash `—`** as inline separators, and small **▲ ▼** triangles to indicate the bidirectional loop
  in the architecture/layer diagram.
- **Numbered kickers:** sequences like `01`, `02`, `03` set in the eyebrow style act as visual markers.
- **No emoji. No decorative illustration.**

**For new work that needs UI icons** (e.g. the console kit): there is no native set to copy, so use
**[Lucide](https://lucide.dev)** (linked from CDN) — its thin, geometric, 1.5–2px stroke style matches
Lexend and the restrained aesthetic. This is a **documented substitution** (no source icons exist);
keep usage minimal, monochrome (ink or sage), and never filled/colourful. Prefer the brand's own
typographic glyphs (`→ · —`) wherever they read clearly.

> No raster logos or imagery were extractable from the deck (the wordmark is set type). The wordmark is
> reproduced as styled text — see `assets/logo.html` and the Brand cards in the Design System tab.

---

## 5. Index / manifest

Root files:
- **`README.md`** — this file.
- **`colors_and_type.css`** — CSS custom properties (palette, type scale, spacing, radii, elevation)
  + semantic helper classes (`.logx-display`, `.logx-eyebrow`, `.logx-stat`, …). Import this everywhere.
- **`SKILL.md`** — Agent-Skills-compatible entry point.

Folders:
- **`assets/`** — brand marks (wordmark lockups as HTML/SVG-free styled type), reusable token notes.
- **`preview/`** — small HTML cards that populate the Design System tab (colours, type, spacing,
  components, brand). Not for reuse — these are documentation specimens.
- **`slides/`** — the **pitch-deck template** recreation. `index.html` runs the full deck; each
  `*.jsx` is one slide layout (cover, three-up, loop, layer table, stats, team, comparison, closing).
  This is the primary faithful deliverable.
- **`ui_kits/logx-console/`** — a disclaimed extrapolation of the LogX product console
  (loop board, edge queue, door-coverage, weekly readout) in the brand language.
  See its README for the disclaimer.

---

*Generated for OSS Ventures / LogX. Source: LogX_Pitch_May25v2.pdf.*
