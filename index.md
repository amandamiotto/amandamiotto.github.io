
{% include collapse.html %}
{% include buttoncreator.html %}


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
    <td>{{ t.Completed }}{{ t.Tags }}</td>
  </tr>
    {% endif %}
{% endfor %}

</tbody>
  </table>



<div class="Teaching Communications">
  Does this hide?  Yes 
</div>
