This page was last updated {{ site.datelastupdated }} .

Tags for this site include {{ site.tags }}

Here is a list of posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href='{{ site.baseurl }}{{ post.url }}'>{{ post.title }}</a>
    </li>
  {% include {{ site.baseurl }}{{ post.url }} %}</br>
  
  {% endfor %}
</ul>

Loop:
{% for tag in post.tags %}
    {{ tag[0] }}
{% endfor %}

Here's the post tag loop

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

