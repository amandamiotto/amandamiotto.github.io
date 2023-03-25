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
{% for q in site.data.Qual %}
      <tr>
    <td>{{ q.name }}</td>
    <td>{{ q.institute }}</td>
    <td>{{ q.Completed }}</td>
  </tr>
{% endfor %}

</tbody>
  </table>
