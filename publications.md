---
layout: page
title: Publications
order: 3
---
<!-- - TOC
{:toc} -->

(click on <i class="fa fa-file-pdf-o" aria-hidden="true"></i> to download preprint files)

### In preparation

<dl>
{% assign list = site.data.pubs | where: 'upcoming', true %}
{% assign count = list.size %}
<!--{% if count != 0 %}
  ### Preprints
  {% endif %}-->
{% for pub in list %}
  <dd style="margin-left: 30px;"><p style='margin-left: -30px !important;
  position: absolute;'>[{{ count }}]</p> {{ pub.title }} <i>with {{ pub.authors }}</i>, {{ pub.year }}</dd>
{% assign count = count | plus: -1 %}
{% endfor %}
</dl>


### Preprints

<dl>
{% assign list = site.data.pubs | where: 'preprint', true %}
{% assign count = list.size %}
<!--{% if count != 0 %}
  ### Preprints
  {% endif %}-->
{% for pub in list %}
  <dd style="margin-left: 30px;"><p style='margin-left: -30px !important;
  position: absolute;'>[{{ count }}]</p> <b>{{ pub.title }}</b> with {{ pub.authors }}. Preprint: <a href="{{ pub.arxivurl }}" target="\_blank"> arXiv: {{ pub.arxivcode }}</a>, {{ pub.year }}&nbsp;<a href="{{  site.baseurl }}{{ pub.pdf }}" target="\_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i></a> {% if pub.submitted %}(<i>accepted</i>){% endif %} {% if pub.accepted %}(<i>accepted for publication on {{ pub.accjourn }}</i>){% endif %}</dd>
{% assign count = count | plus: -1 %}
{% endfor %}
</dl>

### Published
<dl>
{% assign list = site.data.pubs | where: 'published', true %}
{% assign count = list.size %}
{% for pub in list %}
  <!--dt>  {{ pub.title }} with {{ pub.authors }}
  </dt-->
  <dd style="margin-left: 30px;"><p style='margin-left: -30px !important;
  position: absolute;'>[{{ count }}]</p> <a href="{{ pub.doi }}" target="\_blank">{{ pub.title }}</a> with {{ pub.authors }}. &nbsp;<i>{{ pub.journal }}</i> <b>{{ pub.volume }}</b>, {{ pub.pages }}, {{ pub.year }}&nbsp; <a href="{{  site.baseurl }}{{ pub.pdf }}" target="\_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i></a></dd>
{% assign count = count | plus: -1 %}
{% endfor %}
</dl>

<!--
v2 with n. of papers
### Co-authors (\# joint papers)

Dario Benedetto (1), Emanuele Caglioti (1), Sergio Caracciolo (5), Aernout C.D. van Enter (1), Vittorio Erba (1), Arnaud Le Ny (2), Enrico M. Malatesta (1), Gabriele Sicuro (4), Andrea Sportiello (4)
-->

### Co-authors

Dario Benedetto, Emanuele Caglioti, Sergio Caracciolo, Aernout C.D. van Enter, Vittorio Erba, Arnaud Le Ny, Enrico M. Malatesta, Gabriele Sicuro, Andrea Sportiello
