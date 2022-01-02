---
layout: infolab-toplevel
title: Data
permalink: /data/
header:
  overlay_image: /assets/images/banner.jpg
  overlay_filter: "0.4"
toc: true
---

## Multilayer network data

{% for dataset in site.data.data.multilayer %}

**{{ dataset.name }}**

**Layers:** {{ dataset.layers }}; **Actors:** {{ dataset.actors }}; **Edges:** {{ dataset.edges }}.<br/>
**Multi-actor types:** {{ dataset.mat }}; **Multi-edge types:** {{ dataset.met }}; **Attributes:** {{ dataset.attr }}<br/>
**Description:** *{{ dataset.description }}*<br/>
**Links:** [data]({{ dataset.url }}) [bibtex](/assets/bib/data/{{ dataset.bibtex }})

{% endfor %}

