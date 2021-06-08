---
layout: page
title: About
permalink: /about/
---
Ben Razor is a software engineer with over 10 years experience developing sports games and audio visual projects
for web and Android.

{% for item in site.data.projects %}
  {% capture img_name %}{{ item.img_name }}{% endcapture %}
  {% capture name %}{{ item.name }}{% endcapture %}
  {% capture desc %}{{ item.desc}}{% endcapture %}
  {% capture link %}{{ item.link }}{% endcapture %}

  {% include proj-summary.html img_name=img_name name=name desc=desc link=link %}
{% endfor }

You can find the source code for my recent projects at:
{% include icon-github.html username="ben-razor" %} 