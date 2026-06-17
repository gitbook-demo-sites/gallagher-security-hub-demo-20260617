---
description: "Technology partner SDK onboarding."
icon: code
if: 'visitor.claims.unsigned.persona === "technology_partner" || visitor.claims.unsigned.persona === "cp_plus_tech" || visitor.claims.unsigned.persona === "staff"'
---

# SDK onboarding

This dummy page represents Technology Partner content for integrations, SDKs, and sandbox access.

## Onboarding flow

{% stepper %}
{% step %}
### Request sandbox access

Submit the integration use case, region, expected customer flow, and callback endpoints.
{% endstep %}

{% step %}
### Build against sample events

Use SDK examples to validate authentication, event handling, and error states.
{% endstep %}

{% step %}
### Complete security review

Confirm data handling, customer consent, and deployment boundaries before production approval.
{% endstep %}
{% endstepper %}

{% if visitor.claims.unsigned.persona === "cp_plus_tech" %}
## Channel relationship detected

Because this visitor also has Channel Partner access, commercial handoff notes and integration support paths can be shown in the same journey.
{% endif %}

