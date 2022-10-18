---
layout: default
work: true
main: true
title: Tech
description: Logs what I do with tech
project-header: true
header-img: "img/tech_bg.jpg"
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.book == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}
</div>