---
layout: home
title: Home
hero_title: "Working Groups at OSTERA"
hero_text: "The work at OSTERA is organized into Working Groups and collections of Working Groups can be organized into Centers of Excellence. This is where innovation becomes a standard and focused collaboration drives global impact."
hero_buttons:
  - label: Work With Us
    url: https://ostera.org/membership/
  - label: How to Participate
    url: /participate/
    style: secondary
---

## Current Working Groups

<div class="card-grid">
{%- for wg in site.data.working_groups %}
  <div class="card">
    <h3>{{ wg.name }} ({{ wg.abbr }})</h3>
    <p>{{ wg.purpose }}</p>
    <p>
      {%- if wg.website %}<a href="{{ wg.id | prepend: '/' | append: '/' | relative_url }}">Website</a>{% else %}<a href="https://ostera.org/working-groups/">Details</a>{% endif %}
      {%- if wg.charter != "" %} &middot; <a href="{{ wg.charter }}">Charter</a>{% endif %}
      {%- if wg.repo %} &middot; <a href="https://github.com/OSTERA-org-Working-Groups/{{ wg.id }}/">GitHub</a>{% endif %}
    </p>
  </div>
{%- endfor %}
</div>

## How Working Groups Work

Working Groups are at the heart of the OSTERA process. They unite experts and organizations around shared goals and objectives, accelerating progress from idea to industry ready standard to implementation and adoption. These communities focus on solving real world challenges through open collaboration.

Each working group manages its own website and its own public repository in the [OSTERA Working Groups](https://github.com/OSTERA-org-Working-Groups/) GitHub organization. Approved documents are published at [pub.ostera.org](https://pub.ostera.org/).

To learn how to take part, see [How to Participate](participate/).
