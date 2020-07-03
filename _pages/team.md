---
title: "The PhysImAls"
layout: gridlay
excerpt: "The PhysImAls: Team members"
sitemap: false
permalink: /team/
---

# The PhysImAls (Group Members)


Jump to [staff](#staff), [alumni](#alumni),
[lab affiliates](#lab-affiliates), [collaborators](#collaborators).


## Current
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.physimal }}"
       onmouseover="this.src='{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}';" 
       onmouseout="this.src='{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.physimal }}';"
       class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}


 {% if member.external_sites > 0  %}
  <div class="row">
	  {% if member.orcid  %}
	  <div class="col-sm">
	  	  <a href= "{{ member.orcid }}" target="_blank">
		  <img src="{{ site.url }}{{ site.baseurl }}/images/Orcid_icon.jpg" style="float: left; width:5%; margin-right:5%"></a>
		</div>
	  {% endif %}
	  {% if member.google_scholar  %}
  	  <div class="col-sm">
	  <a href= "{{ member.google_scholar }}" target="_blank">
		<img src="{{ site.url }}{{ site.baseurl }}/images/Google_icon.jpg" style="float: left; width:5%; margin-right:5%"></a>
		</div>
	  {% endif %}
	  {% if member.scopus  %}
	  <div class="col-sm">
	  	   <a href= "{{ member.scopus }}" target="_blank">
	       <img src="{{ site.url }}{{ site.baseurl }}/images/scopus_icon.jpg" style="float: left; width:5%; margin-right:5%"></a>
		  </div>
	  {% endif %}
	  {% if member.publons  %}
		  <div class="col-sm">
		  <a href= "{{ member.publons }}" target="_blank">
		  <img src="{{ site.url }}{{ site.baseurl }}/images/publons_icon.jpg" style="float: left; width:5%; margin-right:5%"></a>
		</div>
	  {% endif %}
	  {% if member.researchgate  %}
	  <div class="col-sm">
	  	   <a href= "{{ member.researchgate }}" target="_blank">
	       <img src="{{ site.url }}{{ site.baseurl }}/images/researchgate_icon.jpg" style="float: left; width:5%; margin-right:5%"></a>
		  </div>
	  {% endif %}
  </div>
  {% endif %}
  

  </ul>
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

## Lab Affiliates
{% assign number_printed = 0 %}
{% for member in site.data.associate_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br> email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  </ul>
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

<p> &nbsp; </p>

## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>Role: {{ member.info }}<br>email: <{{ member.email }}></i><br>
  Now {{ member.now }}
  <ul style="overflow: hidden">
  
   </ul>
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

<p> &nbsp; </p>

## Collaborators

<p>
* Dorothee Auer, University of Nottingham, UK
* Penny Gowland, University of Nottingham, UK
* Sue Franics, University of Nottingham, UK
* Thomas Okell, University of Oxford, UK
* Mark Jenkinson, University of Oxford & University of Adelaide,
Australia
* Xavier Golay, University College London, UK
* Matthias van Osch, Ledien University, Netherlands
* Matthias Günther, Fraunhofer MEVIS, Germany
* Bradley MacIntosh, Sunnybook Research Institute, Canada
&nbsp; </p>
