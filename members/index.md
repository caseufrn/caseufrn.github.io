---
layout: default
title: "Members"
---

## Members


<div >
	<div class="panel panel-default">
		<div class="panel-heading">
			<h4 class="panel-title">Faculty</h4>
		</div>
		<div class="panel-body">
			<div class="row">
{% for faculty in site.data.members.faculty %}
				<div class="col-xs-6 col-sm-3 col-md-2">
					<img src="{{faculty.img}}" class="img-responsive">
					<h4><a href="{{faculty.url}}" target="blank">{{faculty.name}}</a><br><small>{{faculty.desc}}</small></h4>
				</div>
{% endfor%}
			</div>
		</div>
	</div>

<!-- PhD Students -->

<div class="panel panel-default">
		<div class="panel-heading">
			<h4 class="panel-title">PhD Students</h4>
		</div>
		<div class="panel-body">
			<div class="row">
{% for person in site.data.members.phdstudent %}
				<div class="col-xs-6 col-sm-3 col-md-2">
					<img src="{{person.img}}" class="img-responsive">
					<h4><a href="{{person.url}}" target="blank">{{person.name}}</a><br><small>{{person.desc}}</small></h4>
				</div>
{% endfor%}
			</div>
		</div>
	</div>

<!-- MSc Students -->

<div class="panel panel-default">
		<div class="panel-heading">
			<h4 class="panel-title">MSc Students</h4>
		</div>
		<div class="panel-body">
			<div class="row">
{% for person in site.data.members.mscstudent %}
				<div class="col-xs-6 col-sm-3 col-md-2">
					<img src="{{person.img}}" class="img-responsive">
					<h4><a href="{{person.url}}" target="blank">{{person.name}}</a><br><small>{{person.desc}}</small></h4>
				</div>
{% endfor%}
			</div>
		</div>
	</div>

<!-- Undergrad Students -->

<div class="panel panel-default">
		<div class="panel-heading">
			<h4 class="panel-title">Undergrad Students</h4>
		</div>
		<div class="panel-body">
			<div class="row">
{% for person in site.data.members.undergrad %}
				<div class="col-xs-6 col-sm-3 col-md-2">
					<img src="{{person.img}}" class="img-responsive">
					<h4><a href="{{person.url}}" target="blank">{{person.name}}</a><br><small>{{person.desc}}</small></h4>
				</div>
{% endfor%}
			</div>
		</div>
	</div>

<!-- Undergrad Students -->

<div class="panel panel-default">
		<div class="panel-heading">
			<h4 class="panel-title">Alumini</h4>
		</div>
		<div class="panel-body">
			<div class="row">
{% for person in site.data.members.alumini %}
				<div class="col-xs-6 col-sm-3 col-md-2">
					<img src="{{person.img}}" class="img-responsive">
					<h4><a href="{{person.url}}" target="blank">{{person.name}}</a><br><small>{{person.desc}}</small></h4>
				</div>
{% endfor%}
			</div>
		</div>
	</div>


</div>
