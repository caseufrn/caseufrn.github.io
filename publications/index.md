---
layout: default
title: "Publications"

years:
 - '2017'
 - '2016'
 - '2015'
 - '2014'
 - '2013'
---

## Publications


{% for year in page.years %}

<div class="panel panel-default">
<div class="panel-heading">
      <h4 class="panel-title">{{year}}</h4>
    </div>
<div class="panel-body">
{% for item in site.data.publications %}
{%if item.year == year %}
<div>
<p><span class="label label-primary">{{item.type}}</span> <strong>{{item.title}}</strong>
<em>{{item.authors}}, {{item.target}}</em>, {{item.year}} <a href="{{item.doi_link}}"><span class="badge">doi</span></a> <a href="{{item.filename}}"><span class="glyphicon glyphicon-download-alt" aria-hidden="true"></span></a>
</p>
</div>
{% endif %}
{% endfor%}
</div>
</div>
{% endfor%}
