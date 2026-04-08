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

Use this page for lab updates, student milestones, publications, talks, and other announcements from the VBIL.

{% if site.posts.size > 0 %}

{% include search-box.html %}

{% include search-info.html %}

{% assign posts_by_year = site.posts
  | group_by_exp: "post", "post.date | date: '%Y'"
%}

{% for year in posts_by_year %}
## {{ year.name }}

{% for post in year.items %}
{% include post-excerpt.html lookup=post.slug %}
{% endfor %}

{% endfor %}

{% else %}

No news posts have been published yet.

To publish one, add a Markdown file to `_posts/` using the filename format `YYYY-MM-DD-title.md`.

{% endif %}
