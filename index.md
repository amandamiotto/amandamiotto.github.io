
{% include collapse.html %}

<button onclick="myFunction('myDIV')">Click Me</button>

<div id="myDIV">
  This is my DIV element.
</div> 


Tags for this site include 


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
    <tr>
    <td>{{ t.name }}</td>
    <td>{{ t.institute }}</td>
    <td>{{ t.Completed }}</td>
  </tr>
    {% endif %}
{% endfor %}

</tbody>
  </table>
