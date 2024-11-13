---
layout: infolab-toplevel
title: Team
permalink: /team/
header:
  overlay_image: /assets/images/water.jpg
  overlay_filter: "0.7"
---

## Project members

<style>
  .profile p {
    font-size: 0.8em; /* Adjust this value as needed */
  }
</style>


<div class="profiles"> 
{% for person in site.data.people.members %}
<figure class="profile">
  <img class="profilepic" src="{{ person.pic }}" alt="{{ person.name }}">
  <figcaption class="profile">
    <p>
      <a href="{{ person.url }}" target="_blank">{{ person.name }}</a><br/>
      {{ person.title }} <br/> 
      {{ person.institution }} <br/> 
      {{ person.position }}
    </p>
  </figcaption>
</figure>
{% endfor %}
<div class="stop"/>
</div>
