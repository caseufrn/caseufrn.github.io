---
layout: default
title: "Publications"

years:
 - '2024'
 - '2023'
 - '2022'
 - '2021'
 - '2020'
 - '2019'
 - '2018'
 - '2017'
 - '2016'
 - '2015'
 - '2014'
 - '2013'
 - '2012'
 - '2011'
 - '2010'
---

## Publications

<!-- Incluir publicações no arquivo publications.csv, no diretório _data -->

{% for year in page.years %}

<div class="panel panel-default">
<div class="panel-heading">
      <h4  data-toc-text="Year: {{year}}" class="panel-title">{{year}}</h4>
    </div>
<div class="panel-body">
{% for item in site.data.publications %}
{%if item.year == year %}
<div>
<p><span class="label {%if item.type == "journal" %}label-success{%else%}label-info{%endif%}">{{item.type}}</span> <strong>{{item.title}}</strong>
<em>{{item.authors}}, {{item.target}}</em>, {{item.year}} 
{% if item.doi_link != nil %}<a href="{{item.doi_link}}" target="_blank"> <span class="glyphicon glyphicon-link"> &nbsp;&nbsp;&nbsp; </span></a>{%endif%}
{% if item.filename != nil %}<a href="{{item.filename}}" target="_blank"> <span class="glyphicon glyphicon-download-alt" aria-hidden="true"> &nbsp;&nbsp;&nbsp; </span></a>{% endif %}
</p>
</div>
{% endif %}
{% endfor%}
</div>
</div>
{% endfor%}
