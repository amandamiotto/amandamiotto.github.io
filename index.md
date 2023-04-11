
{% include collapse.html %}
{% include buttoncreator.html %}
{% include analytics.html %}
{% assign Tblclass = "," | split: "," %}
<center>
<button onclick='hideAll()'>Remove filters</button></center>


{% for t in site.data.Qual %}
   {% assign Tblclass= Tblclass | push: t.Tags %}
{% endfor %}

{% assign Tblclass= Tblclass | sort | uniq | join:" " %}

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
    <tr class="{{ t.Tags | join:" " }}">
    <td>{{ t.name }}</td>
    <td>{{ t.institute }}</td>
    <td>{{ t.Completed }}</td>
  </tr>
{% endfor %}

</tbody>
  </table>



<div class="Teaching Communications">
  Does this hide?  Yes 
</div>
