---
layout:
title:
permalink: /2020/calendar-data/
---

[
{% for mySession in site.session %}
	{
		"session_id": "{{mySession.session_id}}",
		"title":"{{mySession.title}}",
		"start": "{{mySession.start}}",
		"end": "{{mySession.end}}",
		"url":"#{{mySession.session_id}}",
		"permalink":"#{{mySession.permalink}}",
		"color": "{{mySession.color}}"

	}
	{%unless forloop.last %},{%endunless%}
{% endfor %}
]
