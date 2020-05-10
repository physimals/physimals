---
title: "CoNI Lab - Team"
layout: gridlay
excerpt: "CoNI Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members


Jump to [staff](#staff), [alumni](#alumni),
[lab affiliates](#lab-affiliates), [collaborators](#collaborators).


## Staff
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
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
  <i>Role: {{ member.info }}<br>email: <{{ member.email }}></i>

    <ul style="overflow: hidden">
    <li> Now {{ member.now }} </li>
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
  <i>Role: {{ member.info }}<br> Email: <{{ member.email }}></i>
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
* [Saad Jbabdi](https://www.win.ox.ac.uk/people/saad-jbabdi), University of Oxford, UK <br>
* [Alan Anticevic](https://medicine.yale.edu/lab/anticevic), Yale University, USA <br>
* [Matthew Glasser](https://scholar.google.com/citations?user=hqA9AugAAAAJ&hl=en), Washington University - St Louis, USA <br>
* [Stephen Smith](https://www.win.ox.ac.uk/people/stephen-smith), University of Oxford, UK <br>
* [Stephen Coombes](https://www.maths.nottingham.ac.uk/plp/pmzsc), University of Nottingham, UK <br>
* [Mark Jenkinson](https://researchers.adelaide.edu.au/profile/mark.jenkinson#my-research), University of Oxford & University of Adelaide, Australia <br>
* [Daniel Alexander](http://www0.cs.ucl.ac.uk/staff/D.Alexander), University College London, UK <br>
* [Takuya Hayashi](https://www.bdr.riken.jp/en/research/labs/hayashi-t/index.html), RIKEN, Japan <br>
* [Rogier Mars](https://www.win.ox.ac.uk/people/rogier-mars), University of Oxford, UK <br>

<p> &nbsp; </p>
