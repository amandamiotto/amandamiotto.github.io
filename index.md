
{% include collapse.html %}

<button onclick="myFunction('myDIV')">Click Me</button>
<button onclick="myFunction('taggedDIV')">Tagged Click Me</button>

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
    <div id="taggedDIV">
    <tr id="taggedDIV">
    <td>{{ t.name }}</td>
    <td>{{ t.institute }}</td>
    <td>{{ t.Completed }}</td>
  </tr>
    </div>
    {% endif %}
{% endfor %}
  
  Does this hide? <div id="taggedDIV"> Yes </div>

</tbody>
  </table>
