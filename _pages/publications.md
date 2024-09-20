---
title: "Nishio Lab - Publications"
layout: publications
excerpt: "Nishio Lab -- Publications."
permalink: /publications/
---

{% assign current_year = 2024 %}

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

# Awards obtained by students in our team
1. 第39回電気通信普及財団テレコムシステム技術学生賞, 太田翔己 2023年
1. 情報通信系優秀学生賞, 太田翔己 2024年
1. 優秀構想発表賞, 小寺奏怜 2023年
1. 学生交流会 最優秀発表賞（セッション4）, 太田翔己 2023年
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

# Books and Lecture notes
1. 西尾理志, ``無線ネットワークにおける連合機械学習,” 電子情報通信学会誌,　Vol.105, No.1, pp. 16-21, Jan. 2022.
1. 西尾理志, ``RGB-Dカメラと機械学習で無線通信品質を見る," 電子情報通信学会誌,　Vol.102, No.4, pp. 346-352, Apr. 2019.

# Patent
<b>登録特許</b><br>
<ol>
  <li>特許7350265「位置推定装置、コンピュータに実行させるためのプログラムおよびプログラムを記録したコンピュータ読み取り可能な記録媒体」2021年3月25日出願、2023年9月26日登録</li>
  <li>
    西尾 理志、守倉 正博、宮武 遼、淺井 裕介、
    特許第7369402号「学習方法、学習装置及びプログラム」2020年7月15日出願、2023年10月18日登録
  </li>
  <li>
    西尾 理志、角南 智也、板原 壮平、矢野 一人、特許第7243993号「位置推定装置、コンピュータに実行させるためのプログラムおよびプログラムを記録したコンピュータ読み取り可能な記録媒体」2021年3月25日出願、2023年3月13日登録
  </li>
  <li>特許7369402「学習方法、学習装置及びプログラム」2020年7月15日出願、</li>
  <li>
    宮武 遼、淺井 裕介、西尾 理志、三熊 智哉、守倉 正博、特許第7185878号「通信制御システム、事前学習補助装置、通信制御方法及びプログラム」2019年7月30日出願、2022年11月30日登録
  </li>
  <li>西尾 理志、鈴木 信雄、特許7272578「管理装置、コンピュータに実行させるためのプログラムおよびそのプログラムを記録したコンピュータ読み取り可能な記録媒体」2019年1月15日出願</li>
  <li>
    槙　優一、合田　卓矢、松川　尚司、犬童　拓也、西尾　理志、特許第7018630号「ユーザと端末との対応付け方法および対応付けシステム、および、端末の接続状態の管理方法および管理システム」2018年4月16日出願、2022年2月3日登録
  </li>
  <li>宮武 遼、淺井 裕介、西尾 理志、特許第7007669号「通信システム、トラヒック制御装置及びトラヒック制御方法」2018年5月30日出願、2022年1月12日登録</li>
  <li>
    西尾　理志、鈴木　信雄、特許第6999134号「管理装置、コンピュータに実行させるためのプログラムおよびそのプログラムを記録したコンピュータ読み取り可能な記録媒体 」2018年2月14日出願、2021年12月24日登録
  </li>
  <li>槙　優一、合田　卓矢、松川　尚司、犬童　拓也、西尾　理志、山中　豪、守倉　正博、特許第6915787号「通信制御装置、通信システム、通信方法、およびプログラム」平成30年9月26日出願、令和3年7月19日登録
  </li>
  <li>槙　優一、合田　卓矢、松川　尚司、犬童　拓也、西尾　理志、特許第6786041号「移動通信システム、制御装置、方法およびプログラム」2018年1月10日出願、令和2年10月30日登録
  </li>
  <li>宮武 遼、 淺井 裕介、 中平　勝也、守倉　正博、西尾　理志、江上　晃弘、特許第6792267号「無線基地局制御方法および無線基地局制御装置」2017年4月4日出願、平成30年11月15日公開、令和2年11月10日登録</li>
  <li> 宮武 遼、 淺井 裕介、 中平　勝也、守倉　正博、西尾　理志、岡本　浩尚、特許第6714279号 “通信制御方法、通信システム及び事前学習補助装置” 2017年3月2日出願、平成30年9月20日公開、令和2年6月9日登録</li>
  <li>
    西尾　理志、新保　宏之、特許第6627496号「管理装置、コンピュータに実行させるためのプログラムおよびそのプログラムを記録したコンピュータ読み取り可能な記録媒体 」2015年12月25日出願、2019年12月13日登録
  </li>
  <li>鍋谷　寿久、青木　亜秀、西尾理志、守倉正博、山本高至、特許第6628997号「無線通信装置および無線通信方法 」2015年7月23日出願、2019年12月13日登録</li>
  <li>Toshihisa Nabetani, Tsuguhide Aoki, Takayuki Nishio, Masahiro Morikura, Koji Yamamoto「Wireless
    communication device」Patent No.: US10439788B2, Date of Patent: Oct. 8, 2019.</li>
  <li>村山大輔、中平勝也、守倉正博、西尾理志、 特許第6474136号「通信装置及び無線通信方法」2016年2月23日出願、2019年2月8日登録</li>
  <li>Masahiro Morikura, Koji Yamamoto, Takayuki Nishio, Tomoyuki Sugihara, 「Communication control method and
    communication device for enabling power saving」Patent No.: US 9942844B2, Date of Patent: April 10, 2018
  </li>
  <li>山本高至、西尾理志、守倉正博、杉原智行、 特許第6081539号「通信装置及び無線通信方法」2015年8月12日出願、2017年1月27日登録</li>
</ol>

<b>出願特許</b><br>
<ol>
  <li>特願2024-038068「通信品質予測装置、通信品質予測方法、及びプログラム」出願日：2024/03/12
  </li>
  <li>特開2023-118355「通信品質予測モデル更新装置、通信品質予測モデル更新方法、および、通信品質予測モデル更新プログラム」出願日：2022/02/15</li>
  <li>特開2023-026789「通信品質予測装置、通信品質予測方法、及び、通信品質予測プログラム」出願日：2021年8月16日</li>
  <li>守倉　正博、山本　高至、西尾　理志、杉原　智行、特開2016-131312「通信制御方法、及び、通信装置」2015年1月14日出願</li>
  <li>他、出願中特許 3件</li>
</ol>

