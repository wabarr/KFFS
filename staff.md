---
title: KFFS Staff
layout: page
---

<div class="row">
{% assign people = site.people | where: "staff_member", "yes" | sort:"family_name" %}
{% include people_list.html %}
</div>