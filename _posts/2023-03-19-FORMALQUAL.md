---
layout: post_markdown
date: 2023-03-19 01:01:01 -0000
title: Formal Qualifications
description: 
tags: Qualifications All
---
| Degree  | Institute | Year |
|--------------------|--------|---------|
| Bachelor of Science (Bioinformatics) | UniSQ | 2007 |



{% for q in site.data.Qual %}
{{ q.name }}
{% endfor %}
