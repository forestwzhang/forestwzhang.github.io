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
  {% bibliography --query @*[keywords=working] %}
</div>

## Manuscripts

<div class="publications">
  {% bibliography --query @*[keywords=manuscript] %}
</div>

## Publications

<div class="publications">
  {% bibliography --query @*[keywords=published] %}
</div>
