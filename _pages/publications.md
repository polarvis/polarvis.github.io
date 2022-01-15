---
layout: infolab-toplevel
title: Publications
permalink: /publications/
header:
  overlay_image: /assets/images/banner_small.jpg
  overlay_filter: "0.4"
toc: true
---

Here we only list publications related to the activities of the lab. For other publications of the lab members you can consult their personal pages.

{% for publist in site.data.publications %}
## {{ publist.year }}

{% for pub in publist.publications %}
**{{ pub.title }}**<br/>
*{{ pub.author }}*<br/>
{% if pub.type == "article" %}{{ pub.journal }}, Vol. {{ pub.volume }}{% if pub.number != nil %}({{ pub.number }}){% endif %}, {{ pub.year }}
{% elsif pub.type == "in-proceedings" %}In: {{ pub.conference }}, {{ pub.year }}
{% elsif pub.type == "chapter" %}Chapter in: {{ pub.book }}, {{ pub.year }}
{% elsif pub.type == "thesis" %}{{ pub.description }}, {{ pub.year }}
{% endif %}
{% endfor %}

{% endfor %}
