# Interaction Principles

> Status: provisional workflow and behavior guidance.

This document defines how Obsura should handle key interactions in future
product repositories.

See also: [UI Principles](ui-principles.md),
[Component Guidelines](component-guidelines.md)

## Selection Behavior

Selection should feel precise and reversible.

Guidance:

- selected content must be visually obvious
- selection state should remain stable while related panels update
- multiple selection modes should not conflict silently
- users should always understand what the current action target is

## Hover And Focus Expectations

Hover should hint. Focus should confirm.

Guidance:

- hover states should preview interactivity without excessive motion
- keyboard focus must be explicit and reliable
- focus treatment should remain visible on dark and light surfaces
- hover-only affordances should always have a keyboard-accessible equivalent

## Bulk Action Behavior

Bulk actions should save time without hiding consequences.

Guidance:

- show scope before applying the action
- summarize what changed after the action
- make follow-up review easy
- support undo where practical

## Manual Redaction Behavior

Manual redaction is a core trust feature, not a fallback embarrassment.

Guidance:

- manual region creation should feel fast and controlled
- handles, resize behavior, and overlay bounds should be precise
- users should be able to distinguish manual from auto-detected regions if that
  distinction matters to review

## Keyboard-First Support

Obsura should work well for users who move quickly.

Guidance:

- support predictable keyboard navigation
- expose shortcuts for common actions where useful
- keep focus order logical across panels, toolbars, and review surfaces
- avoid trapping power users in mouse-only flows

## Clipboard-First Workflows

Pasting should be a first-class input path for screenshots and text.

Guidance:

- make paste entry obvious on relevant surfaces
- confirm successful paste without interrupting flow
- distinguish between pasted image and pasted text cases clearly

## Confirmation Patterns

Confirmations should exist for risk, not for ceremony.

Guidance:

- ask for confirmation when an action is destructive, irreversible, or easy to
  mis-trigger
- avoid confirmation spam for routine steps
- confirmation dialogs should state the consequence plainly

## Undo And Redo Expectations

Undo and redo support trust because users need to explore safely.

Guidance:

- reversible actions should prefer undo over extra confirmation
- state changes should be grouped sensibly so undo history feels predictable
- users should understand what the last undoable action was

## Export Feedback Patterns

Export is a moment of trust.

Guidance:

- show progress when export is not immediate
- confirm success clearly
- make it obvious what was exported and in which form
- surface failures with useful recovery guidance

## Failure State Behavior

Failures should be calm, specific, and actionable.

Guidance:

- explain what failed
- explain what the user can do next
- avoid blame-heavy or alarmist error language
- preserve as much recoverable work as possible

## OCR And Loading States

Detection, OCR, and heavy processing states should remain understandable.

Guidance:

- show that work is in progress
- indicate which step is running when useful
- keep the interface usable where safe
- avoid vague endless spinners with no context

## Accessibility And Predictability

Interaction behavior should stay predictable across modes.

That means:

- consistent shortcuts and focus behavior
- no critical interaction that depends only on color or animation
- clear state transitions between detect, review, edit, and export steps
