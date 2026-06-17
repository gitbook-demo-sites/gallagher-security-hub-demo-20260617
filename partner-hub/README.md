---
description: "Adaptive hub for Channel Partners, High Security partners, and Technology Partners."
icon: handshake
---

# Partner Hub

This space demonstrates the three gated content areas Gallagher described: commercial channel partner content, high security partner resources, and technology partner content.

{% if visitor.claims.unsigned.persona === "end_user" %}
{% hint style="warning" %}
You are viewing the public version. In production this section would require sign-in.
{% endhint %}
{% endif %}

{% if visitor.claims.unsigned.persona === "channel_partner" || visitor.claims.unsigned.persona === "high_security_partner" || visitor.claims.unsigned.persona === "cp_plus_tech" || visitor.claims.unsigned.persona === "staff" %}
## Channel partner access active

Commercial resources, quoting notes, customer handoff material, and certification guidance are visible.
{% endif %}

{% if visitor.claims.unsigned.persona === "technology_partner" || visitor.claims.unsigned.persona === "cp_plus_tech" || visitor.claims.unsigned.persona === "staff" %}
## Technology partner access active

SDK, sandbox, and integration resources are visible.
{% endif %}

{% if visitor.claims.unsigned.persona === "cp_plus_tech" %}
{% hint style="success" %}
Combined-access view: this visitor sees both Channel Partner and Technology Partner material in one site.
{% endhint %}
{% endif %}

