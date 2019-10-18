---
layout: page
title: Teaching activities
order: 3
---

<!--- TOC
{:toc}-->
I am "Doctorant-enseignant" at the Mathematics Department of the Université Paris-Sud.

### '18-'19

<ul>
  {% for course in site.courses %}
    <li>
      <!--<a href="{{ course.url }}">{{ course.title }}</a>-->
      <b>{{ course.title }}</b>, Travaux dirigés for the {{course.studtype}} students {{ course.level }}
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
