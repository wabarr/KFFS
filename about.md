---
layout: page
title: About the Koobi Fora Field School
comments: false
---
{% if jekyll.environment == 'production' %}  {% endif %} {% capture layout
%}{% if page.layout %}layout-{{ page.layout }}{% endif %}{% endcapture %}

[ ![{{ site.name }}][1] ][2]

{% if page.url == "/" %}

  * {% else %}

  * {% endif %} [Home][3]

{% if page.url == "/blog" %}

  * {% else %}

  * {% endif %} [Blog][4]

{% if page.url == "/about.html" %}

  * {% else %}

  * {% endif %} [About][5]

  * [__][6]

  * [__][7]

# {{ site.name }}

{{ site.description }}

{{ content }}

![{{site.title}}][1]   Subscribe to our mailing list to stay updated!

## Explore →

{% assign tags_list = site.categories %} {% if tags_list.first[0] == null %}
{% for tag in tags_list %} [{{ tag | capitalize }} {{ site.tags[tag].size
}}][8] {% endfor %} {% else %} {% for tag in tags_list %} [{{ tag[0] |
capitalize }} ({{ tag[1].size }})][9] {% endfor %} {% endif %} {% assign
tags_list = nil %}

Copyright © {{ site.time | date: "%Y" }} {{ site.name }}


   [1]: {{ site.baseurl }}/{{ site.logo }}

   [2]: {{ site.baseurl }}/

   [3]: {{ site.baseurl }}/index.html

   [4]: {{ site.baseurl }}/blog.html

   [5]: {{ site.baseurl }}/about

   [6]: https://www.facebook.com/KoobiForaFieldSchool/

   [7]: https://twitter.com/koobiforafs

   [8]: {{ site.baseurl }}/category/{{ tag }}

   [9]: {{ site.baseurl }}/category/{{ tag[0] }}

