---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

Full List :: <u><a href="https://dblp.uni-trier.de/pers/v/Vatsavai:Ranga_Raju.html">[DBLP]</a></u>

## Upcoming (Accepted Papers)

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
