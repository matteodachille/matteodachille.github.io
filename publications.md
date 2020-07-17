---
layout: page
title: Publications
order: 3
---
<!-- - TOC
{:toc} -->

<!--
### Preprints

[5] **Random assignment problems on 2d manifolds**
: with Dario Benedetto, Emanuele Caglioti, Sergio Caracciolo, Gabriele Sicuro and Andrea Sportiello
: [doi: 10.1088/1751-8121/ab4a34](https://doi.org/10.1088/1751-8121/ab4a34){:target="\_blank"} - <a href="assets/concave1d.pdf" target="\_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i> (preprint)</a>

### Published
-->
<!--
[4] **The Dyck bound in the concave 1-dimensional random assignment model**
: with Sergio Caracciolo, Vittorio Erba and Andrea Sportiello
: J. Phys. A: Math. Theor. **53** 064001 – Published 14 January 2020
: [doi: 10.1088/1751-8121/ab4a34](https://doi.org/10.1088/1751-8121/ab4a34){:target="_blank"} - <a href="assets/concave1d.pdf" target="_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i> (preprint)</a>

[3] **Anomalous scaling of the optimal cost in the one-dimensional random assignment problem**
: with Sergio Caracciolo and Gabriele Sicuro
: J. Stat. Phys. **174**, 846 – Published 17 December 2018
: [doi: 10.1007/s10955-018-2212-9](https://doi.org/10.1007/s10955-018-2212-9){:target="_blank"} - <a href="assets/Corrections1d.pdf" target="_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i> (preprint)</a>

[2] **Random Euclidean matching problems in one dimension**
: with Sergio Caracciolo and Gabriele Sicuro
: Phys. Rev. E **96**, 042102  – Published 3 October 2017
: [doi: 10.1103/PhysRevE.96.042102](https://doi.org/10.1103/PhysRevE.96.042102){:target="_blank"} - <a href="assets/OneDimension.pdf" target="_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i> (preprint)</a>

[1] **Finite-size corrections in the random assignment problem**
: with Sergio Caracciolo, Enrico M. Malatesta and  Gabriele Sicuro
: Phys. Rev. E **95**, 052129 – Published 17 May 2017
: [doi: 10.1103/PhysRevE.95.052129](https://doi.org/10.1103/PhysRevE.95.052129){:target="_blank"} - <a href="assets/FSC.pdf" target="_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i> (preprint)</a>


<### Posters -->


<!-- ### Articles -->


<!--### Preprints-->
<!--
<dl>
{% assign list = site.data.pubs | where: 'preprint', true %}
{% assign count = 1 %}
{% for pub in list %}
  <dd style="margin-left: 20px;">[{{ count }}] <b>{{ pub.title }}</b> with {{ pub.authors }}. Preprint: <a href="{{ pub.arxivurl }}" target="\_blank"> arXiv: {{ pub.arxivcode }} </a> ({{ pub.year }}).</dd>
{% assign count = count | plus: -1 %}
{% endfor %}
</dl>
-->
### Published
<dl>
{% assign list = site.data.pubs | where: 'published', true %}
{% assign count = 4 %}
{% for pub in list %}
  <!--dt>  {{ pub.title }} with {{ pub.authors }}
  </dt-->
  <dd style="margin-left: 20px;">[{{ count }}] <a href="{{ pub.doi }}" target="\_blank">{{ pub.title }}</a> with {{ pub.authors }}. &nbsp;<i>{{ pub.journal }}</i> <b>{{ pub.volume }}</b>, {{ pub.pages }} ({{ pub.year }}).</dd>
{% assign count = count | plus: -1 %}
{% endfor %}
</dl>
