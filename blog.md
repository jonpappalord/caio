---
layout: default
title: Dissemination
permalink: /blog/
description: Stories, explanations and research outcomes from the CAIO project.
---

<p class="blog-intro">Stories and events from CAIO about how AI and cities shape one another. We tell new research findings, methods and their implications for urban life.</p>

{% if site.posts.size > 0 %}
<div class="blog-list">
  {% for post in site.posts %}
  <article class="blog-card">
    <p class="blog-card-meta">
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
      {% if post.category %}<span aria-hidden="true">·</span><span>{{ post.category }}</span>{% endif %}
    </p>

    {% if post.media_type %}
    <h2>{{ post.title }}</h2>
    {% else %}
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {% endif %}

    {% if post.subtitle %}<p>{{ post.subtitle }}</p>{% elsif post.excerpt %}<p>{{ post.excerpt | strip_html | truncatewords: 34 }}</p>{% endif %}

    {% if post.media_type %}
      {% assign player_title = post.media_title | default: post.title %}
      {% include media-player.html type=post.media_type src=post.media_src id=post.media_id poster=post.media_poster title=player_title %}
    {% else %}
    <a class="blog-read-more" href="{{ post.url | relative_url }}" aria-label="Read {{ post.title | escape }}">Read article →</a>
    {% endif %}
  </article>
  {% endfor %}
</div>
{% else %}
<p class="empty-state">The first CAIO research stories will appear here soon.</p>
{% endif %}
