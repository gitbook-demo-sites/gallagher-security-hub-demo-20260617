---
description: "Public security advisory pattern with adaptive partner detail."
icon: triangle-exclamation
---

# Security advisories

Security advisories should be public by default when the public needs awareness, with restricted implementation detail shown only to trusted audiences.

## Public advisory template

| Field | Example |
| --- | --- |
| Advisory ID | GSEC-2026-001 |
| Affected products | Command Centre Web demo component |
| Severity | Medium |
| Public action | Upgrade to the latest supported release |

{% if visitor.claims.unsigned.persona === "channel_partner" || visitor.claims.unsigned.persona === "high_security_partner" || visitor.claims.unsigned.persona === "cp_plus_tech" || visitor.claims.unsigned.persona === "staff" %}
## Partner remediation details

- Customer communication template.
- Patch verification checklist.
- Escalation path for complex estates.
{% endif %}

{% if visitor.claims.unsigned.persona === "high_security_partner" || visitor.claims.unsigned.persona === "staff" %}
## High security handling

Coordinate the customer notification timeline with Gallagher before sharing deployment-specific mitigations.
{% endif %}

