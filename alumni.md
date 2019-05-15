---
title: KFFS Alumni
layout: page
---

<div class="row">
{% assign people = site.people | where: "alum", "yes" | where: "staff_member", "no" | sort:"family_name" %}
{% include people_list.html %}
</div>