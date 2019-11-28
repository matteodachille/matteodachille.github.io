---
layout: page
title: Teaching activities
order: 4
---

<!--- TOC
{:toc}-->
Currently, I carry out teaching activities (mostly Travaux Dirigés) in Mathematics, on behalf of the Mathematics Department ([Département de Mathématiques d'Orsay](https://www.math.u-psud.fr/?lang=fr){:target="_blank"}) of the Université de Paris-Sud.


### '18-'19

<ul>
  {% for course in site.courses %}
    <li>
      <a href="{{ course.url }}"><b>{{ course.title }}</b></a>
      - Travaux dirigés for {{course.studtype}} students {{ course.level }}, {{ course.hours}} hours
    </li>
  {% endfor %}
</ul>

<!--### 2018/2019
<!--
## Remediation
Teaching assistant

## Calculus 151
**31.5 hours**

**28.5 hours** of **TD** (French _Travaux Dirigés_, Italian _esercitazioni_, English _tutorials_). 1.5 hours sessions from Monday 14/11/2018 to Tuesday 8/01/2019.

**3 hours** exam on Tuesday 15/01/2019
-->
