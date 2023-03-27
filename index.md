
{% include collapse.html %}


<button onclick='myFunction("taggedDIV")'>Tagged Click Me</button>

<div id="taggedDIV">
  Does this hide?  Yes 
</div>

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
    <div id='taggedDIV'>
    <tr id='taggedDIV'>
    <td>{{ t.name }}</td>
    <td>{{ t.institute }}</td>
    <td>{{ t.Completed }}</td>
  </tr>
    </div>
    {% endif %}
{% endfor %}

</tbody>
  </table>
  
