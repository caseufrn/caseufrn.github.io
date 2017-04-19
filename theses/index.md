---
layout: default
title: "Theses"
---
## Theses


{% include thesessection.html title="PhD Thesis" type="phd" %}

{% include thesessection.html title="MSc Dissertations" type="msc" %}


<!--
    <div class="panel panel-default">
<div class="panel-heading">
      <h4 class="panel-title">{{include.title}}</h4>
    </div>
<div class="panel-body">
{% for item in site.data.theses %}
{%if item.type == {{include.type}} %}
<div>
<p><a href="{{item.link}}" target="_blank"><strong>{{item.title}}</strong></a>, <em>{{item.student}}, Advisor: {{item.advisor}}</em>, {{item.year}} - {% if item.filename != nil %}<a href="{{item.filename}}" target="_blank"><span class="glyphicon glyphicon-download-alt" aria-hidden="true"></span></a>{% endif %}</p>
</div>
{% endif %}
{% endfor%}
</div>
</div>

-->