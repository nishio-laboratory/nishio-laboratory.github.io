---
title: "Nishio Lab - Publications"
layout: publications
excerpt: "Nishio Lab -- Publications."
permalink: /publications/
---

# Publications
<p>
This list is updated almost every month, but Google scholar one is the latest perhaps. <a
  href="https://scholar.google.co.jp/citations?hl=ja&user=hHnMMMkAAAAJ&view_op=list_works&sortby=pubdate">here (Google Schoral)</a>.<br>
国内研究会は<a href="http://www.ieice.org/ken/search/index.php?search_mode=form&year=39&psort=1&pskey=author%3A%22%C0%BE%C8%F8+%CD%FD%BB%D6%22&ps2=1&layout=&lang=&term=AUTHOR">こちらから検索ください（信学会研究会ページ）</a>
</p>

## Journals
<p>
{% for year in (2011..2021) reversed %}
<a href="#J{{year}}">{{ year }}</a>
{% endfor %}
</p>

{% assign prev_year = 0 %}
<ol>
{% for pub in site.data.pub_journal %}
  {% if pub.year != prev_year %}
  <li id="J{{ pub.year }}">
  {% else %}
  <li>
  {% endif %}
  {% if pub.url %}
  {{ pub.authors }}, "{{ pub.title }}," <a href="{{ pub.url }}">{{ pub.journal }}</a>
  {% elsif pub.doi %}
  {{ pub.authors }}, "{{ pub.title }}," <a href="https://doi.org/{{ pub.doi }}">{{ pub.journal }}</a>
  {% else %}
  {{ pub.authors }}, "{{ pub.title }}," {{ pub.journal }}
  {% endif %}
  </li>
  {% assign prev_year = pub.year %}
{% endfor %}
</ol>

## Letters

<p>
{% for year in (2011..2021) reversed %}
<a href="#L{{year}}">{{ year }}</a>
{% endfor %}
</p>

{% assign prev_year = 0 %}
<ol>
{% for pub in site.data.pub_letter %}
  {% if pub.year != prev_year %}
  <li id="L{{ pub.year }}">
  {% else %}
  <li>
  {% endif %}
  {% if pub.url %}
  {{ pub.authors }}, "{{ pub.title }}," <a href="{{ pub.url }}">{{ pub.journal }}</a>
  {% elsif pub.doi %}
  {{ pub.authors }}, "{{ pub.title }}," <a href="https://doi.org/{{ pub.doi }}">{{ pub.journal }}</a>
  {% else %}
  {{ pub.authors }}, "{{ pub.title }}," {{ pub.journal }}
  {% endif %}
  </li>
  {% assign prev_year = pub.year %}
{% endfor %}
</ol>

## International Conferences (refereed)

<p>
{% for year in (2011..2021) reversed %}
<a href="#C{{year}}">{{ year }}</a>
{% endfor %}
</p>

{% assign prev_year = 0 %}
<ol>
{% for pub in site.data.pub_conf %}
  {% if pub.year != prev_year %}
  <li id="C{{ pub.year }}">
  {% else %}
  <li>
  {% endif %}
  {% if pub.url %}
  {{ pub.authors }}, "{{ pub.title }}," <a href="{{ pub.url }}">{{ pub.journal }}</a>
  {% elsif pub.doi %}
  {{ pub.authors }}, "{{ pub.title }}," <a href="https://doi.org/{{ pub.doi }}">{{ pub.journal }}</a>
  {% else %}
  {{ pub.authors }}, "{{ pub.title }}," {{ pub.journal }}
  {% endif %}
  </li>
  {% assign prev_year = pub.year %}
{% endfor %}
</ol>