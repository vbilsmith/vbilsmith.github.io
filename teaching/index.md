---
title: Courses
nav:
  order: 4
  tooltip: Smith CSC course information
---

# {% include icon.html icon="fa-solid fa-feather-pointed" %}Courses

Here is some information about the classes that Prof. Rando has taught at Smith.

{% include section.html %}

{% assign distribution_filters = site.data.courses
  | map: "distribution"
  | join: ","
  | split: ","
  | array_filter
  | uniq
%}
{% assign ordered_distributions = "Core|Seminar|Systems|Theory|Programming" | split: "|" %}

{% include search-box.html %}

{% if distribution_filters.size > 0 %}
<div class="tags">
  {% for distribution in ordered_distributions %}
    {% if distribution_filters contains distribution %}
    <a
      href="{{ '/teaching' | relative_url }}?search=&quot;{{ distribution }}&quot;"
      class="tag"
      data-tooltip="Show {{ distribution }} courses"
    >
      {{ distribution }}
    </a>
    {% endif %}
  {% endfor %}
</div>
{% endif %}

{% include search-info.html %}

{% include list.html data="courses" component="course-excerpt" %}
