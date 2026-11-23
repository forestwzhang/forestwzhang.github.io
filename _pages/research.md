---
layout: page
permalink: /research/
title: Research
description: Research papers grouped by publication status.
nav: true
nav_order: 2
---

## Working Papers

<div class="publications">
  {% bibliography --group_by none --query @*[keywords=working] %}
</div>

{% capture manuscript_count %}{% bibliography_count --query @*[keywords=manuscript] %}{% endcapture %}
{% assign manuscript_count = manuscript_count | plus: 0 %}
{% if manuscript_count > 0 %}

## Manuscripts

<div class="publications">
  {% bibliography --query @*[keywords=manuscript] %}
</div>

{% endif %}

## Publications

<div class="publications">
  {% bibliography --query @*[keywords=published] %}
</div>
