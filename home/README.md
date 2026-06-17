---
description: "A public-first Gallagher Security Hub that adapts by visitor type."
icon: house
layout:
  width: wide
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: false
  outline:
    visible: false
---

# Gallagher Security Hub

Bring product knowledge, partner resources, developer references, and internal enablement into one public-first GitBook site.

{% include ".gitbook/includes/persona-switcher.md" %}

<table data-view="cards">
<thead>
<tr>
<th></th>
<th></th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://app.gitbook.com/s/XSPACE_PRODUCT/">Product knowledge</a></td>
<td>Public how-to content for end users, installers, operators, and site administrators.</td>
</tr>
<tr>
<td><a href="https://app.gitbook.com/s/XSPACE_PARTNER/">Partner Hub</a></td>
<td>Commercial resources, channel partner workflows, high security notes, and technology partner SDKs.</td>
</tr>
<tr>
<td><a href="https://app.gitbook.com/s/XSPACE_STAFF/">Staff workspace</a></td>
<td>Internal migration playbooks, governance, review ownership, and demo notes for Gallagher teams.</td>
</tr>
</tbody>
</table>

## What changes by audience

{% columns %}
{% column %}
### Public visitors

End users can browse product concepts, setup guides, release notes, advisories, troubleshooting, and training pathways without an account.
{% endcolumn %}

{% column %}
### Authenticated visitors

Channel partners, technology partners, and Gallagher staff see additive material in the same navigation rather than being sent to disconnected portals.
{% endcolumn %}
{% endcolumns %}

{% if visitor.claims.unsigned.persona === "channel_partner" || visitor.claims.unsigned.persona === "high_security_partner" || visitor.claims.unsigned.persona === "cp_plus_tech" || visitor.claims.unsigned.persona === "staff" %}
## Channel partner view

You are seeing extra partner guidance such as ordering notes, commercial FAQs, deployment templates, and certification reminders.
{% endif %}

{% if visitor.claims.unsigned.persona === "technology_partner" || visitor.claims.unsigned.persona === "cp_plus_tech" || visitor.claims.unsigned.persona === "staff" %}
## Technology partner view

You are seeing developer-focused material such as SDK onboarding, integration checklists, sandbox access, and API support paths.
{% endif %}

