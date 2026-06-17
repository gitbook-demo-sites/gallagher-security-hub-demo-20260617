---
description: "Example public release notes with partner-only deployment context."
icon: clock-rotate-left
---

# Release notes

{% updates %}
{% update date="2026-06-17" tags="Command Centre, AccessNow" %}
## Command Centre 9.60 demo release

New operator dashboard widgets, improved AccessNow session handling, and clearer event filtering.

{% if visitor.claims.unsigned.persona === "channel_partner" || visitor.claims.unsigned.persona === "cp_plus_tech" || visitor.claims.unsigned.persona === "staff" %}
Partner note: schedule upgrades for customers using custom integrations after validating test events in staging.
{% endif %}
{% endupdate %}

{% update date="2026-05-28" tags="Security Hub" %}
## Security Hub navigation refresh

Public product articles, release notes, and support pathways are now organized around common user journeys.
{% endupdate %}
{% endupdates %}

