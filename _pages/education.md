---
layout: infolab-toplevel
title: Education
permalink: /education/
header:
  overlay_image: /assets/images/banner.jpg
  overlay_filter: "0.4"
toc: true
---

The following courses on topics related to our research are given by members of the Infolab. Normally, students willing to work on a master thesis with us are required to have read at least an introductory course in Data Mining, and PhD students must take the Network Science and the Readings in Network Science courses. 

## Regularly given courses

{% for course in site.data.courses %}

### [{{ course.name }}]({{ course.url }})

**Level:** {{ course.level }}. **Frequency:** {{ course.frequency }}<br/>
**Description:** *{{ course.description }}*<br/>

{% endfor %}


## Tutorials

We regularly give tutorials at international venues (past venues include the ESSLLI school and the SunBelt, IC2S2, Asonam, ICWSM, SocInfo and ARS conferences). The material for the tutorials on multilayer network analysis is available on the GitHub pages of our [R library]() and [Python library]().
