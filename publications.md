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
  position: absolute;'>[{{ count }}]</p> <b>{{ pub.title }}</b> with {{ pub.authors }}, {{ pub.year }}{% if pub.submitted %}. <i>Submitted</i>{% endif %}. Preprints: <a href="{{ pub.arxivurl }}" target="\_blank">{{ pub.arxivcode }}</a>{% if pub.halurl %} - <a href="{{ pub.halurl }}" target="_blank"><i class="ai ai-hal ai-align-center-1x"></i></a> - {% endif %}<a href="{{  site.baseurl }}{{ pub.pdf }}" target="\_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i></a> {% if pub.accepted %}(<i>accepted for publication on {{ pub.accjourn }}</i>){% endif %}</dd>
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
  position: absolute;'>[{{ count }}]</p> <a href="{{ pub.doi }}" target="\_blank">{{ pub.title }}</a> with {{ pub.authors }}. &nbsp;<i>{{ pub.journal }}</i> <b>{{ pub.volume }}</b>, {{ pub.pages }}, {{ pub.year }}. Preprints: <a href="{{ pub.arxivurl }}" target="\_blank">{{ pub.arxivcode }}</a>{% if pub.halurl %} - <a href="{{ pub.halurl }}" target="_blank"><i class="ai ai-hal ai-align-center-1x"></i></a>{% endif %} - <a href="{{  site.baseurl }}{{ pub.pdf }}" target="\_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i></a>
  </dd>
{% assign count = count | plus: -1 %}
{% endfor %}
</dl>



### PhD Thesis

 **Statistical properties of the Euclidean random assignment problem** <br/> _Université Paris-Saclay_, 2020, 253 pages. Manuscript : [<i class="ai ai-hal" aria-hidden="true"></i>](https://tel.archives-ouvertes.fr/tel-03098672v1){:target="\_blank"} - <a href="#" target="\_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i></a><br/><br/> Advisors: [William Jalby](https://scholar.google.fr/citations?user=9m0DLJQAAAAJ&hl=fr){:target="\_blank"}, [Olivier Rivoire](https://www.college-de-france.fr/site/en-cirb/rivoire.htm){:target="\_blank"} and [Andrea Sportiello](https://lipn.univ-paris13.fr/~sportiello/index_eng.html){:target="\_blank"} <br/> PhD jury members: [Michel Ledoux](https://perso.math.univ-toulouse.fr/ledoux/){:target="\_blank"} (_président_), [Charles Bordenave](http://www.i2m.univ-amu.fr/perso/charles.bordenave/start){:target="\_blank"} (_rapporteur_), [Massimiliano Gubinelli](https://www.iam.uni-bonn.de/abteilung-gubinelli/home/){:target="\_blank"} (_rapporteur_), [Guilhem Semerjian](http://www.phys.ens.fr/~guilhem/){:target="\_blank"} (_examinateur_), [Lenka Zdeborová](http://artax.karlin.mff.cuni.cz/~zdebl9am/){:target="\_blank"} (_examinatrice_), [Sergio Caracciolo](http://pcteserver.mi.infn.it/~caraccio/){:target="\_blank"} (_invited member_)



### Co-authors

Dario Benedetto, Emanuele Caglioti, Sergio Caracciolo, Aernout C.D. van Enter, Vittorio Erba, Arnaud Le Ny, Enrico M. Malatesta, Gabriele Sicuro, Andrea Sportiello
