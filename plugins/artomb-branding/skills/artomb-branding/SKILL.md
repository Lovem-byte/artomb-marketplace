---
name: artomb-branding
description: "Use whenever creating or editing any ARTOMB Recruitment document, presentation, PDF, form, or spreadsheet, so the output follows ARTOMB's official colors, fonts, logo, and layout style."
---

# ARTOMB branding for every deliverable

Apply this skill any time someone asks for a PowerPoint/deck, Word document, PDF, form, or Excel/spreadsheet that is for ARTOMB Recruitment (internal or client-facing), unless they explicitly say it's an unbranded/internal working draft. This covers requests like "make a proposal deck," "create a client-facing PDF," "build a tracker in Excel," "draft a form for candidates," even when they don't say the word "branded."

This plugin ships the brand assets alongside this skill, under `assets/` (relative to this skill's own directory):
- `assets/ARTOMB_Brand_Guide.md` — the full brand guide (this file's quick reference, expanded, plus a typographic scale and layout notes)
- `assets/ARTOMB_PowerPoint_Template.pptx` — the official 11-layout master PowerPoint template to duplicate for decks
- `assets/logo-icon-purple.png` — icon mark, deep purple, for light backgrounds
- `assets/logo-icon-white.png` — icon mark, white/reversed, for dark backgrounds
- `assets/logo-lockup-white.png` — full logo lockup (icon + "ARTOMB RECRUITMENT" wordmark), white/reversed, for dark cover/closing pages

Read `assets/ARTOMB_Brand_Guide.md` for full detail when the quick reference below isn't enough. If this session is also attached to the "artomb design" Claude project, the same brand guide and template live there too (`artomb/ARTOMB_Brand_Guide.md`, `artomb/ARTOMB_PowerPoint_Template.pptx`) — either copy is authoritative; prefer whichever is reachable.

## Quick reference

**Colors** (never substitute other hues):
- Deep Purple `#1F0248` — primary/logo color, dark backgrounds, headings on light pages
- Secondary Purple `#3B1C68` — accents, filled circles/numbers
- Accent Gold `#D5A546` — the one pop color: subtitles, bullet accents, callout numbers, taglines, highlights — use sparingly
- Ink `#242330` — default body text on light backgrounds
- Muted Gray-Purple `#6B6874` — footers, captions, page numbers
- Light Tint `#F5F2F8` — card/table backgrounds on light pages
- White `#FFFFFF`

**Fonts** (never substitute):
- Headings, titles, numbers, pull-quotes: **Georgia, Bold** (italic Georgia for quotes/tagline)
- Body copy, labels, table text: **Arial, Regular** (Arial Bold for emphasis)

**Logo:** three assets — purple icon mark (light backgrounds), white icon mark (dark backgrounds), white full lockup with "ARTOMB RECRUITMENT" wordmark (large on dark cover/closing pages). Never recolor, rotate, or stretch the mark. On light backgrounds use the purple icon mark plus a typed "ARTOMB RECRUITMENT" wordmark in Georgia Bold — there is no purple full-lockup image. Use the bundled files in `assets/` (see above).

**Tagline:** *"Building Careers. Empowering Businesses."* — always italic, used near the logo or in a footer/closing area.

**Layout modes** — use only these two, never invent a third:
- *Dark:* Deep Purple full background, white headline text, gold for numbers/subtitles/tagline, one soft Secondary-Purple circle bleeding off a corner as the only decoration. Use for cover pages, section dividers, quotes/testimonials, closing pages.
- *Light:* white background, Deep Purple Georgia-Bold headings, Ink body text, gold for bullet markers/callout numbers, Light Tint for card/box fills. Use for standard content, tables, stats, agendas.

Every page/slide gets a small purple icon mark near the title (light pages) and a footer reading "ARTOMB RECRUITMENT" (Arial 9pt, Muted Gray-Purple) with a page number, unless the deliverable is a single-page form or one-pager where a header lockup replaces the footer.

## Per-format instructions

**PowerPoint (.pptx) / the Slides artifact type:** Don't build slides from a blank theme. Duplicate/adapt the layouts already in `assets/ARTOMB_PowerPoint_Template.pptx` (title, section divider, standard content, two-column comparison, content+image, stats/"By the Numbers", testimonial, numbered process, closing) with python-pptx or the pptx skill, keeping the exact colors, fonts, and placeholder positions from that file, and swap in the new content. Only design a new layout from scratch if none of the 11 existing layouts fit, and in that case still use the palette/fonts/logo rules above.

**Word documents / PDFs:** White page; Deep Purple Georgia-Bold headings; Arial 11pt body; a simple letterhead (purple icon mark + "ARTOMB RECRUITMENT" wordmark in Georgia Bold) top-left of page 1 or centered on a cover page; Muted Gray-Purple footer with the tagline or contact line; gold used sparingly for a rule under the title or for callout/pull-quote boxes (Light Tint fill, Deep Purple text).

**Excel workbooks:** Header row filled Deep Purple with white Arial Bold text; Light Tint for alternating row shading; gold reserved for a single highlight column, key totals, or conditional formatting; Georgia Bold for any title/section labels above tables; Arial for all cell data; company name in a small header or footer.

**Forms (web or PDF):** White or Light Tint background; Deep Purple Georgia-Bold section headings; Arial labels/body; gold for required-field markers or the submit button; purple icon mark in the header; ARTOMB contact line in the footer.

## Guardrails

- Never introduce colors or fonts outside this palette, even "close enough" substitutes, unless the target tool truly can't render Georgia/Arial — in that case pick the closest serif/sans-serif and say what was substituted.
- Never recolor, rotate, skew, or stretch the ARTOMB mark, and never place the purple mark on a dark background or the white mark on a light one.
- If the bundled `assets/` files and the "artomb design" project are both unreachable, still apply the quick-reference palette/fonts/tagline above from memory rather than guessing at ARTOMB's branding.
- If ARTOMB's branding changes (new color, font, or rule), update this skill and its bundled assets, and, if the "artomb design" project is attached, refresh `artomb/ARTOMB_Brand_Guide.md` there too so both stay in sync.

