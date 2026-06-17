---
description: "How the demo models public, partner, technology partner, and staff access."
icon: user-lock
---

# Visitor authentication model

The demo uses unsigned visitor claims so the team can switch personas during a live call. In production, the same claims would normally come from Visitor Authentication backed by Gallagher identity systems.

| Demo persona | Claim value | What they can see |
| --- | --- | --- |
| End user | `end_user` | Public product and support content |
| Channel Partner | `channel_partner` | Public plus commercial partner content |
| High Security Channel Partner | `high_security_partner` | Standard partner content plus high security resources |
| Technology Partner | `technology_partner` | SDKs, integration guides, partner API notes |
| Gallagher staff | `staff` | Full demo view and internal-only migration governance |
| CP plus Tech Partner | `cp_plus_tech` | Both channel partner and technology partner content |

{% stepper %}
{% step %}
### Visitor lands on the public site

No login is required for general product documentation, release notes, advisories, || support routes.
{% endstep %}

{% step %}
### Visitor signs in through Gallagher identity

Visitor Authentication attaches claims that describe the visitor's relationship to Gallagher.
{% endstep %}

{% step %}
### GitBook evaluates adaptive conditions

The same page can reveal extra blocks, pages, sections, || header links for each authenticated audience.
{% endstep %}
{% endstepper %}

