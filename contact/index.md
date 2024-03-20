---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

For current Smith students who are interested in conducting research, please send me an email and include your resume as well as some information about your computer science, SDS, and/or biology background.

{%
  include button.html
  type="email"
  text="Email"
  link="hrando@smith.edu"
%}
{%
  include button.html
  type="phone"
  text="413­585­4497"
  link="+1-413­585­4497"
%}
{%
  include button.html
  type="address"
  tooltip="Bass Hall 109"
  link="https://maps.app.goo.gl/UNLb1gCmeSGj652V7"
%}

{% include section.html %}

{% capture col1 %}

{%
  include figure.html
  image="images/smithcollege.jpg"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/labPhoto-2024-03.jpg"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

{% include section.html dark=true %}

{% capture col1 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col2 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col3 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}
