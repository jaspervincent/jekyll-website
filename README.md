# Jekyll-website
List
- [Blog](https://jaspervincent.github.io)
<nav>
  {% assign baseurl = "/jekyll-website" | concat: page.url %}
  {% for item in site.nav %}
    <a href="{{ item.link }}" 
      {% if  baseurl == item.link %} style="color: red;" {% endif %}
    >
      {{ item.name }}
    </a>
  {% endfor %}
</nav>
