---
permalink: "/2022/keynotes"
layout: egsr-default
title: Keynotes
year: 2022
---

{% if page.year != null %}
	{% assign year = page.year %}
{% else %}
	{% assign year = site.data.egsr.current-year %}
{% endif %}



<div id="program" class="row-xs-12">
{% assign allKeynotes = site.data.keynotes[year]  | sort: 'keynote_id' %}

	<div class="session-content">

		<div class="session-talks" >
				{% for keynote in allKeynotes %}
					<hr width="40%">

					<div>

						<h3 id="{{keynote.speaker | truncatewords: 1, "" | downcase}}" style="overflow: auto;"><span style="float: left; margin-top: 10px; margin-right: 10px;">{{keynote.title}}</span> 
						</h3>
						<h4>{{keynote.speaker}}</h4>


					</div>

					<div style="overflow: auto; margin-bottom:10px;">
						
						<div style="float: left;"><img src="{{keynote.picture}}" style="max-width:30%; float:left; margin-right: 10px; margin-top: 10px; margin-bottom: 10px"> <b>Bio&nbsp;</b><p style="text-align: justify;">{{keynote.bio}}</p></div>
					</div>
					<div>
						  <b>Abstact</b><p style="text-align: justify;">{{keynote.abstract}}</p>
					</div>
					{% endfor %}

		</div>



			<hr width="75%">
	</div>






</div>