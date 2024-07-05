---
title: "Man Yi - Publications"
layout: gridlay
excerpt: "Man Yi -- Publications."
sitemap: false
permalink: /publications/
---

# Publications

{% assign total = site.data.publist.size %}
{% assign reversed_list = site.data.publist | reverse %}
{% for publi in reversed_list %}
  <div class="publications">
    <div class="publication-title">{{ total - forloop.index0 }}. {{ publi.title }}</div>
    <div class="publication-authors"><em>{{ publi.authors }}</em></div>
    <div class="publication-link">
      <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
      <a href="{{ site.baseurl }}/downloads/{{ publi.link.doc }}">(pdf)</a>
    </div>
  </div>
{% endfor %}


