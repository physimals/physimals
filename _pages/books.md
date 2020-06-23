---
title: "Physimals - Books"
layout: gridlay
excerpt: "Physimals -- Books."
sitemap: false
permalink: /books/
---

# Complete Books

### Neuroimaging Primers

[Oxford Neuroimaging Primers](http://www.neuroimagingprimers.org/") are a set of short, accessible 
textbooks focused on MRI-based neuroimaging research, published by Oxford University Press.

<img src="{{ site.url }}{{ site.baseurl }}/images/bookpic/nip1.png" class="img-responsive" width="10%" style="float: left" />
**Introduction to Neuroimaging Analysis**
*Mark Jenkinson, Michael Chappell*

<p> &nbsp; </p>

<img src="{{ site.url }}{{ site.baseurl }}/images/bookpic/nip2.png" class="img-responsive" width="10%" style="float: left" />
**Introduction to Perfusion Quantification using Arterial Spin Labelling**
*Michael Chappell, Thomas Okell, Brad Macintosh*

<p> &nbsp; </p>

<img src="{{ site.url }}{{ site.baseurl }}/images/bookpic/nip3.png" class="img-responsive" width="10%" style="float: left" />
**Introduction to Resting State fMRI Functional Connectivity**
*Janine Bijsterbosch, Stephen Smith, Christian Beckmann*

<p> &nbsp; </p>

### Physiology for Engineers

<img src="{{ site.url }}{{ site.baseurl }}/images/bookpic/pfe.png" class="img-responsive" width="10%" style="float: left" />
[**Physiology for Engineers**](https://www.physiologyforengineers.org)

An introduction to qualitative 
and quantitative aspects of human physiology using mathematical principles and engineering methods that will be familiar to engineers 
and other physical scientists.

*Michael Chappell, Stephen Payne*

<p> &nbsp; </p>

# Book chapters

{% assign number_printed = 0 %}
{% for publi in site.data.books %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.fullbook == 0 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}" target="_blank">{{ publi.link.display }}</a></strong></p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

<p> &nbsp; </p>
