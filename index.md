---
layout: default
---

# Recent Research

{% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h2>
    <p>{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
    <time>{{ post.date | date_to_string }}</time>
  </article>
  <hr>
{% endfor %}
