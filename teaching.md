---
layout: page
title: Teaching
order: 5
---
{% assign i = 0 %}
{% assign s1 = site.courses %}
{% for c in s1 %}
    {% assign i = i | plus: c.hours %}
{% endfor %}


{: style="text-align: justify" }
<!--
I currently teach for the [Laboratoire d’analyse et de mathématiques appliquées (LAMA)](https://lama.u-pem.fr/){:target="\_blank"} of the université Paris-Est Créteil.
-->


### Invited graduate or research-level courses
<br/>

_29.07.24 - 04.08.24_ &nbsp; *An invitation to random assignment problems*  &nbsp; <span style="font-size: .8rem"></span><br/>

AESIM-CIMPA Summer School "Probability with / on random graphs:
trees, networks, dimers, assignments'', Nesin Mathematics Village, Turkey<br/>
[**School webpage**](https://sites.google.com/view/probabilityinturkey/main){:target="_blank"}
{: style="font-size: 15px; margin-left: 170px;" }

Exercises: [1]({{  site.baseurl }}assets/TD1-Nesin24.pdf){:target="_blank"}, [2]({{  site.baseurl }}assets/TD2-Nesin24.pdf){:target="_blank"}, [3]({{  site.baseurl }}assets/TD3-Nesin24.pdf){:target="_blank"}, [4]({{  site.baseurl }}assets/TD4-Nesin24.pdf){:target="_blank"}
{: style="font-size: 18px; margin-left: 170px;" }

###  Regular Classes

Total teaching experience: about {{ i }}h eqTD

How to read the following list, from left to right: <br/>
academic year  <a href="#"><b>Class Title</b></a> - institution, level, total teaching load in eqTD hours
{: style="font-size: 17.3px" }

<!--
Click on class name for details (beware, possibly in French!).
-->
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
