---
title: "Dong Lab -- Publications"
layout: gridlay
excerpt: "Dong Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

## Group highlights

**At the end of this page, you can find the full list of [publications](#full-list-of-publications) and [conferences](#conferences).**

{% for number_printed in (1..10) %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == number_printed %}

{% if even_odd == 1 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% if even_odd == 0 %}
</div>
{% endif %}

{% endif %}
{% endfor %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Full List of publications

{% assign index = 0 %}

{% for publi in site.data.publist %}

  {% assign index = index | plus: 1 %}

  {{index}}. {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}


## Conferences

{% assign index = 0 %}

{% for conf in site.data.conflist %}

  {% assign index = index | plus: 1 %}

  {{index}}. {{ conf.title }} <br />
  <em>{{ conf.authors }} </em><br/> <a href="{{ conf.link.url}}">{{ conf.link.display }}</a>

{% endfor %}
