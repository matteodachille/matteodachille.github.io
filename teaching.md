---
layout: page
title: Teaching
order: 5
---

<!--- TOC
{:toc}-->
Currently, I am Lecturer in Mathematics for the Mathematics Department ([Département de Mathématiques d'Orsay](https://www.math.u-psud.fr/?lang=fr){:target="_blank"}) of the Université de Paris-Sud.


<ul>
  {% for course in site.courses %}
    <li>
      {{course.year}} - <a href="{{ course.url }}"><b>{{ course.title }}</b></a>
      - {{course.studtype}} students {{ course.level }}, {{ course.hours}} hours
    </li>
  {% endfor %}
</ul>
