---
title: "Man Yi - Publications"
layout: gridlay
excerpt: "Man Yi -- Publications."
sitemap: false
permalink: /publications/
---

# Publications

{% assign total = site.data.publist.size %}
{% for publi in site.data.publist reversed %}
  {{ total - forloop.index0 + 1 }}. {{ publi.title }},
  <em>{{ publi.authors }}</em><br />
  <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  [(pdf)]({{ site.baseurl }}/downloads/{{ publi.link.doc }})<br /><br />
{% endfor %}

