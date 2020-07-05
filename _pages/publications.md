---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

Full List at <u><a href="https://dblp.uni-trier.de/pers/v/Vatsavai:Ranga_Raju.html">DBLP</a>,</u> <u><a href="https://scholar.google.com/citations?user=y-JsL4kAAAAJ&hl=en">Google Scholar</a>.</u>

## Upcoming (Accepted Papers)

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
