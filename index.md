---
layout: default
permalink: /
---

# Home

I am interested in how to predict behaviors of collections of objects reliably and efficiently. This applies to how neurons give rise to high-level reasoning, how embryos grow into adults, how carp swim in schools, how traffic flows in cities, how infectious diseases spread through populations, and how societies make progress.

[Contacts](contact.md).

## Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

## Posts by Tag

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
