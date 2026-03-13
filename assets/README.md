# Obsura Brand Assets

This directory contains the canonical brand asset tree for Obsura.

Current checked-in assets are transparent black icon exports in
`icons/monochrome/black/`. The repository structure is also prepared for the
founder's full logo and mark files to be added without inventing placeholder
graphics.

See also:

- [`../docs/logo-usage.md`](../docs/logo-usage.md)
- [`../docs/asset-organization.md`](../docs/asset-organization.md)
- [`../docs/naming.md`](../docs/naming.md)

## Structure

| Path | Purpose |
| --- | --- |
| `logo/svg/` | Canonical SVG logo and mark files |
| `logo/png/` | Approved PNG exports of official logos and marks |
| `icons/monochrome/black/` | Current transparent black icon exports |
| `icons/favicon/` | Reserved for curated favicon bundles |
| `icons/app/` | Reserved for curated app icon packages |
| `icons/social/` | Reserved for social or avatar-specific icon exports |
| `previews/github/` | GitHub avatar and social preview assets |
| `previews/product/` | Product-adjacent preview assets |
| `previews/website/` | Website-specific preview assets |
| `samples_ui_ux/` | Reference-only UI samples used to extract the current Obsura visual system |

## Source Of Truth Rules

- Add official assets here first
- Keep canonical file names stable and descriptive
- Do not create duplicate exports with slightly different names
- Update `manifest.json` when new official assets are added
- Keep each asset or asset family marked with the correct status:
  `draft`, `provisional`, `approved`, or `deprecated`
- Let downstream repos copy approved exports rather than redefining them

Reference-only samples are the exception to the export rule:

- keep them clearly marked as reference-only
- do not publish them as Obsura brand assets
- do not treat them as product screenshots

## Current Official Exports

- `icons/monochrome/black/obsura-icon-16.png`
- `icons/monochrome/black/obsura-icon-32.png`
- `icons/monochrome/black/obsura-icon-57.png`
- `icons/monochrome/black/obsura-icon-60.png`
- `icons/monochrome/black/obsura-icon-70.png`
- `icons/monochrome/black/obsura-icon-72.png`
- `icons/monochrome/black/obsura-icon-76.png`
- `icons/monochrome/black/obsura-icon-96.png`

## Current Reference Inputs

- `samples_ui_ux/`

See [`samples_ui_ux/README.md`](samples_ui_ux/README.md) for handling rules.

## Planned Canonical Logo Names

When the official logo and mark files are added, use names such as:

- `obsura-logo-primary.svg`
- `obsura-logo-dark.svg`
- `obsura-logo-light.svg`
- `obsura-mark.svg`
- `obsura-mark-dark.svg`
- `obsura-mark-light.svg`
