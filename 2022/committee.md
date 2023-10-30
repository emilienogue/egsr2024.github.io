---
layout: egsr-default
title: Committee
year: 2022
---

<div class="col-12 col-sm-12 col-lg-12">

<div class="col-4 col-sm-6 col-lg-4">
    <div class="panel panel-default">
<!--        <div class="panel-heading">
            <h4 class="panel-title">Programme chairs</h4>
        </div>

        {% for chair in site.data.egsr2021.chairs.papers %}
        <div class="panel-body">
            <h4>
                <a href="{{ chair.url }}" target="_blank">{{ chair.name }}</a>
                <br><small>{{ chair.affiliation}}</small>
            </h4>
        </div>
        {% endfor %}

    </div> -->

    <div class="panel panel-default">
        <div class="panel-heading">
            <h4 class="panel-title">Program Committee</h4>
		</div>
        {% for ipc_member in site.data.egsr2022.committee %}
            <div class="panel-body">
                <h4>{{ ipc_member.name }}<br><small>{{ ipc_member.affiliation }}</small></h4>
            </div>
        {% endfor %}
    </div>
</div>

<div class="col-4 col-sm-6 col-lg-4">
<!--    <div class="panel panel-default">
        <div class="panel-heading">
            <h4 class="panel-title">Conference chairs</h4>
        </div>
        {% for chair in site.data.egsr2022.chairs.conference %}
        <div class="panel-body">
            <h4><a href="{{ chair.url }}" target="_blank">{{ chair.name }}</a><br>
            <small> {{ chair.affiliation }} </small></h4>
        </div>
        {% endfor %}
    </div>

    <div class="panel panel-default">
        <div class="panel-heading">
            <h4 class="panel-title">Award chair</h4>
        </div>
        {% for chair in site.data.egsr2022.chairs.awards %}
        <div class="panel-body">
            <h4><a href="{{ chair.url }}" target="_blank">{{ chair.name }}</a><br>
            <small> {{ chair.affiliation }} </small></h4>
        </div>
        {% endfor %}
    </div>-->
</div>