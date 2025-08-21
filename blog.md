---
layout: default
title: Мой блог
---

# Мои статьи

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})
{{ post.date | date: "%d.%m.%Y" }}

{{ post.excerpt | truncatewords: 30 }}

[Читать далее...]({{ post.url }})
{% endfor %}
