
{% include collapse.html %}


<button onclick='hideTableLine("taggedDIV")'>Tagged Click Me</button>



<div id="myDIV">
  This is my DIV element.
</div> 


Tags for this site include 

{% if site.data.Qual.Tags contains "Teaching" %}
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
    <tr id="taggedDIV">
    <td>{{ t.name }}</td>
    <td>{{ t.institute }}</td>
    <td>{{ t.Completed }}</td>
  </tr>
    {% endif %}
{% endfor %}

</tbody>
  </table>
{% endif %}


<div id="taggedDIV">
  Does this hide?  Yes 
</div>
