---
layout: page
permalink: /talks/
title: talks
description: Invited talks and seminars.
nav: true
nav_order: 5
---

The most representative talk of my recent research is the one I gave at Columbia Engineering, as part of the Workshop on Emerging Trends in AI — [watch it here](https://youtu.be/4HTuPx6wjJM?si=DVOShkwhiIIMJBON).

<div class="row justify-content-sm-center mt-4 mb-4">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/columbia_photo.jpg" title="Giannis Daras speaking at Columbia Engineering" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

---

#### Invited talks

<table class="table table-sm">
  <tbody>
  {% for t in site.data.talks %}
    <tr>
      <td class="text-muted" style="width:5rem;">{{ t.year }}</td>
      <td>{% if t.url %}<a href="{{ t.url }}" target="_blank" rel="noopener">{{ t.venue }}</a>{% else %}{{ t.venue }}{% endif %}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>
