---
layout: default
permalink: /theses
title: "Theses"
---

## Theses


<div class="panel panel-default">
<div class="panel-heading">
      <h4 class="panel-title">PhD Thesis</h4>
    </div>
<div class="panel-body">
{% for item in site.data.theses %}
{%if item.type == 'phd' %}
<div>
<p><strong>{{item.title}}</strong>, <em>{{item.student}}, Advisor: {{item.advisor}}</em>, {{item.year}} 
{% if item.filename != nil %}<a href="{{item.filename}}"><span class="glyphicon glyphicon-download-alt" aria-hidden="true"></span></a>{% endif %}
</p>
</div>
{% endif %}
{% endfor%}
</div>
</div>

<div class="panel panel-default">
<div class="panel-heading">
      <h4 class="panel-title">MSc Dissertations</h4>
    </div>
<div class="panel-body">
{% for item in site.data.theses %}
{%if item.type == 'msc' %}
<div>
<p><strong>{{item.title}}</strong>, <em>{{item.student}}, Advisor: {{item.advisor}}</em>, {{item.year}} 
{% if item.filename != nil %}<a href="{{item.filename}}"><span class="glyphicon glyphicon-download-alt" aria-hidden="true"></span></a>{% endif %}
</p>
</div>
{% endif %}
{% endfor%}
</div>
</div>