---
layout: cvmp-twitter
title: News
year: 2024
---

<div class="col-12 col-sm-12 col-lg-12 news">

  {% assign news = site.categories.news | sort:"date" %}
  {% for n in news reversed %}
 {% if n.year == page.year %}
    <div class="panel panel-default bottom3">
        <div class="panel-heading">
            <h2 class="panel-title"><a href="{{ site.url }}{{ site.baseurl }}{{ n.url }}">{{ n.title }}</a></h2>
            <p>{{ n.date | date: "%B %d, %Y" }}</p>
        </div>
        <div class="panel-body">
            {{ n.content }}
        </div>
    </div>
    {% endif %}

    {% endfor %}
</div><!--/span-->
