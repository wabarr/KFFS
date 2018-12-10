---
title: KFFS Staff
layout: page
---

{% assign people = site.people | sort:"family_name" %}

{% for person in people %}
{% if person.staff_member == "yes" %}
<h2>{{person.first_name}} {{person.family_name}}</h2>
{% endif %}
{% endfor %}