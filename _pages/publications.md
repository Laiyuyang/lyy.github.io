---
title: "Man Yi - Publications"
layout: gridlay
excerpt: "Man Yi -- Publications."
sitemap: false
permalink: /publications/
---

# Publications

{% assign total = site.data.publist.size %}
{% assign counter = total %}
{% for publi in site.data.publist %}
  {{ counter }}. {{ publi.title }},
  <em>{{ publi.authors }}</em><br />
  <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  [(pdf)]({{ site.baseurl }}/downloads/{{ publi.link.doc }})<br /><br />
  {% assign counter = counter | minus: 1 %}
{% endfor %}




