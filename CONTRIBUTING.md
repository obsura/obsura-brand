# Contributing To Obsura Brand

This repository exists to keep Obsura's brand assets and brand guidance
practical, consistent, and reusable across the project.

Before changing anything here, read the relevant document in [`docs/`](docs/)
and check the related standards direction in `obsura-standards` when needed.

## What Belongs Here

Good contributions to this repository include:

- clarifying naming, messaging, or usage guidance
- adding official brand assets or approved exports
- tightening copy used across repositories or public surfaces
- fixing contradictions, duplicate guidance, or unclear asset structure
- improving asset metadata and organizational hygiene

This is not the place for product implementation work or repo-specific runtime
assets that only matter to one application.

## How To Propose Changes

- Small wording or structure fixes can be opened directly in a pull request.
- Brand direction, naming, or messaging changes should start with a `brand
  request` issue when they affect multiple documents.
- New asset exports, logo variants, or preview files should start with an
  `asset request` issue when the need is not already agreed.
- Copy updates for repository descriptions, hero text, taglines, or bios can
  use the `brand request` path unless they are tiny direct fixes.

Use the issue templates in [`.github/ISSUE_TEMPLATE/`](.github/ISSUE_TEMPLATE/).

## Brand Change Rules

- Keep the official product name as `Obsura`
- Keep repository names aligned with the `obsura-` naming system unless
  `obsura-standards` explicitly documents an exception
- Prefer concrete product language over slogans
- Do not invent new brand themes that conflict with the restrained, technical,
  review-first direction

## Asset Change Rules

- Add official source files to the canonical location first
- Do not create duplicate exports with slightly different names
- Do not commit files named like `final-final-v2` or other ambiguous variants
- Update [`assets/manifest.json`](assets/manifest.json) when new official assets
  are added
- If a downstream repo needs a new official variant, add it here before copying
  it downstream

## Copy Change Rules

- Keep wording clear, exact, and calm
- Avoid hype, legal theater, and vague security claims
- Mark future direction clearly instead of implying shipped capability
- Update related descriptions, taglines, or wording guidance together when they
  overlap

## Pull Request Expectations

Each pull request should:

- explain the problem being solved
- describe the practical outcome
- update all affected docs and asset references
- stay focused on one coherent brand problem
- avoid speculative or decorative additions with no operational use

## Commit And Branch Naming

Use short, descriptive names.

Examples:

- `brand/repo-description-refresh`
- `assets/add-light-mark-exports`
- `docs/logo-usage-clarity`
- `copy/hero-text-update`

Prefer imperative commit subjects such as:

- `docs: tighten tagline guidance`
- `assets: add github preview export`
- `brand: align repo descriptions with standards`

## License

By contributing, you agree that your contributions will be licensed under this
repository's license and subject to its provisional trademark note unless a
later policy states otherwise.
