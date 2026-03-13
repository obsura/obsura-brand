# Brand System Freeze

> Status: approved reference direction extracted from `assets/samples_ui_ux`
> on 2026-03-13.

This document turns the sample UI set under `assets/samples_ui_ux/` into the
frozen visual direction for Obsura.

The text, product names, and product scenarios shown in those images are not
Obsura content. Only the repeated visual patterns, component treatments, and
interaction cues are adopted here.

See also: [Visual Direction](visual-direction.md),
[Design Foundations](design-foundations.md),
[Design Tokens](design-tokens.md),
[Component Guidelines](component-guidelines.md)

## Source Set

Use the full `assets/samples_ui_ux/` directory as the approved reference set
for this freeze.

Those files are:

- reference-only
- useful for extracting structure, tone, palette balance, and component style
- not official Obsura marketing or product artwork
- not reusable as published Obsura assets

## Brand Sentence

Obsura should look like a calm privacy workbench: light, precise, and quietly
premium, with enough softness to feel approachable and enough structure to feel
safe.

## Repeating Signals In The Sample Set

These traits appear across the reference images often enough to treat them as
the stable system:

- light neutral canvases instead of dark security dashboards
- white elevated cards and floating tool surfaces
- restrained periwinkle action color with pale blue and pale lavender support
  tones
- mint, amber, and coral semantic accents used sparingly
- rounded rectangles, pill tabs, and softened container edges
- hairline borders with shallow ambient shadows
- medium-weight sans typography with roomy, disciplined spacing
- contextual menus, floating toolbars, side inspectors, and structured data
  views
- simple geometric iconography, mostly outline-led inside product UI

## Obsura Signature

The Obsura brand system should preserve those signals in this form:

- light-first chrome for app shell, docs, and marketing surfaces
- one calm action color instead of multiple competing accents
- soft precision: rounded corners and gentle depth around highly structured
  content
- content-first workspaces where the review target remains more important than
  the frame around it
- dark surfaces only when the task benefits, such as image review, comparison,
  or code-heavy inspection
- no cyber-noir styling, no hacker green, no heavy black default chrome, and no
  decorative gradients as the main identity

## Adopt

- warm paper and mist neutrals as the default base
- white cards with subtle border plus shadow separation
- periwinkle as the primary action and focus color
- ice blue and lavender as supporting highlight and selection tones
- large but controlled radii for cards, menus, and input shells
- compact, high-clarity toolbars and menus
- left-nav plus main canvas plus right-inspector layouts where the workflow
  needs them
- semantic status chips that stay soft rather than loud
- clean, technical typography with a strong monospace companion

## Reject

- dark-mode-as-brand
- high-contrast neon color systems
- glossy gradients or glow-heavy buttons
- crowded enterprise chrome
- brutalist hard edges
- playful blobs, mascot styling, or whimsical illustration-led framing
- red-heavy warning palettes as a default visual language

## Core Palette Snapshot

The extracted palette direction is:

- paper neutrals around `#FCFBF9`, `#F5F3F0`, and `#ECE8E4`
- ink neutrals around `#171717`, `#4B4B4B`, and `#7C7772`
- primary periwinkle around `#5B4CE3`
- soft lavender around `#E9E5FF`
- soft ice blue around `#DDF3FF`
- mint success around `#7FD698` to `#89E67A`
- amber warning around `#E8A63C`
- coral danger around `#E57F73`

The full role-based token mapping lives in
[Design Tokens](design-tokens.md).

## Component Freeze

Across the reference set, the stable component language is:

- floating menus and popovers with 12px to 16px radius
- pill or segmented filters sitting on muted rails
- inputs and command bars with quiet borders and strong internal padding
- cards that carry metrics, lists, or actions without oversized decoration
- inspectors and overlays that feel layered but not detached
- tables and list rows that prioritize scanability over dense ornament
- AI assistance that appears as compact, contextual support rather than a full
  takeover

Obsura should translate that language into review-specific components such as:

- detection lists
- redaction inspectors
- review canvases
- compare states
- export summaries
- risk and confidence badges

## Practical Translation For Obsura

The references are mostly general productivity UI. Obsura should inherit the
surface language, not the product metaphors.

That means:

- keep the calm white-card and mist-shell styling
- adapt highlight and badge systems for detect, review, approve, replace, and
  export workflows
- reserve strong dark fills for actual redaction outputs or focused inspection
  surfaces
- keep AI suggestions secondary to manual review and explicit user decisions

## Freeze Rule

If a future design proposal moves Obsura toward a darker, louder, or more
security-theater-heavy direction than this reference set, treat that as a brand
change and update this repository deliberately rather than letting it drift in a
downstream app.
