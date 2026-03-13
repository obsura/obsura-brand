# Design Foundations

> Status: approved brand-system guidance for future implementation
> repositories.

This document defines the visual foundations of Obsura at the design level. It
sets direction for future product work without prescribing implementation code.

See also: [Brand System Freeze](brand-system-freeze.md),
[Visual Direction](visual-direction.md), [Design Tokens](design-tokens.md),
[UI Principles](ui-principles.md)

## Purpose

Obsura should feel like a clean operational workbench for reviewing and
redacting sensitive technical content under real time pressure. The UI should
feel stable, readable, and deliberate before it feels expressive.

## Visual Model

Obsura should combine:

- a light shell
- white elevated working surfaces
- precise data structure
- calm accent restraint
- dark review zones only where the task benefits from them

## Color System

Use a neutral-light foundation with one primary action color and soft semantic
support tones.

| Role | Reference | Usage |
| --- | --- | --- |
| App shell | `#F5F3F0` | outer workspace background, docs framing, empty-state backdrop |
| Canvas | `#FCFBF9` | main page background and broad content field |
| Muted surface | `#F3F1EE` | segmented rails, grouped controls, muted cards |
| Elevated surface | `#FFFFFF` | cards, menus, dialogs, inspectors, sheets |
| Border | `#E2DDD8` | default separators and control outlines |
| Primary text | `#171717` | headings, labels, and critical values |
| Secondary text | `#4B4B4B` | supporting body text and metadata |
| Tertiary text | `#7C7772` | muted labels, helper text, inactive context |
| Primary accent | `#5B4CE3` | primary buttons, active tabs, focus-led actions |
| Accent soft | `#E9E5FF` | selected rows, soft badges, focus-adjacent fills |
| Ice support | `#DDF3FF` | detected highlights, informational emphasis, secondary status surfaces |
| Success | `#7FD698` | safe, approved, completed, healthy states |
| Warning | `#E8A63C` | caution, review-needed, pending states |
| Danger | `#E57F73` | destructive actions and risk states |

Obsura should not look neon, black-box-heavy, threat-themed, or gradient-led.

## Typography System

Typography should optimize for technical clarity, compact scanning, and calm
confidence.

Preferred families:

- interface sans: `Geist` or a similar neutral grotesk
- technical mono: `Geist Mono` or a similar compact monospace

Guidance:

- use medium-weight body and label text more often than ultra-light typography
- keep headings clean, short, and confidently sized
- preserve readable sizing for dense tables, inspectors, and chips
- use monospace for file paths, code-like values, logs, OCR output, and other
  exact strings
- avoid ornamental display faces or personality-led headline fonts

## Shape Language

Obsura should feel exact, but not sharp-edged or severe.

Guidance:

- favor rectangles, rounded rectangles, and pill controls
- keep default radii in the 12px to 16px range for controls and menus
- reserve 20px to 24px radii for cards, shells, and larger containers
- avoid bubbly, cartoon, or overly geometric hard-edge extremes

## Spacing Model

Spacing should signal order and speed.

Guidance:

- use a 4px base scale
- let 12px and 16px dominate control and card padding
- use 24px and 32px for section boundaries and larger shell spacing
- keep dense technical views readable without becoming airy for its own sake
- avoid dramatic whitespace that wastes room in operational workflows

Obsura is a workbench, not a brochure.

## Border And Elevation Model

Elevation should clarify layers, not create spectacle.

Guidance:

- use 1px low-contrast borders almost everywhere
- pair borders with shallow ambient shadows for floating surfaces
- keep modals, menus, and inspectors visibly distinct without looking detached
- prefer contrast, borders, and layering discipline over dramatic blur

## Icon Style Direction

Icons should feel technical, minimal, and readable.

Guidance:

- favor simple geometric silhouettes
- keep line weight consistent inside a given surface
- prefer outline icons for product controls and navigation
- reserve filled icons for marks, app tiles, or clearly intentional emphasis
- use icons to reinforce actions and states, not to carry full meaning alone

## Surface And Background System

Obsura should use a light layered surface model.

Recommended layers:

- app shell on paper or mist neutrals
- primary work surfaces on white
- muted rails and grouped controls on a slightly darker neutral
- floating overlays on white with border plus shadow
- focused dark review surfaces only when content contrast demands them

## Dark Surface Strategy

Obsura should be light-mode-default and dark-mode-supported.

That means:

- the main brand identity should live on light surfaces
- dark surfaces are allowed for image review, comparison, and dense text
  inspection when they improve readability
- dark mode should not turn the product into a different visual language
- contrast rules should stay equally rigorous in both directions

## Motion And Feedback

Motion should feel short, quiet, and physical.

Guidance:

- use brief fades, lifts, and anchored expansions
- keep motion strongest on menus, tooltips, popovers, and state confirmation
- avoid long travel distances and ornamental choreography
- respect reduced-motion preferences in future implementations

## Product Feel

In product UI, Obsura should feel:

- fast
- calm
- exact
- clean
- safe to operate
- readable under pressure
- polished without looking flashy

If a design choice makes the product look more exciting but less trustworthy,
choose the calmer option.
