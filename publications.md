---
layout: page
title: Publications
order: 1
---
<!-- - TOC
{:toc} -->

(Links on titles go at journal versions. Click on YYMM.NNNNN - <i class="ai ai-hal ai-align-center-1x"></i> - <i class="ai ai-researchgate ai-align-center-1x"></i> - <i class="ai ai-academia ai-align-center-1x"></i> - <i class="fa fa-file-pdf-o" aria-hidden="true"></i>&nbsp; to access/download preprints)
{: style="font-size: 15.5px; margin-left: 0px" }

{% assign list_wip = site.data.pubs | where: 'upcoming', true %}
{% assign list_prep = site.data.pubs | where: 'preprint', true %}
{% assign list = site.data.pubs | where: 'published', true %}

<div style="height:0.25em;"></div>

#### Preprints
<div style="height:0.5em;"></div>

<dl>
{% assign count = list_prep.size | plus: list.size %}
<!--{% if count != 0 %}
  ### Preprints
  {% endif %}-->
{% for pub in list_prep %}
<dd style="margin-left:0; display:flex; align-items:baseline;margin-bottom:16px;">
    <span style="width:30px; margin-left:-30px; margin-right:5px;text-align:right; font-size:11.5pt; flex-shrink:0;">
        {{ count }}.
    </span>
    <div>
      <b style="font-size:13.5pt;">{{ pub.title }}</b><br/>
      {% if pub.authors %}
      <span style="font-size:12.5pt;">with {{ pub.authors }}.</span>
    {% endif %}
  <span style="font-size:12pt;"><a href="{{ pub.arxivurl }}" target="_blank">{{ pub.arxivcode }}</a>{% if pub.halurl %} - <a href="{{ pub.halurl }}" target="_blank"><i class="ai ai-hal ai-align-center-1x"></i></a>{% endif %}{% if pub.rg %} - <a href="https://www.researchgate.net/publication/{{ pub.rg }}" target="_blank"><i class="ai ai-researchgate ai-align-center-1x"></i></a>{% endif %}{% if pub.academia %} - <a href="https://www.academia.edu/{{ pub.academia }}" target="_blank"><i class="ai ai-academia ai-align-center-1x"></i></a>{% endif %} - <a href="{{  site.baseurl }}{{ pub.pdf }}" target="_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i></a></span> {% if pub.submitted %}
  <span style="font-size:12.5pt;margin-left:5px;"><i>Submitted</i></span>
  {% endif %}
  <br/>
{% if pub.abstract %}
  <details>
    <summary style="font-size:11.5pt;"><i>Abstract</i> </summary>
    <p style="font-size:11pt;">{{ pub.abstract }}</p>
    </details>
{% endif %}
{% if pub.accepted %}Accepted on <i>{{ pub.accjourn }}</i><br/>{% endif %}
  </div>
  <br/>
</dd>
{% assign count = count | plus: -1 %}
{% endfor %}
</dl>

<div style="height:0.75em;"></div>

#### Published in peer reviewed journals
<div style="height:0.5em;"></div>
<dl>
{% assign list = site.data.pubs | where: 'published', true %}
{% assign count = list.size %}
{% for pub in list %}

<dd style="margin-left:0; margin-bottom:1em; display:flex; align-items:baseline;">
    <span style="width:30px; margin-left:-30px; margin-right:5px; text-align:right; font-size:11.5pt; flex-shrink:0;">
        {{ count }}.
    </span>

    <div>
        <a href="{{ pub.doi }}" target="_blank" style="color:#4169e1; font-size:13.5pt;">
            {{ pub.title }}
        </a><br/>

        {% if pub.authors %}
        <span style="font-size:12.5pt;">
            with {{ pub.authors }}.
        </span>
        {% endif %}

        <span style="font-size:12.5pt;">
            <b>{{ pub.journal }}</b>
            {% if pub.volume %} {{ pub.volume }}{% endif %}
            {% if pub.pages %}, {{ pub.pages }}{% endif %}
            {% if pub.year %}, {{ pub.year }}{% endif %}.
        </span>
        <br/>
        <span style="font-size:12pt;">
            <a href="{{ pub.arxivurl }}" target="_blank">{{ pub.arxivcode }}</a>

            {% if pub.halurl %}
            - <a href="{{ pub.halurl }}" target="_blank">
                <i class="ai ai-hal ai-align-center-1x"></i>
              </a>
            {% endif %}

            {% if pub.rg %}
            - <a href="https://www.researchgate.net/publication/{{ pub.rg }}" target="_blank">
                <i class="ai ai-researchgate ai-align-center-1x"></i>
              </a>
            {% endif %}

            {% if pub.academia %}
            - <a href="https://www.academia.edu/{{ pub.academia }}" target="_blank">
                <i class="ai ai-academia ai-align-center-1x"></i>
              </a>
            {% endif %}

            - <a href="{{ site.baseurl }}{{ pub.pdf }}" target="_blank">
                <i class="fa fa-file-pdf-o" aria-hidden="true"></i>
              </a>
        </span>

        {% if pub.abstract %}
        <details>
            <summary style="font-size:11.5pt;"><i>Abstract</i></summary>
            <p style="font-size:11pt;">{{ pub.abstract }}</p>
        </details>
        {% endif %}


    </div>
