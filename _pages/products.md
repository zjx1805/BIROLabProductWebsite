---
title: "BIRO Lab - Products"
layout: gridlay
excerpt: "BIRO Lab -- Products."
sitemap: false
permalink: /products
---

# Products

Jump to [sensors](#sensors), [actuators](#actuators), [exoskeletons](#exoskeletons). 

## Sensors

{% assign number_printed = 0 %}
{% for product in site.data.productList %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if product.highlight == 1 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <productTitle>{{ product.title }}</productTitle>
  <img src="{{ site.url }}{{ site.baseurl }}/images/productImages/{{ product.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ product.description }}</p>
  {% for data in product.data %}
  <p> {{data[0]}}: {{data[1]}} </p>
  {% endfor %}
  <p><strong><a href="{{ site.url }}{{ site.baseurl }}{{ product.link.url }}">{{ product.link.display }}</a></strong></p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}

</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}

</div>
{% endif %}

<p> &nbsp; </p>

## Actuators

{% assign number_printed = 0 %}
{% for product in site.data.productList %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if product.highlight == 1 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <productTitle>{{ product.title }}</productTitle>
  <img src="{{ site.url }}{{ site.baseurl }}/images/productImages/{{ product.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ product.description }}</p>
  {% for data in product.data %}
  <p> {{data[0]}}: {{data[1]}} </p>
  {% endfor %}
  <p><strong><a href="{{ product.link.url }}">{{ product.link.display }}</a></strong></p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}

</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}

</div>
{% endif %}

<p> &nbsp; </p>

## Exoskeletons

{% assign number_printed = 0 %}
{% for product in site.data.productList %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if product.highlight == 1 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <productTitle>{{ product.title }}</productTitle>
  <img src="{{ site.url }}{{ site.baseurl }}/images/productImages/{{ product.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ product.description }}</p>
  {% for data in product.data %}
  <p> {{data[0]}}: {{data[1]}} </p>
  {% endfor %}
  <p><strong><a href="{{ product.link.url }}">{{ product.link.display }}</a></strong></p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}

</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}

</div>
{% endif %}

<p> &nbsp; </p>