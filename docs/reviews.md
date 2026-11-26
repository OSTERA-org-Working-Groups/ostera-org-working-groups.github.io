---
layout: page
title: Public Reviews
permalink: /reviews/
lead: "This page lists every Public Review from every Working Group at OSTERA."
---

{% comment %}
  The theme fills in the tables below when the page is viewed, from each
  Working Group's /<id>/reviews.json, which each Working Group site builds
  from its work items' registry.yaml files. Nothing on this page needs to
  be edited when a Public Review opens.
{% endcomment %}
{%- capture ids %}{% for wg in site.data.working_groups %}{% if wg.website %}{{ wg.id }} {% endif %}{% endfor %}{% endcapture %}
<div class="all-reviews" data-all-reviews="{{ ids | strip }}">
<p>The Public Reviews of each Working Group are on its Work Items page:</p>
<ul>
{%- for wg in site.data.working_groups %}{% if wg.website %}
<li><a href="{{ '/' | append: wg.id | append: '/work-items/' | relative_url }}">{{ wg.name }}{% if wg.abbr %} ({{ wg.abbr }}){% endif %}</a></li>
{%- endif %}{% endfor %}
</ul>
</div>

## How to Comment

Anyone may comment on a draft during its Public Review, even if they are not a member of OSTERA. To make a comment, click on the document that you are interested in from the Draft column above. Then from the document's details page, find the How to Comment section, which will contain a link to the Working Group's repository for opening an issue and the link for sending an email to [public-review@ostera.org](mailto:public-review@ostera.org).

<!-- BEGIN STANDARD TEXT -->

## Intellectual Property

Anything you submit to OSTERA, such as an issue, a pull request, a comment, or an email, is a contribution under the [OSTERA IPR and Copyright Policy](https://ostera.org/policies/), and by submitting it you agree to that policy. Do not submit anything you do not have the right to contribute.

If you have knowledge of intellectual property rights, including patents, copyrights, trademarks, and service marks, for software or text, the use of which may be required to implement or publish any of the work items being considered, please disclose it by following the instructions at [ostera.org/ipr/](https://ostera.org/ipr/) or contact the Secretariat at [secretariat@ostera.org](mailto:secretariat@ostera.org).

<!-- END STANDARD TEXT -->

## Citing Drafts

Drafts are works in progress. They have not been approved by OSTERA and **MUST NOT** be cited as OSTERA publications. Approved documents are published at [pub.ostera.org](https://pub.ostera.org/).
