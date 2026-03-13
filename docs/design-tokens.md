# Design Tokens

> Status: approved reference token vocabulary for future implementation
> repositories.

This document defines the approved reference token system for Obsura. These
names and values are intended to guide future translation into Tailwind, CSS
variables, or component libraries in repositories such as `obsura-web`.

See also: [Brand System Freeze](brand-system-freeze.md),
[Design Foundations](design-foundations.md), [UI Principles](ui-principles.md)

## Token Philosophy

Tokens should express stable design intent rather than one-off styling choices.
The values below freeze the current brand system derived from the reference UI
sample set.

They should help future repos answer:

- what visual role something has
- how dense or spacious a surface should feel
- which layer or state a component belongs to
- how motion and elevation should behave

## Color Tokens

### Background, Surface, Border, And Text

| Token | Value | Role |
| --- | --- | --- |
| `color-bg-app` | `#F5F3F0` | outer app shell, page frame, broad backdrop |
| `color-bg-canvas` | `#FCFBF9` | main page background and long-form content areas |
| `color-surface-muted` | `#F3F1EE` | grouped controls, segmented rails, muted cards |
| `color-surface-primary` | `#FFFFFF` | cards, forms, menus, dialogs, inspectors |
| `color-surface-secondary` | `#F8F7F5` | secondary cards and recessed subpanels |
| `color-surface-contrast` | `#1E1E22` | dark review canvas, final redaction fill, inverse blocks |
| `color-border-subtle` | `#ECE7E2` | low-emphasis separators |
| `color-border-default` | `#E2DDD8` | default control and card border |
| `color-border-strong` | `#CFC7C0` | stronger grouping boundary |
| `color-text-primary` | `#171717` | headings, labels, critical values |
| `color-text-secondary` | `#4B4B4B` | body copy and supporting metadata |
| `color-text-tertiary` | `#7C7772` | helper text, inactive labels, placeholders |
| `color-text-inverse` | `#FFFFFF` | text on periwinkle or dark contrast surfaces |

### Accent And Semantic

| Token | Value | Role |
| --- | --- | --- |
| `color-accent-primary` | `#5B4CE3` | primary action, active state, strong emphasis |
| `color-accent-primary-hover` | `#4E40D5` | primary hover |
| `color-accent-primary-pressed` | `#4336BF` | primary active |
| `color-accent-soft` | `#E9E5FF` | soft selected state and accent-backed badges |
| `color-focus-ring` | `#A39AF5` | keyboard focus ring and focus glow |
| `color-info` | `#DDF3FF` | informational surface tint |
| `color-info-strong` | `#4890DB` | stronger informational icon or marker |
| `color-success` | `#7FD698` | success, approved, healthy |
| `color-success-muted` | `#E9F9EE` | muted success surfaces |
| `color-warning` | `#E8A63C` | caution and pending states |
| `color-warning-muted` | `#FFF3DE` | muted warning surfaces |
| `color-danger` | `#E57F73` | destructive and risk states |
| `color-danger-muted` | `#FDEAE6` | muted destructive surfaces |

### Review Workflow

| Token | Value | Role |
| --- | --- | --- |
| `color-detect-auto` | `#DDF3FF` | auto-detected span or region |
| `color-detect-manual` | `#E9E5FF` | manually created region or user-owned marker |
| `color-selection` | `#F2EEFF` | active selected row, block, or highlight |
| `color-selection-strong` | `#CFC6FF` | selected outline or stronger selected fill |
| `color-redaction-fill` | `#1E1E22` | final redaction block or hidden-content mask |
| `color-redaction-outline` | `#5B4CE3` | editable overlay edge, resize, or active region |
| `color-replacement-fill` | `#F3F1EE` | replacement chip, replacement preview, neutral reviewed state |
| `color-confidence-low` | `#FDEAE6` | low-confidence badge or caution card |
| `color-confidence-medium` | `#FFF3DE` | medium-confidence badge or review-needed state |
| `color-confidence-high` | `#E9F9EE` | high-confidence badge or approved state |

## Spacing Tokens

