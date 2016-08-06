---
layout: archive
---

{% include base_path %}

<h3 class="archive__subtitle">Artists</h3>

{% for post in site.artists %}
  {% include archive-single-artist.html %}
{% endfor %}

{% include paginator.html %}
