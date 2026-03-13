# Component Guidelines

> Status: approved non-code component guidance grounded in the current brand
> system freeze.

This document defines design expectations for key component families in Obsura.
It does not define implementation code.

See also: [Brand System Freeze](brand-system-freeze.md),
[UI Principles](ui-principles.md),
[Interaction Principles](interaction-principles.md),
[Design Tokens](design-tokens.md)

## Shared Component Traits

All components should:

- prioritize legibility over decoration
- use white or soft-tint surfaces on a light shell
- keep radii mostly between 12px and 16px
- use 1px low-contrast borders before stronger fills
- rely on one clear accent color for active emphasis
- communicate state clearly
- support keyboard focus visibly
- behave consistently across dense technical workflows
- avoid looking soft, toy-like, or excessively marketing-driven

## Buttons

### Primary Button

Use for the main action in a local context, such as export, confirm, or apply.

Expectations:

- filled with the primary periwinkle accent
- white label text with medium or semibold weight
- 40px to 44px height in most contexts
- 12px radius by default
- clearly dominant without glowing or shouting
- stable hover, focus, active, disabled, and loading states
- should feel safe, not aggressive

### Secondary Button

Use for important but non-primary actions such as preview, review, or open
settings.

Expectations:

- white surface with default border and dark text
- visually subordinate to primary
- strong enough to remain readable on light shells and tinted rails

### Ghost Button

Use for low-emphasis actions inside dense toolbars or inspectors.

Expectations:

- minimal base weight
- transparent or lightly tinted base
- stronger visible feedback on hover and focus
- should never disappear into the background

### Destructive Button

Use for discard, remove, reset, or irreversible cleanup actions.

Expectations:

- distinct semantic styling
- prefer muted danger surfaces for most contexts
- reserve solid danger fills for true point-of-no-return actions
- must not be confused with primary confirmation
- disabled and loading states should remain obvious

## Inputs

### Text Input

Use for filenames, labels, replacement values, and compact structured entry.

Expectations:

- white surface
- 44px default height unless density demands smaller
- 12px radius with 1px border
- strong text readability
- clear placeholder hierarchy
- obvious error, focus, and disabled states

### Search Input

Use for pack search, entity filtering, or finding content in technical text.

Expectations:

- fast, lightweight visual treatment
- leading search icon and optional trailing shortcut chip
- clear active and empty states
- supports keyboard-first flow

### Textarea

Use for longer freeform or semi-structured content entry.

Expectations:

- readable line height
- sensible padding
- clear overflow and resize behavior

### Code Or Text Block Editor

Use for logs, configs, pasted text, or technical body content.

Expectations:

- monospace typography
- high readability under dense content
- selection, highlight, and redaction states must remain easy to parse

### Command Or Composer Input

Use for quick actions, paste-first entry, and AI-assisted prompts that stay
secondary to the main workflow.

Expectations:

- large rounded shell with calm border treatment
- inline mode chips, tool buttons, or shortcut hints can live inside the shell
- should feel like an entry point, not a chat app takeover

## Navigation And Selection

### Tabs And Segmented Controls

Use for compact mode switches, filtered views, and local content grouping.

Expectations:

- sit on a muted rail or grouped surface
- active segment may use white or accent-soft fill
- labels stay short and highly scannable

### Sidebar Item

Use in product navigation, workflow lists, and supporting app sections.

Expectations:

- icon-left, label-right layout
- active state should use subtle fill, not heavy blocks
- repeated items must stay readable in long lists

### Data Row Or Table Row

Use for detections, files, packs, entities, audit events, and result lists.

Expectations:

- strong scanability across repeated rows
- calm separators rather than heavy gridlines
- selected state should use a soft fill and clear outline or accent marker
- avatars, status dots, badges, and timestamps should not break alignment

## Menus, Popovers, And Overlays

### Context Menu

Use for row actions, selection actions, and compact management flows.

Expectations:

- white floating surface with 12px to 16px radius
- left-aligned icons and optional right-aligned shortcuts
- hovered row uses muted surface fill, not saturated highlight
- enough width for clear labels without becoming oversized

### Popover Or Inspector Card

Use for anchored detail views, settings, and in-place review tools.

Expectations:

- white surface, subtle border, medium shadow
- clear section grouping and header hierarchy
- anchored placement that preserves context with the source selection

### Modal Or Sheet

Use for multi-step confirmations, larger edit flows, or export decisions.

Expectations:

- elevated white surface over a restrained scrim
- large enough to hold structured decisions without feeling like a blank page
- only one dominant primary action per modal
- destructive and confirm actions must remain visually distinct

