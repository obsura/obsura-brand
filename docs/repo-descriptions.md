# Repo Descriptions

This document provides the official description set for current and likely
Obsura repositories.

See also: [Naming](naming.md), [Messaging](messaging.md)

## Naming Note

The current standards baseline favors a split repository strategy such as
`obsura-web`, `obsura-api`, and `obsura-engine`.

If a top-level `obsura` repository is used later, treat it as a deliberate
exception and align it with `obsura-standards` first.

## Official Descriptions

| Repository | GitHub Description | README Intro |
| --- | --- | --- |
| `obsura-standards` | Cross-project standards, governance, and shared direction for Obsura. | This repository defines the product direction, architecture guidance, governance model, documentation rules, and shared terminology for Obsura. |
| `obsura-brand` | Brand assets, logo exports, visual references, and reusable copy guidance for Obsura. | This repository is the source of truth for Obsura's brand assets, naming rules, usage guidance, and reusable project copy. |
| `obsura-web` | Main web application for review-first redaction workflows in Obsura. | This repository contains the main Obsura web application for detecting, reviewing, styling, and exporting redacted content. |
| `obsura-api` | Backend services, job orchestration, and integrations for Obsura. | This repository contains the backend services and orchestration layer that support Obsura workflows and integrations. |
| `obsura-engine` | Shared detection, redaction, styling, and export logic for Obsura. | This repository contains the reusable processing logic that powers detection, redaction, replacement, and export across Obsura surfaces. |
| `obsura-docs` | End-user and operator documentation for Obsura. | This repository contains practical guides, setup instructions, and usage documentation for Obsura users and operators. |
| `obsura-packs` | Reusable recognizers, styles, templates, and workflow packs for Obsura. | This repository contains reusable packs that extend Obsura with recognizers, redaction styles, templates, and workflow defaults. |
| `obsura-windows` | Windows companion app and OS-level workflow support for Obsura. | This repository contains Windows-specific integrations such as hotkeys, tray behavior, and handoff flows for Obsura. |
| `obsura` | Reserved for a flagship product repository if the repo strategy changes later. | If this repository name is adopted later, it should describe the primary Obsura product surface without conflicting with the split-repo standards baseline. |

## Description Rule

Prefer descriptions that identify responsibility directly. Avoid clever taglines
in repository descriptions.
