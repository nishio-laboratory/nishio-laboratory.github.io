---
title: "Nishio Lab - Publications"
layout: publications
excerpt: "Nishio Lab -- Publications."
permalink: /publications/
---

{% assign current_year = 2022 %}

# Publications
<p>
This list is updated almost every month, but Google scholar one is the latest perhaps. <a
  href="https://scholar.google.co.jp/citations?hl=ja&user=hHnMMMkAAAAJ&view_op=list_works&sortby=pubdate">here (Google Schoral)</a>.<br>
国内研究会は<a href="http://www.ieice.org/ken/search/index.php?search_mode=form&year=39&psort=1&pskey=author%3A%22%C0%BE%C8%F8+%CD%FD%BB%D6%22&ps2=1&layout=&lang=&term=AUTHOR">こちらから検索ください（信学会研究会ページ）</a>
</p>

## Journals
<p>
{% for year in (2011..current_year) reversed %}
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
{% for year in (2011..current_year) reversed %}
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
{% for year in (2011..current_year) reversed %}
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

## Invited and tutorial talks
<!--
<p>
{% for year in (2011..2021) reversed %}
<a href="#C{{year}}">{{ year }}</a>
{% endfor %}
</p>
-->

{% assign prev_year = 0 %}
<ol>
{% for pub in site.data.pub_tutorial %}
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

# Awards obtained by students in our team (including Morikura Lab.)
1. 第39回電気通信普及財団テレコムシステム技術学生賞, 太田翔己 2023年
1. 情報通信系優秀学生賞, 太田翔己 2024年
1. 優秀構想発表賞, 小寺奏怜 2023年
1. 2022年度 電気情報通信学会 センサネットワークとモバイルインテリジェンス研究会 優秀発表賞, 依田光仁 2023年
1. 情報通信系優秀学生賞, 陳誠 2023年
1. 情報通信系優秀学生賞, 堀川裕太郎 2023年
1. 優秀構想発表賞, 太田翔己 2022年
1. 優秀構想発表賞, 依田光仁 2022年
1. 情報通信系優秀学生賞, 太田翔己 2023年
1. 優秀構想発表賞, 陳誠 2022年
1. IEEE VTS Japan 2022 Young Researcher's Encouragement Award，太田翔己，2022年6月20日
1. IEEE VTS Japan 2022 Young Researcher's Encouragement Award，依田光仁，2022年6月20日
1. 2021年度 電気情報通信学会 センサネットワークとモバイルインテリジェンス研究会 優秀発表賞, 若手研究奨励賞, 板原壮平 2022年
1. 電気通信普及財団テレコムシステム技術学生賞, 板原壮平 2022年
1. IEEE関西支部学生研究奨励賞, 板原壮平 2022年 
1. 公益財団法人NEC C&C財団　2021年度Ｃ＆Ｃ若手優秀論文賞, 香田優介 2021年
1. IEEE LifeTech 2021 Outstanding Student Paper Awards for Oral Presentation, 仁野諒子, 2021年
1. 電気通信普及財団テレコムシステム技術学生賞, 香田優介 2021年
1. IEEE関西支部学生研究奨励賞, 香田優介 2021年
1. ICETC 2020 Best Short Paper Award，角南智也，2020年
1. IEEE VTS Japan 2020 Young Researcher's Encouragement Award，新﨑聖峰，2020年11月18日
1. IEEE VTS Japan 2020 Young Researcher's Encouragement Award，岩崎正寛，2020年11月18日
1. IEEE VTS Japan 2020 Young Researcher's Encouragement Award，板原壮平，2020年11月18日
1. IEEE VTS Japan 2020 Young Researcher's Encouragement Award，紀平悠人，2020年11月18日
1. 優秀ポスター発表賞，香田優介，IEICE RISING 2019, 2019年11月27日.
1. IEEE VTS Japan 2019 Young Researcher's Encouragement Award，清水鴻育，2019年9月23日
1. IEEE VTS Japan 2019 Young Researcher's Encouragement Award，鄧汪東，2019年4月29日
1. IEEE VTS Japan 2019 Young Researcher's Encouragement Award，三熊智哉，2019年4月29日
1. 電子情報通信学会 学術奨励賞奨励賞, 田谷 昭仁, 2019年
1. 電気通信普及財団テレコムシステム技術学生賞, 尹 博, 2019年
1. IEEE関西支部学生研究奨励賞 尹 博, 2019年
1. IEEE関西支部学生研究奨励賞 神矢翔太郎, 2019年
1. 2018年度C&C若手優秀論文賞受賞, 神矢翔太郎, 2019年
1. IEEE VTS Japan 2018 Young Researcher's Encouragement Award，中島功太，2018年8月
1. IEEE VTS Japan 2017 Young Researcher's Encouragement Award，吉川慧司，2017年9月25日
1. IEEE VTS Japan 2017 Young Researcher's Encouragement Award，山下翔大，2017年6月5日
1. IEEE VTS Japan 2017 Young Researcher's Encouragement Award，岡本浩尚，2017年6月5日
1. 京都大学教育研究振興財団 国際研究集会発表助成，山田仰，2017年
1. C&C 振興財団国際会議論文発表者助成，岡本浩尚，2017年度前期
1. 電気通信普及財団テレコムシステム技術学生賞受賞, 神矢翔太郎, "Self-Organization of Coverage of Densely Deployed WLANs Considering Outermost APs without Generating Coverage Holes"
1. IEEE関西支部学生研究奨励賞, 小熊優太, "Proactive Base Station Selection Based on Human Blockage Prediction Using RGB-D Cameras for mmWave Communications" (presented in Globecom 2015)
1. C&C 振興財団国際会議論文発表者助成，小熊優太，2015 年度後期
1. 第8回ICTイノベーション優秀研究賞, 西岡良，"広域無線LANに向けた同報通信技術" 2015年

