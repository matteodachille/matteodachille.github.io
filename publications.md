---
layout: page
title: Publications
order: 3
---
<!-- - TOC
{:toc} -->

(click on YYMM.NNNNN - <i class="ai ai-hal ai-align-center-1x"></i> - <i class="ai ai-researchgate ai-align-center-1x"></i> - <i class="ai ai-academia ai-align-center-1x"></i> - <i class="fa fa-file-pdf-o" aria-hidden="true"></i>&nbsp; to access/download preprint versions)

{% assign list_wip = site.data.pubs | where: 'upcoming', true %}
{% assign list_prep = site.data.pubs | where: 'preprint', true %}
{% assign list = site.data.pubs | where: 'published', true %}


### In preparation

<dl>
{% assign count = list_wip.size | plus: list.size | plus: list_prep.size %}
<!--{% if count != 0 %}
  ### Preprints
  {% endif %}-->
{% for pub in list_wip %}
  <dd style="margin-left: 30px;"><p style='margin-left: -30px !important;
  position: absolute;'>[{{ count }}]</p>&nbsp; {{ pub.title }} <i>with {{ pub.authors }}</i>, {{ pub.year }}</dd>
{% assign count = count | plus: -1 %}
{% endfor %}
</dl>


### Preprints

<dl>
{% assign count = list_prep.size | plus: list.size %}
<!--{% if count != 0 %}
  ### Preprints
  {% endif %}-->
{% for pub in list_prep %}
  <dd style="margin-left: 30px;"><p style='margin-left: -30px !important;
  position: absolute;'>[{{ count }}]</p> <b>{{ pub.title }}</b> with {{ pub.authors }}, {{ pub.year }}{% if pub.submitted %}. <i>Submitted</i>{% endif %}. Preprints: <a href="{{ pub.arxivurl }}" target="_blank">{{ pub.arxivcode }}</a>{% if pub.halurl %} - <a href="{{ pub.halurl }}" target="_blank"><i class="ai ai-hal ai-align-center-1x"></i></a>{% endif %}{% if pub.rg %} - <a href="https://www.researchgate.net/publication/{{ pub.rg }}" target="_blank"><i class="ai ai-researchgate ai-align-center-1x"></i></a>{% endif %}{% if pub.academia %} - <a href="https://www.academia.edu/{{ pub.academia }}" target="_blank"><i class="ai ai-academia ai-align-center-1x"></i></a>{% endif %} - <a href="{{  site.baseurl }}{{ pub.pdf }}" target="_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i></a> {% if pub.accepted %}(<i>accepted for publication on {{ pub.accjourn }}</i>){% endif %}</dd>
{% assign count = count | plus: -1 %}
{% endfor %}
</dl>

### Published in peer reviewed journals
<dl>
{% assign list = site.data.pubs | where: 'published', true %}
{% assign count = list.size %}
{% for pub in list %}
  <!--dt>  {{ pub.title }} with {{ pub.authors }}
  </dt-->
  <dd style="margin-left: 30px;"><p style='margin-left: -30px !important;
  position: absolute;'>[{{ count }}]</p> <a href="{{ pub.doi }}" target="_blank">{{ pub.title }}</a> with {{ pub.authors }}. &nbsp;<i>{{ pub.journal }}</i> <b>{{ pub.volume }}</b>, {{ pub.pages }}, {{ pub.year }}. Preprints: <a href="{{ pub.arxivurl }}" target="_blank">{{ pub.arxivcode }}</a>{% if pub.halurl %} - <a href="{{ pub.halurl }}" target="_blank"><i class="ai ai-hal ai-align-center-1x"></i></a>{% endif %}{% if pub.rg %} - <a href="https://www.researchgate.net/publication/{{ pub.rg }}" target="_blank"><i class="ai ai-researchgate ai-align-center-1x"></i></a>{% endif %}{% if pub.academia %} - <a href="https://www.academia.edu/{{ pub.academia }}" target="_blank"><i class="ai ai-academia ai-align-center-1x"></i></a>{% endif %} - <a href="{{  site.baseurl }}{{ pub.pdf }}" target="_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i></a>
  </dd>
{% assign count = count | plus: -1 %}
{% endfor %}
</dl>


