---
layout: infolab-toplevel
title: Publications
permalink: /publications/
header:
  overlay_image: /assets/images/water.jpg
  overlay_filter: "0.4"
toc: true
---

<h1>Publications</h1>

{% for year_data in site.data.publications %}
  <h2>{{ year_data.year }}</h2> <!-- Display the year -->
  {% for pub in year_data.publications %}
    <div class="publication-entry">
      <strong>{{ pub.title }}</strong><br/>
      <em>{{ pub.author }}</em><br/>
      {% if pub.type == "article" %}
        {{ pub.journal }}{% if pub.volume %}, Vol. {{ pub.volume }}{% endif %}{% if pub.number %}({{ pub.number }}){% endif %}, {{ pub.year }}
      {% elsif pub.type == "in-proceedings" %}
        In: {{ pub.conference }}, {{ pub.year }}
      {% elsif pub.type == "chapter" %}
        Chapter in: {{ pub.book }}, {{ pub.year }}
      {% elsif pub.type == "thesis" %}
        {{ pub.description }}, {{ pub.year }}
      {% endif %}
      {% if pub.doi %}<br/>DOI: <a href="https://doi.org/{{ pub.doi }}">{{ pub.doi }}</a>{% endif %}
      {% if pub.fulltext %}<br/><a href="{{ pub.fulltext }}" target="_blank">Full Text</a>{% endif %}
      {% if pub.git %}<br/><a href="{{ pub.git }}" target="_blank">GitHub Repository</a>{% endif %}
    </div>
    <br/>
  {% endfor %}
{% endfor %}
