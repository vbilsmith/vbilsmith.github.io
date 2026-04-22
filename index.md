---
---

# The Veterinary and Biological Informatics Lab at Smith College

Here in the VBIL within the Computer Science Department at Smith, we are interested in different ways that we can represent complex ideas, especially in the domain of health AI. Projets range from pure bioinformatics to document engineering, all in the interest of more effectively representing complex ideas about the world around us.

{% include section.html %}

## Latest News

{% if site.posts.size > 0 %}
{% for post in site.posts limit: 3 %}
{% include post-excerpt.html lookup=post.slug %}
{% endfor %}
{% else %}
Future lab announcements, milestones, publications, and event updates will appear here.
{% endif %}

{%
  include button.html
  link="news"
  text="View all news"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% include section.html %}

## Highlights

{% capture text %}

Learn more about our research by browsing our publications.
{%
  include button.html
  link="research"
  text="See our publications"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/thumbnails/dogproject.jpg"
  link="research"
  title="Our Research"
  text=text
%}

{% capture text %}

Smith students of all years and many different majors are contributing to our ongoing research in bioinformatics, health AI, document engineering, and more.

{%
  include button.html
  link="team"
  text="Meet our team"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/labPhoto-2024-03.jpg"
  link="team"
  title="Our Team"
  text=text
%}
