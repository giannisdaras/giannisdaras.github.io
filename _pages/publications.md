---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

For the most updated version of my publications page, see my [Google Scholar profile](https://scholar.google.com/citations?user=LaScvbQAAAAJ&hl=en).


{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
