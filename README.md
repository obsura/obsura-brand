# Obsura Brand

Obsura Brand is the canonical brand repository for the Obsura project.

It is the source of truth for brand assets, brand documentation, naming rules,
logo usage guidance, verbal identity, and reusable copy for future Obsura
repositories and public surfaces.

> Status: canonical brand source of truth. This repository is intended to be
> referenced by future repositories rather than redefined inside them.

## Relationship To `obsura-standards`

[`obsura-standards`](https://github.com/obsura/obsura-standards) is the
authoritative source for project-wide standards, architecture direction,
governance, and cross-repository naming.

This repository is the operational brand layer that turns that direction into:

- official brand spelling and naming rules
- practical usage guidance for logos and marks
- verbal identity and copy guidance
- an approved visual system, design foundations, and reference UI tokens
- repo descriptions and tagline options
- shared asset organization for downstream reuse

This repository should stay focused on brand concerns. Do not duplicate broad
project standards here unless they directly affect brand usage.

## What Lives Here

- Official brand documentation in [`docs/`](docs/)
- Official asset structure in [`assets/`](assets/)
- Reference UI samples used to freeze the current visual system
- Brand usage guidance for repos, docs, social, and product surfaces
- Design foundations, UI principles, and approved reference tokens for future
  product surfaces
- Repo descriptions and reusable copy for the wider Obsura ecosystem
- Contribution workflows for brand and asset changes

## What Does Not Live Here

- Product implementation code
- Application runtime assets that only exist for one repo or release
- Broad project governance, architecture, or engineering policy
- Marketing filler or speculative brand systems

## Repository Map

| Path | Purpose |
| --- | --- |
| [`docs/index.md`](docs/index.md) | Brand document index |
| [`docs/brand-overview.md`](docs/brand-overview.md) | Brand essence, personality, and intended perception |
| [`docs/brand-principles.md`](docs/brand-principles.md) | Practical principles that constrain future brand work |
| [`docs/verbal-identity.md`](docs/verbal-identity.md) | Preferred wording, avoided terms, and product language |
| [`docs/tone-of-voice.md`](docs/tone-of-voice.md) | Voice rules and context-specific writing examples |
| [`docs/messaging.md`](docs/messaging.md) | Official descriptions, positioning, and message pillars |
| [`docs/taglines.md`](docs/taglines.md) | Optional tagline guidance |
| [`docs/repo-descriptions.md`](docs/repo-descriptions.md) | Official GitHub and README descriptions for Obsura repos |
| [`docs/naming.md`](docs/naming.md) | Product, repo, and asset naming rules |
| [`docs/logo-usage.md`](docs/logo-usage.md) | Logo, mark, icon, and background usage guidance |
| [`docs/brand-system-freeze.md`](docs/brand-system-freeze.md) | Approved extraction of the current Obsura visual system from the sample UI reference set |
| [`docs/visual-direction.md`](docs/visual-direction.md) | Approved visual character and direction |
| [`docs/design-foundations.md`](docs/design-foundations.md) | UI-facing visual foundations for color, typography, spacing, surfaces, and shape language |
| [`docs/design-tokens.md`](docs/design-tokens.md) | Approved reference tokens that future repos can translate into CSS variables or Tailwind config |
| [`docs/ui-principles.md`](docs/ui-principles.md) | Product UI principles for review-first, high-trust workflows |
| [`docs/component-guidelines.md`](docs/component-guidelines.md) | Design expectations for major UI component families before implementation exists |
| [`docs/interaction-principles.md`](docs/interaction-principles.md) | Interaction guidance for selection, clipboard flows, confirmations, undo, and feedback |
| [`docs/asset-organization.md`](docs/asset-organization.md) | Source-of-truth rules for asset storage and downstream reuse |
| [`docs/social-and-profile-usage.md`](docs/social-and-profile-usage.md) | GitHub, social, and profile usage guidance |
| [`docs/website-and-product-copy.md`](docs/website-and-product-copy.md) | Hero copy, blurbs, CTAs, and product copy guidance |
| [`assets/README.md`](assets/README.md) | Asset tree overview and operational asset rules |
| [`assets/samples_ui_ux/README.md`](assets/samples_ui_ux/README.md) | Rules for the sample UI references that informed the frozen brand system |
| [`assets/manifest.json`](assets/manifest.json) | Machine-readable asset inventory |

## Asset Structure

Official assets belong under [`assets/`](assets/).

- Full logo and mark source files should live in `assets/logo/svg/`
- Approved PNG exports of those files should live in `assets/logo/png/`
- Current checked-in icon exports live in `assets/icons/monochrome/black/`
- Preview and profile exports belong under `assets/previews/`
- Reference-only design samples live under `assets/samples_ui_ux/` and must not
  be treated as official Obsura artwork

This repository does not invent missing logo lockups. It provides the canonical
structure and naming so the founder's real files can be added immediately.

## Design Guidance Boundary

This repository defines what Obsura should look like, sound like, and feel like
across brand and product surfaces.

It can document:

- design foundations
- approved reference tokens
- component expectations
- interaction principles

It should not hold:

- framework components
- Tailwind configuration
- app CSS
- implementation-specific UI code

## How Other Repositories Should Use This Repo

- Treat this repository as the source of truth for official brand files and
  wording.
- Copy optimized runtime assets into a consuming repository only when that repo
  needs local delivery files such as `public/brand/` assets.
- Make changes to official logos, marks, previews, or naming here first.
- Update downstream copies only after the canonical change lands here.

Examples:

- `obsura-web` may copy approved runtime assets into `public/brand/`
- `obsura-docs` may reuse approved logos and social previews
- `obsura-windows` may consume approved app icon exports
- future repos should reuse official descriptions from `docs/repo-descriptions.md`

## Contributing

Read [`CONTRIBUTING.md`](CONTRIBUTING.md) before proposing brand, asset, or copy
changes.

- Use the issue templates for brand or asset requests
- Keep changes scoped and update related docs together
- Avoid duplicate exports, duplicate naming schemes, and unofficial logo edits

## License And Brand Use

This repository uses a practical brand-focused licensing posture rather than a
code-only default.

- Repository contents are currently published under the terms in
  [`LICENSE`](LICENSE)
- Trademark and official brand usage are described in
  [`TRADEMARKS.md`](TRADEMARKS.md)
- Project-level legal direction remains documented in
  `obsura-standards/docs/legal/`
