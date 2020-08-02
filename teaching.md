---
layout: page
title: Teaching
order: 4
---
{% assign i = 0 %}
{% assign s1 = site.courses %}
{% for c in s1 %}
    {% assign i = i | plus: c.hours %}
{% endfor %}

(total experience: approx. {{ i }} hours)
<!--- TOC
I am currently Research and Teaching Assistant (ATER) at the Université de Paris Est (Créteil). During my PhD, I was Tutor (Moniteur) and then Lecturer in Mathematics at the Université de Paris-Saclay.
Classes I am/have been involved with are:
{:toc}-->

Currently: Lecturer in Mathematics for the Mathematics Department ([Département de Mathématiques d'Orsay](https://www.math.u-psud.fr/?lang=fr){:target="\_blank"}) of the Université de Paris-Saclay.



### Classes:

<ul>
  {% assign sorted = site.courses | sort: 'year' | reverse %}
  {% for course in sorted %}
    <li style="margin-left: -20px;">
      {{course.year}} - <a href="{{ course.url }}"><b>{{ course.title }}</b></a>
      - {{ course.level }} level, {{ course.hours}} hours eqTD.
    </li>
  {% endfor %}
</ul>
