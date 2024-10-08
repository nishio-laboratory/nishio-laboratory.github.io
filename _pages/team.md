---
title: "Nishio Lab - Members"
layout: gridlay
excerpt: "Nishio Lab: Team members"
sitemap: false
permalink: /member/
---

# Group Members

<!-- 
 **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**

Jump to [staff](#staff), [master and bachelor students](#master-and-bachelor-students), [alumni](#alumni), [administrative support](#administrative-support), [lab visitors](#lab-visitors).
-->

## Staff
{% assign number_printed = 0 %}
{% for member in site.data.staff %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/member_photo/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% if member.url %}
  <h4 class="mt-3"><a href="{{member.url}}">{{ member.name }}</a></h4>
  {% else %}
  <h4 class="mt-3">{{ member.name }}</h4>
  {% endif %}
  <i>{{ member.info }} <br>email: <{{ member.email }}></i>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


## Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/member_photo/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% if member.url %}
  <h4 class="mt-3"><a href="{{member.url}}">{{ member.name }}</a></h4>
  {% else %}
  <h4 class="mt-3">{{ member.name }}</h4>
  {% endif %}
  <i>{{ member.info }} <br>email: <{{ member.email }}></i>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


## Alumni
{% assign number_printed = 0 %}
{% for member in site.data.alumni %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/member_photo/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% if member.url %}
  <h4 class="mt-3"><a href="{{member.url}}">{{ member.name }}</a></h4>
  {% else %}
  <h4 class="mt-3">{{ member.name }}</h4>
  {% endif %}
  <i>{{ member.info }} <br>email: <{{ member.email }}></i>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}