---
title: News
nav:
  order: 4
  tooltip: Lab updates and announcements
redirect_from:
  - /blog
  - /blog/
---

# {% include icon.html icon="fa-regular fa-newspaper" %}News

{% if site.posts.size > 0 %}

{% include search-box.html %}

{% include search-info.html %}

{% assign current_year = "" %}

{% for post in site.posts %}
{% assign post_year = post.date | date: "%Y" %}
{% if post_year != current_year %}
{% assign current_year = post_year %}
## {{ current_year }}
{% endif %}
{% include post-excerpt.html
  lookup=post.slug
  show_full_content=true
%}
{% endfor %}

{% else %}

No news posts have been published yet.

To publish one, add a Markdown file to `_posts/` using the filename format `YYYY-MM-DD-title.md`.

{% endif %}
