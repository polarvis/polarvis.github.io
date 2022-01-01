---
layout: infolab-toplevel
title: People
permalink: /people/
---

## Members

<div class="profiles"> 
{% for person in site.data.people.members %}
<div class="profile">
  <img class="profilepic" src="{{ person.pic }}" alt="{{ person.name }}">
  <div class="profiletext">
  <p>{{ person.name }} <br/> {{ person.title }}</p>
  </div>
</div>
{% endfor %}
<div class="stop"/>
</div>


## Associate members[^1]

[^1]: Associate members are affiliated with other Departments or Universities, but actively contribute to the Infolab, for example as project co-Principal Investigators or as co-supervisors of junior members. 

{% for person in site.data.people.ass_members %}
**{{ person.name }}**, {{ person.title }}, {{ person.affiliation }}.
{% endfor %}

## Past members[^2]

[^2]: Visiting researchers who spent a significant ammount of time (normally a few months) at the Infolab and previous members (PhD students, postdocs, etc.).

{% for person in site.data.people.past_members %}
**{{ person.name }}**, {{ person.title }} ({{ person.year }}).
{% endfor %}

## Alumni[^3]

[^3]: Master and Bachelor students who did their thesis at the Infolab.

{% for person in site.data.people.alumni %}
**{{ person.name }}**, {{ person.role }} ({{ person.year }})<br/>
*{{ person.thesis }}*.
{% endfor %}