### PhD Thesis


 **Statistical properties of the Euclidean random assignment problem** <br/> _Université Paris-Saclay_, 2020, 253 pages. Manuscript : [<i class="ai ai-hal" aria-hidden="true"></i>](https://tel.archives-ouvertes.fr/tel-03098672v1){:target="_blank"} - [<i class="ai ai-researchgate ai-align-center-1x" aria-hidden="true"></i>](https://www.researchgate.net/publication/348317683_Statistical_Properties_of_the_Euclidean_Random_Assignment_Problem){:target="_blank"} - <a href="#" target="_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i></a><br/><br/> Co-Directors: [William Jalby](https://scholar.google.fr/citations?user=9m0DLJQAAAAJ&hl=fr){:target="_blank"}, [Olivier Rivoire](https://www.college-de-france.fr/site/en-cirb/rivoire.htm){:target="_blank"} and [Andrea Sportiello](https://lipn.univ-paris13.fr/~sportiello/index_eng.html){:target="_blank"} <br/> PhD jury members: [Michel Ledoux](https://perso.math.univ-toulouse.fr/ledoux/){:target="_blank"} (_président_), [Charles Bordenave](http://www.i2m.univ-amu.fr/perso/charles.bordenave/start){:target="_blank"} (_rapporteur_), [Massimiliano Gubinelli](https://www.iam.uni-bonn.de/abteilung-gubinelli/home/){:target="_blank"} (_rapporteur_), [Guilhem Semerjian](http://www.phys.ens.fr/~guilhem/){:target="_blank"} (_examinateur_), [Lenka Zdeborová](http://artax.karlin.mff.cuni.cz/~zdebl9am/){:target="_blank"} (_examinatrice_), [Sergio Caracciolo](http://pcteserver.mi.infn.it/~caraccio/){:target="_blank"} (_membre invité_)

### Other documents
#### MSc Thesis

   **On two linear assignment problems: random assignment and Euclidean bipartite matching** <br/>
   University of Milan, 2016. Manuscript: [<i class="ai ai-researchgate ai-align-center-1x" aria-hidden="true"></i>](http://dx.doi.org/10.13140/RG.2.1.1725.2082){:target="_blank"} - [<i class="ai ai-academia ai-align-center-1x" aria-hidden="true"></i>](https://www.academia.edu/25062627/On_Two_Linear_Assignment_Problems_Random_Assignment_and_Euclidean_Bipartite_Matching){:target="_blank"} - [<i class="fa fa-file-pdf-o" aria-hidden="true"></i>]({{ site.baseurl }}downloads/masterthesis.pdf){:target="_blank"} <br/>
 Supervisor: [Sergio Caracciolo](http://pcteserver.mi.infn.it/~caraccio/){:target="_blank"} <br/>
 External rapporteur: [Gabriele Sicuro](https://gabrielesicuro.wordpress.com/){:target="_blank"}

#### BSc Thesis

 **La teoria di Schwarz-Christoffel e il Biliardo Quantistico Poligonale** <br/>
 University of Milan, 2012. Manuscript (in italian): [<i class="ai ai-researchgate ai-align-center-1x" aria-hidden="true"></i>](http://dx.doi.org/10.13140/RG.2.1.2101.6403){:target="_blank"} - [<i class="ai ai-academia ai-align-center-1x" aria-hidden="true"></i>](https://www.academia.edu/2506378/La_Teoria_di_Schwarz_Christoffel_e_il_Biliardo_Quantistico_Poligonale){:target="_blank"} - [<i class="fa fa-file-pdf-o" aria-hidden="true"></i>]({{ site.baseurl }}downloads/bscthesis.pdf){:target="_blank"}<br/>
 Supervisor: [Luca Guido Molinari](http://wwwteor.mi.infn.it/~molinari/){:target="_blank"}



<br/>

### Co-authors webpages


 <!--
 Previous version
 Dario Benedetto, Emanuele Caglioti, Sergio Caracciolo, Aernout C.D. van Enter, Vittorio Erba, Arnaud Le Ny, Enrico M. Malatesta, Gabriele Sicuro, Andrea Sportiello
 -->

 [Dario Benedetto](http://brazil.mat.uniroma1.it/dario/){:target="_blank"}, [Emanuele Caglioti](https://sites.google.com/site/ecaglioti/){:target="_blank"}, [Sergio Caracciolo](http://pcteserver.mi.infn.it/~caraccio/){:target="_blank"}, [Aernout C.D. van Enter](http://www.math.rug.nl/~aenter/){:target="_blank"}, [Vittorio Erba](https://vittorioerba.github.io/){:target="_blank"}, [Arnaud Le Ny](https://perso.math.u-pem.fr/le_ny.arnaud/){:target="_blank"}, [Enrico M. Malatesta](https://www.artlab.unibocconi.eu/wps/wcm/connect/cdr/artlab/home/people/students+and+postdocs/enrico+malatesta){:target="_blank"}, [Gabriele Sicuro](https://gabrielesicuro.wordpress.com/){:target="_blank"}, [Andrea Sportiello](https://lipn.univ-paris13.fr/~sportiello/index_eng.html){:target="_blank"}
