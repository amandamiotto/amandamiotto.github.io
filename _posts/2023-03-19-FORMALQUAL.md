---
layout: post_markdown
date: 2023-03-19 01:01:01 -0000
title: Formal Qualifications
description: 
tags: Qualifications All
---

<table>
<thead>
  <tr>
    <th>Degree</th>
    <th>Institute</th>
    <th>Year Completed</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
    
    
| Degree  | Institute | Year Completed |
|--------------------|--------|---------|
{% for q in site.data.Qual %}
| {{ q.name }} | {{ q.institute }} | {{ q.Completed }} |
|||
{% endfor %}

