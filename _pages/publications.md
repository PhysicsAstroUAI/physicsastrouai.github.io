---
title: UAI Physics + Astro - Publications"
layout: gridlay
excerpt: "Physics + Astro Group at UAI"
sitemap: false
permalink: /publications/
---


# Publications

## Recent highlights

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
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


## Full Lists of publications

A full list of publications for Astrophysics@UAI can be found in the following <a href="https://ui.adsabs.harvard.edu/public-libraries/hA1Ady6dQ5qYjhUCEa3qxw">NASA ADS public library</a>.

A list of the publications for High Energy Physics can be found in this <a href="https://inspirehep.net/institutions/910504">INSPIRE institution list</a>.

A list of Condensed Matter/Material Physics/Nonelinear Physics can be found in the following <a href="https://ui.adsabs.harvard.edu/public-libraries/hCXAMso8Rzi0nXWLnLy1DQ"> NASA ADS public library</a> (this list is not complete as ADS lacks some journals in this area).

Finally, all together in a single <a href="https://ui.adsabs.harvard.edu/public-libraries/YHeqTHpvSCWXNeVjtKNgmQ">ADS library!</a>


