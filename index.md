Tags for this site include 

{% for t in {{ site.data.Qual.Tags }} %}
{{t}}
{% endfor %}

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

