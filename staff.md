---
title: KFFS Staff
layout: page
---

<div class="row">
{% assign people = site.people | sort:"family_name" %}
{% for person in people %}
{% if person.staff_member == "yes" %}
<div class="col-lg-4 col-md-6 mb-30px card-group">

<div class="card h-100">
<div class="maxthumb">
{% if person.headshot != "" %}
<img class="img-fluid" src="{{site.baseurl}}/{{person.headshot}}" alt="{{ person.first_name }} {{person.family_name}}">
{% else %}
<img class="img-fluid" src="{{site.baseurl}}/assets/images/blog-authors/unknown.png" alt="{{ person.first_name }} {{person.family_name}}">
{% endif %}
</div>

<div class="card-body">
<h2 class="card-title"><a class="text-dark">{{ person.first_name }} {{person.family_name}}</a></h2>
<p class="card-text">{{ person.content }}</p>    
</div>

<div class="card-footer">
<div class="wrapfooter">
<div class="row">
{% if person.email != "" %}
<div class="col-lg-4 col-md-6">
<a href="mailto:{{person.email}}">
   Contact <i class="fa fa-envelope fa-1x"></i>
</a>
</div>
{% endif %}
{% if person.twitter %}
<div class="col-lg-4 col-md-6">
<a href="https://twitter.com/{{person.twitter | replace:'@',''}}">
   Follow <i class="fab fa-twitter fa-1x"></i>
</a>
</div>
{% endif %}
</div>
</div>
</div>

</div>
</div>
{% endif %}
{% endfor %}
</div>