---
title: "Honors"
permalink: /honors/
author_profile: true
layout: archive
collection: honors
---

<ul>
  {% for post in site.honors reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}
</ul>