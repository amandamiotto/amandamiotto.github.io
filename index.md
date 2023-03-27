
{% include collapse.html %}

<button onclick="myFunction('myDIV')">Click Me</button>

<div id="myDIV">
  This is my DIV element.
</div> 


Tags for this site include 


Here is a list of posts


Here's the post tag loop

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %} 
  {{ post }}
    {% endfor %}
  </ul>
{% endfor %}

