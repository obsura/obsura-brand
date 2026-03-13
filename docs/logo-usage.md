# Logo Usage

This document explains how to use official Obsura logos, marks, and icon
exports.

See also: [Naming](naming.md), [Asset Organization](asset-organization.md),
[Social And Profile Usage](social-and-profile-usage.md)

## Asset Classes

Obsura uses three practical classes of brand asset:

### Full Logo

The full logo is the main identification asset for README headers, docs
mastheads, website hero sections, and other surfaces where the product name
should be visible in one unit.

Canonical storage:

- `assets/logo/svg/`
- `assets/logo/png/`

### Mark

The mark is the compact brand symbol for avatars, icons, favicons, app icons,
and tight UI spaces.

Canonical storage:

- `assets/logo/svg/`
- `assets/logo/png/`
- `assets/icons/`

### Icon Exports

Icon exports are runtime-friendly square files for product or platform usage.

Current checked-in assets:

- `assets/icons/monochrome/black/obsura-icon-16.png`
- `assets/icons/monochrome/black/obsura-icon-32.png`
- `assets/icons/monochrome/black/obsura-icon-57.png`
- `assets/icons/monochrome/black/obsura-icon-60.png`
- `assets/icons/monochrome/black/obsura-icon-70.png`
- `assets/icons/monochrome/black/obsura-icon-72.png`
- `assets/icons/monochrome/black/obsura-icon-76.png`
- `assets/icons/monochrome/black/obsura-icon-96.png`

## Variant Guidance

Planned canonical logo and mark variants should use these names when committed:

- `obsura-logo-primary`
- `obsura-logo-dark`
- `obsura-logo-light`
- `obsura-mark`
- `obsura-mark-dark`
- `obsura-mark-light`

This repository currently contains icon exports only. Do not invent missing
logo variants in downstream repositories.

## Background Character

Default branded contexts for Obsura should be:

- white
- paper
- mist
- soft ice support fields when a lighter accent surface helps

Avoid treating pure black, dark gray, or saturated gradients as the default
brand backdrop.

## Mark Framing

When the mark appears in an avatar, app tile, compact product header, or social
preview, prefer a controlled container:

- rounded square or rounded rectangle
- precise internal padding
- white or paper background
- subtle border or shadow when separation is needed

The mark itself should stay crisp and flat. Put atmosphere in the surrounding
surface, not inside the symbol.

## When To Use The Full Logo

Use the full logo when:

- a surface has enough room for the wordmark
- the brand should be immediately recognizable by name
- the asset appears in a README, website header, docs masthead, or launch asset

## When To Use The Mark

Use the mark when:

- the surface is square or tightly constrained
- the brand is already obvious from nearby text
- the asset is used for avatars, favicons, app icons, or compact UI areas

## Dark And Light Versions

- use dark variants on light backgrounds
- use light variants on dark review surfaces or controlled dark backgrounds
- do not recolor exported assets ad hoc in downstream repositories

If a required background-safe variant does not exist yet, add it here first.

## GitHub Avatar Guidance

Use the mark, not the full logo.

The current transparent black icon set may lose contrast on dark UI surfaces
and uncontrolled profile themes. If GitHub or another platform needs a
controlled-background avatar export, add that export under
`assets/previews/github/` or `assets/icons/social/` first.

## Website And App Header Guidance

Use the full logo when the header introduces the product by name.

Use the mark only when the word `Obsura` is already present in the header or
navigation.

## Favicon And App Icon Guidance

Use the smallest suitable icon export from `assets/icons/monochrome/black/`
until approved favicon or app-specific packages are added.

If a downstream app needs a bundled `.ico`, platform manifest set, or larger app
icon sizes, treat those as derived exports and add the official source asset
here first.

## What Not To Do

- do not stretch, crop, or rotate official assets
- do not add glow, gradients, or decorative effects to the mark
- do not default the mark onto hard black surfaces unless the variant is
  designed for that use
- do not place a dark mark on a dark background or a light mark on a light
  background
- do not redraw the logo locally for one repo
- do not create unofficial "temporary" variants outside this repository
