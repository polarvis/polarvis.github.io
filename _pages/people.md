---
layout: infolab-toplevel
title: Team
permalink: /team/
header:
  overlay_image: /assets/images/water.jpg
  overlay_filter: "0.7"
---

## Project members


<div class="profiles"> 
{% for person in site.data.people.members %}
<figure class="profile">
  <img class="profilepic" src="{{ person.pic }}" alt="{{ person.name }}">
  <figcaption class="profile">
    <p>
      <a href="{{ person.url }}" target="_blank">{{ person.name }}</a><br/>
      {{ person.title }} <br/> 
      {{ person.institution }} <br/> 
      {{ person.institution2 }} <br/> 
      {{ person.position }}
    </p>
  </figcaption>
</figure>
{% endfor %}
<div class="stop"/>
</div>
