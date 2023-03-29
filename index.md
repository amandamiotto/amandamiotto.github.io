
{% include collapse.html %}


<button onclick='hideTableLine("Teaching")'>Tagged Click Me</button>
{% assign alltags = "" | split: "," | inspect %}


Tags for this site include 
{% for tg in site.data.Qual %}
    {{ tg.Tags }}
    {% for individTags in tg.Tags %}
        {{ individTags | inspect }}
    {% endfor %}
{% endfor %}

Qual 1 Alltags printed here
{{ alltags }}



{% if site.data.Qual.Tags contains "Teaching" %}
Does it find teaching in all tags for Quals?

{% endif %}

<table>
<thead>
  <tr>
    <th>Degree</th>
    <th>Institute</th>
    <th>Year Completed</th>
  </tr>
</thead>
<tbody>    
{% for t in site.data.Qual %}
    {% if t.Tags contains "Teaching" %}
    <tr class="Teaching">
    <td>{{ t.name }}</td>
    <td>{{ t.institute }}</td>
    <td>{{ t.Completed }}</td>
  </tr>
    {% endif %}
{% endfor %}

</tbody>
  </table>



<div class="taggedDIV">
  Does this hide?  Yes 
</div>
