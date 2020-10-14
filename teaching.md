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

(total experience: approx. {{ i }} hours eqTD)
<!--- TOC
I am currently Research and Teaching Assistant (ATER) at the Université de Paris Est (Créteil). During my PhD, I was Tutor (Moniteur) and then Lecturer in Mathematics at the Université de Paris-Saclay.
Classes I am/have been involved with are:
{:toc}-->

I am currently a research and teaching assistant (ATER) for the [Laboratoire d’analyse et de mathématiques appliquées (LAMA)](https://lama.u-pem.fr/){:target="\_blank"} of the Université de Paris-Est Créteil.



### Current and previous classes:

<ul>
  {% assign sorted = site.courses | sort: 'year' | reverse %}
  {% for course in sorted %}
    <li style="margin-left: -20px;">
      {{course.year}} - <a href="{{ course.url }}"><b>{{ course.title }}</b></a>
      - {{ course.level }} level{% if course.hours %}, {{ course.hours}} hours eqTD {% endif %}.
    </li>
  {% endfor %}
</ul>
