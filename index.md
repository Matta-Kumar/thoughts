---
layout: base.html
title: AI SEO Thought
description: Mattakumar SEO Thought
date: 2025-06-20
pagination:
  data: collections.posts
  size: 5
  alias: posts
---

All notes being published here from Obsidian using [Eleventy](https://11ty.dev/).

<div>
{% for post in posts %}
<ul>
    <li><a href="https://www.mattakumar.com/thought{{ post.url }}">{{ post.data.title }}</a></li>
</ul>
{% endfor %}

<!-- Pagination links -->

{% if pagination.href.next %}
<a class="contrast" role="button" href="{{ pagination.href.next }}">→</a>
{% endif %}
{% if pagination.href.previous %}
<a class="contrast" role="button" href="{{ pagination.href.previous }}">←</a>
{% endif %}

</div>
