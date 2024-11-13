---
layout: infolab-toplevel
title: Team
permalink: /team/
header:
  overlay_image: /assets/images/water.jpg
  overlay_filter: "0.7"
---

## Project members


<div class="profiles-grid"> 
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
</div>

Add the following CSS (inside a <style> tag in your HTML or in your site’s CSS file):

.profiles-grid {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  gap: 20px;
  align-items: start;
}

.profile {
  text-align: center;
}

.profilepic {
  width: 100px; /* Adjust as needed */
  height: auto;
  border-radius: 50%;
}
