---
description: "Ownership and review model for the migrated Security Hub."
icon: list-check
if: 'visitor.claims.unsigned.persona === "staff"'
---

# Content governance

## Suggested review owners

| Content category | Owner | Review cadence |
| --- | --- | --- |
| Public product docs | Product documentation | Quarterly |
| Security advisories | Product security | As needed |
| Channel commercial | Partner enablement | Monthly |
| High security | High security program owner | Before each release |
| Technology partner SDKs | Developer relations | Per API release |

## Publishing controls

- Use Git Sync pull requests for large migrations.
- Use GitBook change requests for page-level review.
- Require security review before publishing sensitive partner-only content.
- Keep old MindTouch IDs in metadata during the migration window.

