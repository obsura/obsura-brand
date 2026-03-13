# Asset Organization

This document explains how official Obsura brand assets are organized and how
other repositories should consume them.

See also: [Logo Usage](logo-usage.md), [Naming](naming.md)

## Why The Asset Tree Is Structured This Way

The structure separates:

- canonical logo and mark files
- runtime-friendly icon exports
- surface-specific preview assets
- reference-only design inputs
- machine-readable asset metadata

This keeps the source of truth explicit without forcing every downstream repo to
store the same files in the same way.

## Source Of Truth Rules

- `obsura-brand` is the canonical home for official brand assets
- official changes happen here first
- downstream repos may copy approved exports, but should not redefine them
- `assets/manifest.json` should reflect the current official inventory

## Asset Status Model

Use the shared status model in `assets/manifest.json` to reduce confusion:

- `draft`: planned or exploratory
- `provisional`: usable direction, still open to refinement
- `approved`: canonical and ready for reuse
- `deprecated`: retained for compatibility, not for new adoption

Apply status to asset families and individual exports where useful.

## Current Asset Layout

| Path | Purpose |
| --- | --- |
| `assets/logo/svg/` | Canonical SVG logo and mark files |
| `assets/logo/png/` | Approved PNG exports of canonical logos and marks |
| `assets/icons/monochrome/black/` | Current transparent black mark exports |
| `assets/icons/favicon/` | Reserved for approved favicon bundles if needed later |
| `assets/icons/app/` | Reserved for approved app icon packages if needed later |
| `assets/icons/social/` | Reserved for platform-specific social icon exports |
| `assets/previews/github/` | GitHub avatar and social preview exports |
| `assets/previews/product/` | Product-adjacent preview compositions |
| `assets/previews/website/` | Website share cards and hero preview assets |
| `assets/samples_ui_ux/` | Reference-only UI sample set used to freeze the current brand system |

## Adding New Exports

When adding an official export:

1. start from the canonical source asset
2. use the naming rules from [Naming](naming.md)
3. place the file in the correct directory
4. update `assets/manifest.json`
5. update usage documentation if the new asset changes guidance

## What Belongs Here Versus In Product Repositories

Belongs here:

- official logos and marks
- approved PNG or SVG exports meant for reuse across repos
- GitHub or website preview assets used across the project
- reference-only sample inputs that directly inform brand documentation
- canonical naming and usage documentation

Belongs in product repositories:

- app-specific runtime copies such as `public/brand/`
- release-specific screenshots
- repo-local marketing graphics that are not official reusable assets
- build artifacts generated only for one deployment target

Reference-only samples should stay here only when they are serving brand-system
analysis. They are not downstream runtime assets.

## Downstream Consumption Guidance

Downstream repositories should:

- copy only the assets they actually need
- preserve canonical file names when practical
- reference this repository in pull requests when an official asset changes
- avoid editing copied assets in place unless the change is also made here

If a new official variant is needed for `obsura-web`, `obsura-docs`,
`obsura-windows`, or any future repo, add it here first and then copy it
downstream.
