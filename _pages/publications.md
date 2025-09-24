---
layout: infolab-toplevel
title: Publications 
permalink: /publications/
header:
  overlay_image: /assets/images/water.jpg
  overlay_filter: "0.4"
toc: true
excerpt: " "
---

{% for publist in site.data.publications %}
## {{ publist.year }}

{% for pub in publist.publications %}
**{{ pub.title }}**<br/>
*{{ pub.author }}*<br/>
{% if pub.type == "article" %}{{ pub.journal }}{% if pub.volume %}, Vol. {{ pub.volume }}{% endif %}{% if pub.number != nil %}({{ pub.number }}){% endif %}, {{ pub.year }}
{% elsif pub.type == "in-proceedings" %}In: {{ pub.conference }}, {{ pub.year }}
{% elsif pub.type == "chapter" %}Chapter in: {{ pub.book }}, {{ pub.year }}
{% elsif pub.type == "thesis" %}{{ pub.description }}, {{ pub.year }}
{% endif %}
{% endfor %}

{% endfor %}

