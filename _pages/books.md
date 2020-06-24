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

This primer gives a general and accessible introduction to the wide array of MRI-based neuroimaging methods that are used in research. Supplemented with online datasets and examples to enable the reader to obtain hands-on experience working with real data, it provides a practical and approachable introduction for those new to the neuroimaging field. The text also covers the fundamentals of what different MRI modalities measure, what artifacts commonly occur, the essentials of the analysis, and common 'pipelines' including brain extraction, registration and segmentation.

<div style="clear: both;"></div>

<img src="{{ site.url }}{{ site.baseurl }}/images/bookpic/nip2.png" class="img-responsive" width="10%" style="float: left" />

**Introduction to Perfusion Quantification using Arterial Spin Labelling**

*Michael Chappell, Thomas Okell, Brad Macintosh*

The aim of this primer is to equip someone new to the field of perfusion imaging and ASL with the knowledge not only to make good choices about ASL acquisition and analysis, but also to understand what choices they are making and why. Examples of analysis applied to real data are given throughout the text and instructions on how to reproduce the analyses are illustrated on the primer website.

<div style="clear: both;"></div>

<img src="{{ site.url }}{{ site.baseurl }}/images/bookpic/nip3.png" class="img-responsive" width="10%" style="float: left" />

**Introduction to Resting State fMRI Functional Connectivity**

*Janine Bijsterbosch, Stephen Smith, Christian Beckmann*

From data acquisition to interpretation of results, Introduction to Resting State fMRI Functional Connectivity discusses a wide range of approaches without requiring any previous knowledge of resting state fMRI, making it highly accessible to readers from a broad range of backgrounds.

<div style="clear: both;"></div>

### Physiology for Engineers series

<img src="{{ site.url }}{{ site.baseurl }}/images/bookpic/pfe.png" class="img-responsive" width="10%" style="float: left" />

[**Physiology for Engineers**](https://www.physiologyforengineers.org)

*Michael Chappell, Stephen Payne*

An introduction to qualitative 
and quantitative aspects of human physiology using mathematical principles and engineering methods that will be familiar to engineers 
and other physical scientists.

<div style="clear: both;"></div>

<img src="{{ site.url }}{{ site.baseurl }}/images/bookpic/mie.png" class="img-responsive" width="10%" style="float: left" />

[**Principles of Medical Imaging for Engineers**](https://www.physiologyforengineers.org)

*Michael Chappell*

**Coming Soon!** An introduction to the principles of medical imaging that underpin all of the major medical imaging methods. By first considering how to get signals from within the body, and then how to turn these into images, this book shows how mathematical and physics principles work in the context of medical imaging. 

<div style="clear: both;"></div>

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
  <img src="{{ site.url }}{{ site.baseurl }}/images/bookpic/{{ publi.image }}" class="img-responsive" width="25%" style="float: left" />
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
