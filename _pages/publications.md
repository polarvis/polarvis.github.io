---
layout: infolab-toplevel
title: Publications 
permalink: /publications/
title: Events 
permalink: /events/
header:
  overlay_image: /assets/images/water.jpg
  overlay_filter: "0.4"
toc: true
---



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
