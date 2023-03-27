
{% include collapse.html }%

<button class="collapsible" id="yaml">Click here for the code.</button>

<div class="content" id="yamldata" markdown="1">
  CONTENT
</div>



Tags for this site include 

{% for t in {{ site.data.Qual }} %}
{{Tags.t}}
{% end for %}

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

