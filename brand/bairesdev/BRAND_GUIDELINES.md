# BairesDev Brand Guidelines (Working Draft)

> Source-of-truth reference for generating presentations, decks, and documents
> in the BairesDev visual language using Claude Code.

**Status:** Working draft. Items marked `TO VERIFY` were inferred from public
rebrand coverage because `bairesdev.com`, `brandfetch.com`, and the official
brandbook PDF were not reachable from this sandbox (HTTP 403). Replace the
`TO VERIFY` values with the exact tokens from the official brandbook when
available.

**Primary reference:** [BairesDev Brandbook Summary (PDF)](https://bairesdev.mo.cloudinary.net/blog/editorial/rebranding_pdf_brandbook_summary.pdf)
**Companion file:** [`tokens.yaml`](./tokens.yaml) — same values, machine-readable.

---

## 1. Brand at a Glance

| Attribute | Value |
|---|---|
| Rebrand launched | 2023 |
| Campaign | "We Are Here" |
| Primary hue | **Orange** (replacing the historic blue) |
| Logo mark | Two semicircles (partnership, movement, shared purpose) |
| Identity system | Geometric shape system; elements move and affect each other |
| Voice attributes | Energetic, vital, confident, human, partnership-oriented |

Verified from: [Say Hello to Our New Brand](https://www.bairesdev.com/blog/say-hello-to-our-new-brand/), [Press — "We Are Here"](https://www.bairesdev.com/press/bairesdev-presents-new-brand-with-the-campaign-we-are-here/).

---

## 2. Color Palette

### 2.1 Primary

| Token | Name | HEX | RGB | Usage |
|---|---|---|---|---|
| `color.primary` | BairesDev Orange | `#F26B21` *(TO VERIFY)* | `242, 107, 33` | Main brand color. Headlines, CTAs, key accents. |
| `color.ink` | Ink / Near-Black | `#0E0E0E` *(TO VERIFY)* | `14, 14, 14` | Body text, logotype on light backgrounds. |
| `color.paper` | Paper / Off-White | `#FFFFFF` | `255, 255, 255` | Default background. |

### 2.2 Accent (from official palette — verify exact shades)

| Token | Name | HEX | RGB | Usage |
|---|---|---|---|---|
| `color.accent.blue` | Signal Blue | `#1E5FEA` *(TO VERIFY)* | `30, 95, 234` | Data viz, secondary CTAs, informational accents. |
| `color.accent.yellow` | Sun Yellow | `#F7C948` *(TO VERIFY)* | `247, 201, 72` | Highlights, callouts, caution states. |
| `color.accent.green` | Growth Green | `#00A86B` *(TO VERIFY)* | `0, 168, 107` | Positive/success states, growth metrics. |

> Per public coverage, the accent palette spans **orange, blue, yellow, green**.

### 2.3 Neutral scale (recommended for docs/decks)

| Token | HEX | Usage |
|---|---|---|
| `neutral.950` | `#0E0E0E` | Primary text |
| `neutral.800` | `#1F2937` | Headings on light bg |
| `neutral.600` | `#4B5563` | Secondary text |
| `neutral.400` | `#9CA3AF` | Disabled, metadata |
| `neutral.200` | `#E5E7EB` | Dividers, borders |
| `neutral.100` | `#F3F4F6` | Subtle backgrounds |
| `neutral.050` | `#FAFAFA` | Page background alt |

### 2.4 Usage rules

- **60 / 30 / 10**: 60% neutrals (paper + ink), 30% brand orange, 10% accent.
- Never set body copy in orange — reserve for headlines, accents, data marks.
- Maintain **WCAG AA** contrast: orange on white passes for large text only;
  for body size, use ink on paper or paper on orange.
- Avoid mixing more than **two accents** on a single slide/page.

---

## 3. Typography

> The official brandbook lists the specific typefaces. Until confirmed, use
> the pairings below — both are free, web-safe, and match the geometric,
> energetic tone of the rebrand.

### 3.1 Type stack (recommended working defaults)

| Role | Family (working) | Fallback | License |
|---|---|---|---|
| Display / Headlines | **Inter** (700–900) *(TO VERIFY vs brandbook)* | `system-ui, -apple-system, Segoe UI, Roboto, sans-serif` | OFL (free) |
| Body / UI | **Inter** (400–600) | same | OFL (free) |
| Mono / Code | **JetBrains Mono** | `ui-monospace, Menlo, Consolas, monospace` | OFL (free) |

> If the brandbook names a custom face (e.g., a Displaay / Grilli Type
> commission), replace Inter with that face and keep Inter as a web fallback.

### 3.2 Type scale (16px base)

| Token | Size | Line-height | Weight | Use |
|---|---|---|---|---|
| `display.xl` | 64 / 4rem | 1.05 | 800 | Cover slides, hero headlines |
| `display.lg` | 48 / 3rem | 1.1 | 700 | Section titles |
| `heading.1` | 32 / 2rem | 1.2 | 700 | Slide / page titles |
| `heading.2` | 24 / 1.5rem | 1.25 | 600 | Subsections |
| `heading.3` | 20 / 1.25rem | 1.3 | 600 | Card titles |
| `body.lg` | 18 / 1.125rem | 1.55 | 400 | Intro paragraphs |
| `body` | 16 / 1rem | 1.6 | 400 | Default body |
| `body.sm` | 14 / 0.875rem | 1.5 | 400 | Captions, metadata |
| `mono` | 14 / 0.875rem | 1.5 | 500 | Code, data |

### 3.3 Typographic rules

- Headlines: tight tracking (`-0.02em`), sentence case (no all-caps).
- Body: normal tracking, left-aligned, max 72ch measure.
- Never use more than **two weights** in the same heading hierarchy.

---

## 4. Logo

- **Mark:** two semicircles forming a whole — read as "us + clients" and
  "company + people." Always preserve the gap between semicircles.
- **Clear space:** minimum = height of one semicircle on all sides.
- **Minimum size:** 24px digital, 12mm print.
- **Color modes:** orange-on-paper (primary), paper-on-ink (dark mode),
  ink-on-paper (mono print). Never recolor to a non-brand hue.

Official assets: [Brandfetch — BairesDev](https://brandfetch.com/bairesdev.com),
[Seeklogo vector](https://seeklogo.com/vector-logo/505439/bairesdev).

---

## 5. Visual System

- **Geometric shape system**: circles, semicircles, and rounded rectangles
  act as containers for text, icons, and photography.
- **Motion principle**: elements affect each other — one shape's movement
  propagates. In static docs, imply this via overlapping shapes and
  directional composition.
- **Photography**: real people, natural light, candid over posed.
- **Iconography**: rounded, 2px stroke, geometric; align to the shape system.

---

## 6. Using These Tokens with Claude Code

### 6.1 For slide decks (HTML)

Point Claude at `brand/bairesdev/tokens.yaml` and ask for
`visual-explainer:generate-slides`. Example:

```text
Generate a 6-slide deck on "Q1 delivery metrics" using the brand tokens
defined in brand/bairesdev/tokens.yaml. Use BairesDev Orange for section
headers, neutral scale for body, and the geometric shape system for
decorative elements.
```

### 6.2 For documents (Markdown / PDF)

Ask Claude to apply tokens when rendering:

```text
Write a one-pager on <topic> styled with the BairesDev brand tokens in
brand/bairesdev/tokens.yaml. Headings in ink, accents in orange, max two
accent colors per page.
```

### 6.3 For diagrams

`visual-explainer:generate-web-diagram` — reference the tokens file and
request the geometric shape system (semicircles, rounded containers).

---

## 7. Verification Checklist

Before shipping any externally-facing artifact, confirm against the
official brandbook PDF:

- [ ] Primary orange hex matches brandbook
- [ ] Accent blue/yellow/green hex match brandbook
- [ ] Typeface names match brandbook (replace Inter if needed)
- [ ] Logo clear-space and minimum-size rules match brandbook
- [ ] Photography and iconography guidance match brandbook

---

## 8. Changelog

| Date | Change | Author |
|---|---|---|
| 2026-04-16 | Initial working draft from public rebrand sources | Claude Code |
