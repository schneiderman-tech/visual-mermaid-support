# Support & Service Levels — Visual Mermaid for Confluence

Last updated: 2026-09-15

## Getting help

File a bug report or feature request at: **https://github.com/nivSchneiderman/visual-mermaid-support/issues**

That tracker is monitored and is the single place to check status on an open request.

## Support hours

09:00–17:00 Israel Time (Asia/Jerusalem, UTC+2 / UTC+3 in summer), **Sunday–Thursday**.

That is the standard Israeli working week, and it is five days a week as the Marketplace
requires. Note that it covers Sunday and not Friday — a request sent on a Friday is picked up the
following Sunday. "Business days" below means these days.

## Response targets

| Severity                                   | First response  |
| ------------------------------------------ | --------------- |
| Critical — app unusable, data loss risk    | 24 hours        |
| High — major feature broken, no workaround | 3 business days |
| Normal — minor bug, workaround exists      | 5 business days |
| Low — feature request, cosmetic            | best effort     |

## Emergency contact

24×7 emergency contact for critical issues: **niv@schneiderman.tech**

## Uptime and recovery

Visual Mermaid has no vendor-operated backend. It is a static Forge app: all rendering happens
in the customer's browser, and the only data it touches (diagram source) is stored inside the
Confluence page itself, not on any server this vendor runs.

- **Uptime**: inherited from Atlassian's own Forge platform and Confluence Cloud SLA — there is
  no separate vendor infrastructure that can be down while Confluence is up.
- **RPO (Recovery Point Objective)**: not applicable. The app holds no data of its own; all
  diagram data lives in Confluence page storage and is covered by Atlassian's own backup and
  recovery guarantees for page content.
- **RTO (Recovery Time Objective)**: a broken release is fixed by shipping a corrected version
  through Forge's deployment pipeline, typically within hours of a confirmed critical bug.

## Versioning and end of life

As long as any customer has an active paid subscription, this app will continue to be maintained
and will not be withdrawn from the Marketplace. Any scope or pricing change that requires
re-approval will be announced with reasonable notice before it takes effect.

## Contact

General support: niv@schneiderman.tech
