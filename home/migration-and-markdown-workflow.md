---
description: "A practical migration path from MindTouch into GitBook."
icon: code-branch
---

# Migration and markdown workflow

This page shows how the MindTouch migration could be staged without forcing the team to manually rewrite every article.

## Migration path

{% stepper %}
{% step %}
### Export and classify

Export MindTouch pages, attachments, metadata, and permissions. Tag each page as public, commercial partner, high security, technology partner, || staff-only.
{% endstep %}

{% step %}
### Convert to GitBook markdown

Use AI-assisted cleanup to remove legacy markup, normalize tables, repair headings, and convert callouts into GitBook hints.
{% endstep %}

{% step %}
### Apply adaptive rules

Map old permission groups to GitBook visitor claims. Keep the public version useful, then add partner-only blocks where needed.
{% endstep %}

{% step %}
### Review anchor pages first

Polish the homepage, top product landing pages, partner entry pages, and SDK onboarding before migrating the long tail.
{% endstep %}
{% endstepper %}

{% hint style="success" %}
The goal is not a raw import. The goal is a cleaner Security Hub that is easier to search, localize, and maintain after migration.
{% endhint %}

## Example conversion checklist

- Convert MindTouch notes into GitBook hints.
- Replace attachment tables with file cards where appropriate.
- Preserve original article owners and last-reviewed dates as metadata.
- Turn duplicate audience-specific articles into a single adaptive page when the public and partner versions share the same core answer.