| Token | Value | Role |
| --- | --- | --- |
| `space-1` | `4px` | tight icon gaps and micro spacing |
| `space-2` | `8px` | chip padding and dense inline spacing |
| `space-3` | `12px` | default control padding and small card gaps |
| `space-4` | `16px` | default card padding and stacked element gaps |
| `space-5` | `20px` | medium container padding |
| `space-6` | `24px` | section padding and card-to-card spacing |
| `space-8` | `32px` | shell padding and major content separation |
| `space-10` | `40px` | wide layout spacing |
| `space-12` | `48px` | large sectional separation |
| `space-16` | `64px` | page-level breathing room |

## Radius Tokens

| Token | Value | Role |
| --- | --- | --- |
| `radius-xs` | `8px` | tiny chips and compact badges |
| `radius-sm` | `12px` | buttons, inputs, menus |
| `radius-md` | `16px` | cards, popovers, inspector panels |
| `radius-lg` | `20px` | shell sections and larger cards |
| `radius-xl` | `24px` | hero cards, large modals, statement containers |
| `radius-pill` | `999px` | pills, segmented controls, chips when intentional |

## Typography Tokens

### Families, Sizes, Weights, And Line Height

| Token | Value | Role |
| --- | --- | --- |
| `font-family-sans` | `"Geist", "Segoe UI", sans-serif` | interface and brand text |
| `font-family-mono` | `"Geist Mono", "SFMono-Regular", Consolas, monospace` | exact strings, logs, code-like content |
| `font-size-body-xs` | `12px` | metadata, compact labels |
| `font-size-body-sm` | `13px` | dense tables, chips, helper text |
| `font-size-body-md` | `14px` | default body and form text |
| `font-size-body-lg` | `16px` | larger body, high-importance summary text |
| `font-size-heading-sm` | `20px` | card titles and section headers |
| `font-size-heading-md` | `24px` | page subsection headings |
| `font-size-heading-lg` | `32px` | page titles |
| `font-size-heading-xl` | `40px` | hero or landing statements |
| `font-size-mono-sm` | `12px` | compact mono metadata |
| `font-size-mono-md` | `13px` | code blocks, logs, technical body text |
| `font-weight-regular` | `400` | default body copy |
| `font-weight-medium` | `500` | labels, controls, compact emphasis |
| `font-weight-semibold` | `600` | section headings and key values |
| `font-weight-bold` | `700` | rare high-emphasis headings |
| `line-height-tight` | `1.2` | titles and compact headings |
| `line-height-default` | `1.45` | default body text |
| `line-height-relaxed` | `1.6` | long instructions or prose blocks |

## Shadow Tokens

| Token | Value | Role |
| --- | --- | --- |
| `shadow-xs` | `0 1px 2px rgba(17, 24, 39, 0.04)` | micro lift on controls |
| `shadow-sm` | `0 6px 18px rgba(17, 24, 39, 0.06)` | cards and anchored menus |
| `shadow-md` | `0 12px 30px rgba(17, 24, 39, 0.10)` | popovers and floating inspectors |
| `shadow-lg` | `0 24px 60px rgba(17, 24, 39, 0.12)` | large modals and emphasized overlays |
| `shadow-overlay` | `0 30px 80px rgba(17, 24, 39, 0.18)` | full overlay surfaces |

## Layer Tokens

| Token | Value | Role |
| --- | --- | --- |
| `layer-base` | `0` | page and app shell |
| `layer-sticky` | `10` | sticky bars and floating toolbars |
| `layer-panel` | `20` | drawers and inspectors |
| `layer-popover` | `30` | menus, tooltips, anchored popovers |
| `layer-modal` | `40` | dialogs and modal sheets |
| `layer-toast` | `50` | toast and transient global notices |

## Motion Tokens

| Token | Value | Role |
| --- | --- | --- |
| `motion-duration-fast` | `120ms` | hover, focus, pressed transitions |
| `motion-duration-base` | `180ms` | menus, popovers, selection transitions |
| `motion-duration-slow` | `240ms` | modal and larger surface transitions |
| `motion-ease-standard` | `cubic-bezier(0.2, 0.8, 0.2, 1)` | most UI transitions |
| `motion-ease-emphasized` | `cubic-bezier(0.2, 0.9, 0.2, 1)` | larger but still quiet transitions |

Transitions should feel quick and low-friction, core review surfaces should not
animate excessively, and all future implementations should respect
reduced-motion preferences.
