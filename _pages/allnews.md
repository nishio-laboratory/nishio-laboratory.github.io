---
title: "Nishio Lab - Research Project"
layout: personal
excerpt: "Nishio Lab -- Research Project"
permalink: /allnews.html
---

<div class="well">
<h4>News</h4>

{% for article in site.data.news%}
{{ article.date }}
<p>{{ article.headline }}
{% if article.doi %}
<a href="https://doi.org/{{article.doi}}" target="_blank" rel="noopener noreferrer">{{article.doi}}</a>
{% elsif article.url %}
<a href="{{article.url}}" target="_blank" rel="noopener noreferrer">URL</a>
{% endif %}
</p>
{% endfor %}

</div>

