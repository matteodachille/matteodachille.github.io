---
layout: page
title: Publications
order: 3
---
<!-- - TOC
{:toc} -->

(click on <i class="fa fa-file-pdf-o" aria-hidden="true"></i> for preprint files)

### Preprints

<dl>
{% assign list = site.data.pubs | where: 'preprint', true %}
{% assign count = list.size %}
<!--{% if count != 0 %}
  ### Preprints
  {% endif %}-->
{% for pub in list %}
  <dd style="margin-left: 20px;">[{{ count }}] <b>{{ pub.title }}</b> with {{ pub.authors }}. Preprint: <a href="{{ pub.arxivurl }}" target="\_blank"> arXiv: {{ pub.arxivcode }} </a> ({{ pub.year }}){% if pub.submitted %}, <i>submitted</i>{% endif %} <a href="{{  site.baseurl }}{{ pub.pdf }}" target="\_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i></a></dd>
{% assign count = count | plus: -1 %}
{% endfor %}
</dl>

### Published
<dl>
{% assign list = site.data.pubs | where: 'published', true %}
{% assign count = list.size %}
{% for pub in list %}
  <!--dt>  {{ pub.title }} with {{ pub.authors }}
  </dt-->
  <dd style="margin-left: 20px;">[{{ count }}] <a href="{{ pub.doi }}" target="\_blank">{{ pub.title }}</a> with {{ pub.authors }}. &nbsp;<i>{{ pub.journal }}</i> <b>{{ pub.volume }}</b>, {{ pub.pages }} ({{ pub.year }}) <a href="{{  site.baseurl }}{{ pub.pdf }}" target="\_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i></a></dd>
{% assign count = count | plus: -1 %}
{% endfor %}
</dl>
