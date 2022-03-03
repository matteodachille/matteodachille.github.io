---
layout: page
title: Teaching
order: 6
---
{% assign i = 0 %}
{% assign s1 = site.courses %}
{% for c in s1 %}
    {% assign i = i | plus: c.hours %}
{% endfor %}


{: style="text-align: justify" }
I currently teach for the [Laboratoire d’analyse et de mathématiques appliquées (LAMA)](https://lama.u-pem.fr/){:target="\_blank"} of the université Paris-Est Créteil.



### Current and previous classes

(academic year  class title - institution, level, total teaching load in eqTD hours). <br/> Click on class name for more details (possibly in French).

<ul style="list-style: none;
   margin-left: 10;
   padding-left: 1em;
   text-indent: -2.2em;">
  {% assign sorted = site.courses | sort: 'classnumber' | reverse %}
  {% for course in sorted %}
    <li style="margin-left: -40px;">
      {{course.year}} &nbsp; <a href="{{ course.url }}"><b>{{ course.title }}</b></a>
      - {{ course.etab}}, {{ course.level }}{% if course.hours %}, {{ course.hours}}h {% endif %}
    </li>
  {% endfor %}
</ul>


_Total experience_: about {{ i }}h eqTD
