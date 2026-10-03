# Privacy Policy — Visual Mermaid for Confluence

Last updated: 2026-09-15

## The short version

This app collects nothing. It makes no network requests outside Atlassian's own infrastructure.
There is nothing for this privacy policy to disclose beyond that.

## What the app does with your data

Visual Mermaid stores a diagram's source text inside the Confluence macro's own configuration,
which lives inside the page it's placed on. That configuration is Confluence page data — it is
stored, backed up, and access-controlled by Atlassian exactly like the rest of the page, and it
moves with the page (copy, export, history, deletion) because it never leaves it.

The app does **not**:

- make any request to a server outside Atlassian's infrastructure (no `permissions.external`
  block exists in the app's manifest, and CI fails the build if one is ever added)
- use analytics, telemetry, crash reporting, or any third-party SDK
- require or create a user account of any kind
- store data in any location other than the Confluence page the diagram is on
- share data with any subprocessor, because there is no subprocessor

## Permissions this app requests, and why

| Scope                   | Purpose                                                                                                                                        |
| ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| `read:page:confluence`  | To find the Mermaid code block a macro is bound to.                                                                                            |
| `write:page:confluence` | Used only by the **Render all Mermaid code blocks** action, only when a user runs it, and only after it shows what it will change on the page. |

Neither scope is used to read or write anything outside the page a user is actively viewing or
acting on.

## Data residency

Because nothing is stored outside Confluence, data residency for anything this app touches is
whatever your Atlassian organization has already configured for Confluence itself.

## Hosting

The app runs entirely on Atlassian's Forge platform — Atlassian's own compute, not a
vendor-operated server. This is also the basis for its _Runs on Atlassian_ eligibility.

## Changes to this policy

If this app ever starts making an external request of any kind, that will be a listed, reviewable
change to the app's permissions (Atlassian requires re-approval for scope changes), and this
policy will be updated before that version ships.

## Contact

Questions about this policy: niv@schneiderman.tech