</dd>




  {% assign count = count | plus: -1 %}
{% endfor %}
</dl>


<!--
### In preparation

<dl>
{% assign count = list_wip.size | plus: list.size | plus: list_prep.size %}
{% if count != 0 %}
  ### Preprints
  {% endif %}

{% for pub in list_wip %}
  <dd style="margin-left: 30px;"><p style='margin-left: -30px !important;
  position: absolute;'>[{{ count }}]</p>&nbsp; {{ pub.title }} <i>with {{ pub.authors }}</i>, {{ pub.year }}</dd>
{% assign count = count | plus: -1 %}
{% endfor %}
</dl>
-->

<br/>

#### Co-authors

(chronological order)
{: style="font-size: 15.5px; margin-left: 0px" }

[Sergio Caracciolo](http://pcteserver.mi.infn.it/~caraccio/){:target="_blank"}, [Gabriele Sicuro](https://gsicuro.github.io/){:target="_blank"}, [Enrico M. Malatesta](https://didattica.unibocconi.eu/docenti/cv.php?rif=227138&cognome=MALATESTA&nome=ENRICO_MARIA){:target="_blank"}, [Vittorio Erba](https://vittorioerba.github.io/){:target="_blank"}, [Andrea Sportiello](https://lipn.univ-paris13.fr/~sportiello/index_eng.html){:target="_blank"},
 [Dario Benedetto](http://brazil.mat.uniroma1.it/dario/){:target="_blank"}, [Emanuele Caglioti](https://sites.google.com/site/ecaglioti/){:target="_blank"}, [Arnaud Le Ny](https://perso.math.u-pem.fr/leny.arnaud/){:target="_blank"}, [Aernout C.D. van Enter](http://www.math.rug.nl/~aenter/){:target="_blank"}, [Nicolas Curien](https://www.imo.universite-paris-saclay.fr/~nicolas.curien/){:target="_blank"}, [Nathanaël Enriquez](https://www.imo.universite-paris-saclay.fr/~nathanael.enriquez/){:target="_blank"}, [Russell Lyons](https://rdlyons.pages.iu.edu/){:target="_blank"}, [Meltem Ünel](https://sites.google.com/view/meltemunel/main){:target="_blank"}, [Paul Melotti](https://www.imo.universite-paris-saclay.fr/~paul.melotti/){:target="_blank"}, [Vanessa Jacquier](https://research-portal.uu.nl/en/persons/vanessa-jacquier/){:target="_blank"}, [Wioletta M. Ruszel](https://www.uu.nl/staff/WMRuszel){:target="_blank"}, [Loren Coquille](https://www-fourier.ujf-grenoble.fr/~coquilll/){:target="_blank"}, [Jan Grebík](https://grebikj.github.io/){:target="_blank"}, [Ali Khezeli](https://scholar.google.com/citations?user=rPXh3bAAAAAJ&hl=en){:target="_blank"}, [Konstantin Recke](https://sites.google.com/view/konstantin-recke/){:target="_blank"}, [Amanda Wilkens](https://www.math.cmu.edu/~awilkens/){:target="_blank"}, [Francesco Mattesini](https://francescomattesini.github.io/){:target="_blank"}, [Dario Trevisan](https://web.dm.unipi.it/trevisan/it/){:target="_blank"}, [Christoph Thäle](https://sites.google.com/view/christophthaele){:target="_blank"}
 {: style="font-size: 16.5px; margin-left: 0px" }


<br/>

### Other documents

#### PhD Thesis


 **Statistical properties of the Euclidean random assignment problem** <br/> 2020, Université Paris-Saclay. Manuscript: [<i class="ai ai-hal" aria-hidden="true"></i>](https://tel.archives-ouvertes.fr/tel-03098672v1){:target="_blank"} - [<i class="ai ai-researchgate ai-align-center-1x" aria-hidden="true"></i>](https://www.researchgate.net/publication/348317683_Statistical_Properties_of_the_Euclidean_Random_Assignment_Problem){:target="_blank"} - <a href="#" target="_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i></a><br/>
 Co-Directors: [William Jalby](https://scholar.google.fr/citations?user=9m0DLJQAAAAJ&hl=fr){:target="_blank"}, [Olivier Rivoire](https://www.college-de-france.fr/site/en-cirb/rivoire.htm){:target="_blank"} and [Andrea Sportiello](https://lipn.univ-paris13.fr/~sportiello/index_eng.html){:target="_blank"} <br/> Jury: [Michel Ledoux](https://en.wikipedia.org/wiki/Michel_Ledoux){:target="_blank"} (_président_), [Charles Bordenave](http://www.i2m.univ-amu.fr/perso/charles.bordenave/start){:target="_blank"} (_rapporteur_), [Massimiliano Gubinelli](https://www.maths.ox.ac.uk/people/massimiliano.gubinelli){:target="_blank"} (_rapporteur_), [Guilhem Semerjian](http://www.phys.ens.fr/~guilhem/){:target="_blank"} (_examinateur_), [Lenka Zdeborová](https://en.wikipedia.org/wiki/Lenka_Zdeborov%C3%A1){:target="_blank"} (_examinatrice_), [Sergio Caracciolo](http://pcteserver.mi.infn.it/~caraccio/){:target="_blank"} (_membre invité_)
{: style="font-size: 16.5px; margin-left: 0px" }


#### MSc Thesis

   **On two linear assignment problems: random assignment and Euclidean bipartite matching** <br/>
   2016, University of Milan. Manuscript: [<i class="ai ai-researchgate ai-align-center-1x" aria-hidden="true"></i>](http://dx.doi.org/10.13140/RG.2.1.1725.2082){:target="_blank"} - [<i class="ai ai-academia ai-align-center-1x" aria-hidden="true"></i>](https://www.academia.edu/25062627/On_Two_Linear_Assignment_Problems_Random_Assignment_and_Euclidean_Bipartite_Matching){:target="_blank"} - [<i class="fa fa-file-pdf-o" aria-hidden="true"></i>]({{ site.baseurl }}downloads/masterthesis.pdf){:target="_blank"} <br/>
 Supervisor: [Sergio Caracciolo](http://pcteserver.mi.infn.it/~caraccio/){:target="_blank"} <br/>
 External rapporteur: [Gabriele Sicuro](https://gsicuro.github.io/){:target="_blank"}
 {: style="font-size: 16.5px; margin-left: 0px" }

#### BSc Thesis

 **La teoria di Schwarz-Christoffel e il Biliardo Quantistico Poligonale** <br/>
 2012, University of Milan. Manuscript (in italian): [<i class="ai ai-researchgate ai-align-center-1x" aria-hidden="true"></i>](http://dx.doi.org/10.13140/RG.2.1.2101.6403){:target="_blank"} - [<i class="ai ai-academia ai-align-center-1x" aria-hidden="true"></i>](https://www.academia.edu/2506378/La_Teoria_di_Schwarz_Christoffel_e_il_Biliardo_Quantistico_Poligonale){:target="_blank"} - [<i class="fa fa-file-pdf-o" aria-hidden="true"></i>]({{ site.baseurl }}downloads/bscthesis.pdf){:target="_blank"}<br/>
 Supervisor: [Luca Guido Molinari](http://wwwteor.mi.infn.it/~molinari/){:target="_blank"}
{: style="font-size: 16.5px; margin-left: 0px" }
