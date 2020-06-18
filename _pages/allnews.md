---
title: "News"
layout: textlay
excerpt: "Physimals at Nottingham University."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}

<p> &nbsp; </p>
