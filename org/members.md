---
layout: page
title: members
permalink: /members/
author: Sejun Kwon
---

{% for staff_member in site.staff_member %}
  <h2>{{ staff_member.name }} - {{ staff_member.position }}</h2>
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}

{% for member in site.data.members %}
 - <a href="https://github.com/{{ member.github }}"> {{ member.name }} </a>
{% endfor %}