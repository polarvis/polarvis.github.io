---
layout: infolab-toplevel
title: People
permalink: /people/
header:
  overlay_image: /assets/images/water.jpg
  overlay_filter: "0.7"
---

Example of a list generated from the file `_data/people/members.yml`.

## Project members

<div class="profiles"> 
{% for person in site.data.people.members %}
<figure class="profile">
  <img class="profilepic" src="{{ person.pic }}" alt="{{ person.name }}">
  <figcaption class="profile">
  <p>{{ person.name }} <br/> {{ person.title }}</p>
  </figcaption>
</figure>
{% endfor %}
<div class="stop"/>
</div>
