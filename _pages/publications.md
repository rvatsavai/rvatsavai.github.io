---
layout: archive
title: "Publications"
test: see 
permalink: /publications/
author_profile: true
---

Why <u><a href="https://dblp.uni-trier.de/pers/v/Vatsavai:Ranga_Raju.html">DBLP</a>.</u>

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
