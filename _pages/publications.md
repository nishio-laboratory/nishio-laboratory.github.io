---
title: "Nishio Lab - Publications"
layout: publications
excerpt: "Nishio Lab -- Publications."
permalink: /publications/
---

# Publications
For the latest list, please see [Google Scholar](https://scholar.google.co.jp/citations?user=hHnMMMkAAAAJ&hl=ja).


## Full List
### Journals
<ol>
{% for pub in site.data.pub_journal %}
  <li>
  {{ pub.authors }}, "{{ pub.title }}," <a href="{{ pub.link.url }}">{{ pub.link.display }}</a>
  </li>
{% endfor %}
</ol>

### Letters

<ol>
{% for pub in site.data.pub_letter %}
  <li>
  {{ pub.authors }}, "{{ pub.title }}," <a href="{{ pub.link.url }}">{{ pub.link.display }}</a>
  </li>
{% endfor %}
</ol>

### International Conferences (refereed)

<ol>
{% for pub in site.data.pub_conf %}
  <li>
  {{ pub.authors }}, "{{ pub.title }}," <a href="{{ pub.link.url }}">{{ pub.link.display }}</a>
  </li>
{% endfor %}
</ol>
