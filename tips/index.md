---
layout: default
work: true
main: true
title: Tips
description: Logs about tips
project-header: true
header-img: "img/tips_bg.jpg"
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.projects == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}
</div>