---
layout: 2021/egsr-default
title: Program
year: 2021
---

{% if page.year != null %}
	{% assign year = page.year %}
{% else %}
	{% assign year = site.data.egsr.current-year %}
{% endif %}

The conference takes place on ohyay, where participants can watch the talks and ask questions either in writing or via video chat. The main event will also be live streamed and recorded on YouTube for those who cannot attend the presentations live.

Registered participants can access the ohyay space: [https://ohyay.co/s/egsr2021](https://ohyay.co/s/egsr2021)

Live streams of each day are available via the following YouTube links:
1. [https://youtu.be/u9HqKGqvJhQ](https://youtu.be/u9HqKGqvJhQ)
2. [https://youtu.be/TvWkwDYtBP4](https://youtu.be/TvWkwDYtBP4)
3. [https://youtu.be/eIvTXdTN2MQ](https://youtu.be/eIvTXdTN2MQ)
4. [https://youtu.be/WUBf30dzk3Q](https://youtu.be/WUBf30dzk3Q)

All times are in your local time zone.

The papers are available in the EG digital library: [CGF Track](https://diglib.eg.org/handle/10.2312/2633074), [Symposium Track](https://diglib.eg.org/handle/10.2312/2633075).

<!-- If you are a registered participant, you can join the ohyay workspace via [this link](https://ohyay.co/s/egsr2021).
**Note: not everyone has been granted access yet. If the link does not work for you, please be patient.**
**Important:** Make sure that you use the **same email address** on ohyay that you used during registration. -->

<style>
    @media screen and (min-width: 768px) {
        .schedule {
            display: grid;
            grid-template-rows: repeat(57, 1fr); /* 1 row = 5min slot between 15:00 and 19:00 plus header*/
            grid-template-columns: repeat(4, 1fr); /* 1 col for each of 4 days */
        }
        .session {
            display: block;
        }
    }
    .session {
        background-color: rgb(37, 74, 113);
        color: rgb(256,256,256);
        border-radius: 2px;
        padding: 4px;
        margin: 2px;
    }
    .session:hover {
        cursor: pointer;
    }
    .time-slot {
        color: rgb(256,256,256);
    }
    .special {
        background-color: rgb(187, 84, 93);
    }
</style>

<div class="schedule">

{% assign sorted = site.session | sort: 'start' %}
{% assign curDay = -1 %}

{% for session in sorted %}
    {% if session.year == year %}
        {% assign confStart = '2021-06-29 15:00:00 CEST' | date: '%s' %}
        {% assign start = session.start | date: '%s' %}
        {% assign end = session.end | date: '%s' %}
        {% assign relStart = start | minus: confStart %}
        {% assign startDays = relStart | divided_by: 60 | divided_by: 60 | divided_by: 24%}
        {% assign offset = startDays | times: 24 | times: 60 | times: 60 %}
        {% assign startSecs = relStart | minus: offset %}
        {% assign startMins = startSecs | divided_by: 60 %}
        {% assign durationSecs = end | minus: start %}
        {% assign durationMins = durationSecs | divided_by: 60 %}
        {% if curDay != startDays %}
            <div style="grid-row: 1 / span 3">
                <h4>{{ session.start | date: "%A, %d %B" }}</h4>
            </div>
            {% assign curDay = startDays %}
        {% endif %}
        <div
            {% if session.is_special %}
            class="session special"
            {% else %}
            class="session"
            {% endif %}
            style="
                grid-row: {{ startMins | divided_by: 5 | plus: 4 }} / span {{ durationMins | divided_by: 5 }};
                grid-column: {{startDays | plus: 1}};"
            onClick="window.location = '{{ session.url }}';">
            <span class="time-slot">{{ session.start | date: "%Y-%m-%dT%H:%M+02:00" }}</span>
            <h4 class="session-title">{{ session.title }}</h4>
            <span class="session-chair">{{ session.authors }}</span>
        </div>
    {% endif %}
{% endfor %}
</div>

<script>
    var times = document.getElementsByClassName("time-slot");
    for (var i = 0, len = times.length | 0; i < len; i++) {
        var date = new Date(times[i].innerHTML);
        times[i].innerHTML = date.toLocaleTimeString([], { hour: '2-digit', minute: '2-digit', timeZoneName: 'short' });
    }
</script>
