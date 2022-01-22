<article>
  <header><h1>{{ include.title | default: page.title }}</h1></header>
  <ul class="archive">
    {% for post in site.projects %}
    <li>
      <time datetime="{{ projects.date | date_to_xmlschema }}">{{ projects.date | date: "%Y-%m-%d" }}</time>
      <a href="{{ projects.url | relative_url }}">{{ projects.title }}</a>
    </li>
    {% endfor %}
  </ul>
</article>
