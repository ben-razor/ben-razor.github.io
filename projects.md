---
layout: page
title: Projects
permalink: /projects/
---
A collection of demonstration projects. 

{% for item in site.data.projects %}
  {% capture img_name %}{{ item.img_name }}{% endcapture %}
  {% capture name %}{{ item.name }}{% endcapture %}
  {% capture desc %}{{ item.desc}}{% endcapture %}
  {% capture link %}{{ item.link }}{% endcapture %}
  {% capture item %}{{ item }}{% endcapture %}

  {% include proj-summary.html img_name=img_name name=name desc=desc link=link item=item%}
{% endfor %}

You can find the source code for my recent projects at:
{% include icon-github.html username="ben-razor" %} 