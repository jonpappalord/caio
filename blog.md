---
layout: default
title: Blog
permalink: /blog/
description: Stories, explanations and research outcomes from the CAIO project.
---

<p class="blog-intro">Stories from CAIO about how artificial intelligence and cities shape one another. We explain new research findings, methods and their implications for urban life.</p>

{% if site.posts.size > 0 %}
<div class="blog-list">
  {% for post in site.posts %}
  <article class="blog-card">
    <p class="blog-card-meta">
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
      {% if post.category %}<span aria-hidden="true">·</span><span>{{ post.category }}</span>{% endif %}
    </p>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {% if post.subtitle %}<p>{{ post.subtitle }}</p>{% elsif post.excerpt %}<p>{{ post.excerpt | strip_html | truncatewords: 34 }}</p>{% endif %}
    <a class="blog-read-more" href="{{ post.url | relative_url }}" aria-label="Read {{ post.title | escape }}">Read article →</a>
  </article>
  {% endfor %}
</div>
{% else %}
<p class="empty-state">The first CAIO research stories will appear here soon.</p>
{% endif %}