## Review Elements

### Detected Entity Chip

Use to summarize detected entity types or matched values.

Expectations:

- compact and scannable
- color should reinforce category or state, not replace readable labeling
- use soft ice or soft lavender fills by default
- long values should truncate predictably when necessary

### Confidence Badge

Use when model or recognizer confidence is relevant to review.

Expectations:

- should provide signal without creating false certainty
- low, medium, and high states must remain distinguishable
- never use confidence styling as the only explanation of risk

### Replacement Badge

Use to indicate the replacement strategy or redaction style being applied.

Expectations:

- easy to compare across entities
- readable in lists, panels, and review cards

### Status Label

Use for workflow states such as detected, reviewed, ignored, exported, failed,
or pending.

Expectations:

- semantic color plus readable text
- should remain legible in dense layouts

## Layout Components

### App Shell

Role:

holds the global frame for navigation, main work area, and supporting panels

Expectations:

- mist or paper shell background
- white primary work surfaces
- clear separation between shell chrome and content surfaces
- should feel stable, not skeletal

### Top Bar

Role:

holds global navigation, file context, and top-level actions

Expectations:

- compact
- stable across pages or workspaces
- should not dominate the review canvas
- may include search or quick-action entry when useful

### Side Panel

Role:

holds filters, lists, packs, or supporting navigation

Expectations:

- dense but readable
- easy scanning of repeated items
- supports collapse or width discipline where useful

### Inspector Panel

Role:

shows details for the current selection, rule, or detected item

Expectations:

- clear sectioning
- visible relationship to selected content
- should support rapid compare-and-adjust flows

### Toolbar

Role:

holds direct manipulation actions for review and editing

Expectations:

- actions grouped by intent
- strong icon-plus-label clarity where needed
- no cluttered wall of low-value controls
- floating variants should feel light and contextual

### Action Footer

Role:

anchors workflow progression, confirmation, or export steps

Expectations:

- high clarity for next-step actions
- should feel stable and trustworthy

### Card

Role:

holds grouped metrics, list summaries, settings clusters, or workflow snapshots

Expectations:

- white or soft-tint surface
- 16px to 20px radius
- header, body, and footer divisions should stay subtle
- should work equally well in dashboard and utility contexts

### File Dropzone

Role:

supports upload, paste, and drag-and-drop entry points

Expectations:

- obvious affordance without oversized marketing treatment
- should feel like a serious workspace entry point
- drag-active state must be clear

## Specialized Product Components

### Redaction Region Overlay

Use for visual masking or replacement on images and screenshots.

Expectations:

- boundaries remain precise
- handles and selection states should be easy to target
- active editable state should use a periwinkle outline
- final redacted state should use a dark charcoal fill
- overlay styling must not hide whether the content has been reviewed

### Image Review Canvas

Use as the main surface for screenshot and image review.

Expectations:

- content remains central
- zoom, pan, and selection controls should not overwhelm the canvas
- overlays, guides, and states need strong contrast discipline
- may use a dark surface when the image content benefits from it

### Text Highlight Span

Use to mark detected or selected text ranges.

Expectations:

- preserve text readability
- distinguish selected, hovered, detected, and redacted states clearly
- support dense technical text without visual chaos

### Rule Card

Use to represent recognizers, replacement rules, or workflow rules.

Expectations:

- clear summary of trigger, scope, and effect
- supports enabled, disabled, draft, and warning states
- should be easy to scan in lists

### Pack Card

Use to represent reusable recognizer or workflow packs.

Expectations:

- present name, purpose, status, and trust context clearly
- avoid marketplace-style visual noise

### Compare Panel

Use to show original versus redacted output, or before versus after review
states.

Expectations:

- columns or stacked views should align clearly
- differences should be easy to scan without loud diff styling
- the reviewed result should feel more resolved than the source state

### Export Option Card

Use to present export targets or formatting options.

Expectations:

- clear consequence and output description
- obvious selected state
- must communicate risk-relevant differences, not just look selectable

### AI Suggestion Popover

Use for rewriting, replacement suggestions, or review assistance that stays
optional.

Expectations:

- anchored near the current text or selection
- compact and dismissible
- clearly separate suggestion from accepted result
- should never obscure the fact that the user still owns the final decision

## Accessibility Expectations

All future components should support:

- visible keyboard focus
- sufficient contrast
- readable text at practical UI sizes
- semantic labeling beyond color alone
- reduced-motion-aware behavior where motion exists
