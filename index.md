---
layout: default
---

{% for post in site.posts %}
  <article class="post">
    <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
    <br />
    {{ post.content }}
    <br />
  </article>
{% endfor %}
