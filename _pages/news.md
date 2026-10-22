---
title: "News"
permalink: /news/
author_profile: true
---

{% assign years = site.data.news | group_by_exp: "item", "item.date | date: '%Y'" %}
<div class="page-card">
{%- for year in years %}
<h2 class="year-heading">{{ year.name }}</h2>
{% include news-list.html items=year.items date_format="%b" timeline=true %}
{%- endfor %}
</div>
