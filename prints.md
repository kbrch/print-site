---
layout: archive
---

{% include base_path %}

<h3 class="archive__subtitle">Prints</h3>

<ul class="print-list">
{% for print in site.prints %}
  <li>
    <a href="/prints/{{ print.title }}">
      <img src="{{ print.main_image }}" alt="" />
      <br/>
      <p>{{ print.title | replace: '_', ' '}}</p>
      {% assign thisArtist2 = print.artist_id %}
      <small>{{ site.data.artists[thisArtist2].name }}</small>

    </a>
  </li>
{% endfor %}
</ul>

{% include paginator.html %}
