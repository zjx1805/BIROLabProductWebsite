---
title: "BIRO Lab - Products"
layout: gridlay
excerpt: "BIRO Lab -- Products."
sitemap: false
permalink: /products
---

# Products

Jump to [exoskeletons](#exoskeletons), [actuators](#actuators), [sensors](#sensors). 

## Exoskeletons

{% assign number_printed = 0 %}
{% for product in site.data.exoskeletonList %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if product.highlight == 1 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well product-listing">
  <productTitle>{{ product.title }}</productTitle>
  <a href="{{ site.url }}{{ site.baseurl }}{{ product.link.url }}">
    <img src="{{ site.url }}{{ site.baseurl }}/images/productImages/{{ product.image }}" class="img-responsive" width="33%" style="float: left" />
  </a>
  <p class="product_short_description">{{ product.description }}</p>
  {% for data in product.data %}
  <p class="product_short_description"> {{data[0]}}: {{data[1]}} </p>
  {% endfor %}
  <!-- <p><strong><a href="{{ site.url }}{{ site.baseurl }}{{ product.link.url }}">{{ product.link.display }}</a></strong></p> -->
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
{% for product in site.data.actuatorList %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if product.highlight == 1 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well product-listing">
  <productTitle>{{ product.title }}</productTitle>
  <a href="{{ site.url }}{{ site.baseurl }}{{ product.link.url }}">
    <img src="{{ site.url }}{{ site.baseurl }}/images/productImages/{{ product.image }}" class="img-responsive" width="33%" style="float: left" />
  </a>
  <p class="product_short_description">{{ product.description }}</p>
  {% for data in product.data %}
  <p class="product_short_description"> {{data[0]}}: {{data[1]}} </p>
  {% endfor %}
  <!-- <p><strong><a href="{{ site.url }}{{ site.baseurl }}{{ product.link.url }}">{{ product.link.display }}</a></strong></p> -->
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

## Sensors

{% assign number_printed = 0 %}
{% for product in site.data.sensorList %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if product.highlight == 1 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well product-listing">
  <productTitle>{{ product.title }}</productTitle>
  <a href="{{ site.url }}{{ site.baseurl }}{{ product.link.url }}">
    <img src="{{ site.url }}{{ site.baseurl }}/images/productImages/{{ product.image }}" class="img-responsive" width="33%" style="float: left" />
  </a>
  <p class="product_short_description">{{ product.description }}</p>
  {% for data in product.data %}
  <p class="product_short_description"> {{data[0]}}: {{data[1]}} </p>
  {% endfor %}
  <!-- <p><strong><a href="{{ site.url }}{{ site.baseurl }}{{ product.link.url }}">{{ product.link.display }}</a></strong></p> -->
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



