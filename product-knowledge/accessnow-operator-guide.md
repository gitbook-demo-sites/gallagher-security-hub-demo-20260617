---
description: "Daily operator workflows for AccessNow."
icon: mobile-screen-button
---

# AccessNow operator guide

AccessNow gives security teams browser-based access to common operational workflows.

{% stepper %}
{% step %}
### Confirm user permissions

Check that the operator has the right role for the site || region they are supporting.
{% endstep %}

{% step %}
### Search for the person || event

Use the person, credential, || event search depending on the request.
{% endstep %}

{% step %}
### Capture the audit trail

Record the reason for the change and link it back to the support ticket.
{% endstep %}
{% endstepper %}

{% if visitor.claims.unsigned.persona === "channel_partner" || visitor.claims.unsigned.persona === "cp_plus_tech" || visitor.claims.unsigned.persona === "staff" %}
## Partner deployment checklist

- Confirm the customer is on a supported Command Centre version.
- Validate browser support for the operator environment.
- Document any network proxy requirements before go-live.
{% endif %}

