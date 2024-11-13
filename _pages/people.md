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
    font-size: 0.8em; /* Adjust font size as needed */
    word-wrap: break-word; /* Allows words to break to the next line if too long */
    word-break: break-word; /* Forces breaks in words that are too long */
    max-width: 200px; /* Set a max width to control the width of the box */
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
      {{ person.institution2 }} <br/> 
      {{ person.position }}
    </p>
  </figcaption>
</figure>
{% endfor %}
<div class="stop"/>
</div>
