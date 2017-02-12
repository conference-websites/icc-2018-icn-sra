---
layout: default
title: Committees
---

## Organizing Committee

{% assign item = site.data.committees['org'] %}
{% include committees.html committees=item %}

[Contact workshop chairs](mailto:{% for i in item[0].people %}{{ i.email }}{% if forloop.last != true %},{% endif %}{% endfor %}?subject=[ICN-SRA'2017]){: data-role="button" class="button" }.

## Technical Program Committee

{% assign item = site.data.committees['tpc'] %}
{% include committees.html committees=item %}
