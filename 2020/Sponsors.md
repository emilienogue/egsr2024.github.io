---
# permalink: /sponsors/
permalink: "/2020/sponsors"
layout: egsr-default
title: Sponsors
year: 2020
---
{% if page.year != null %}
    {% assign year = page.year %}
{% else %}
    {% assign year = site.data.egsr.current-year %}
{% endif %}
We thank all our Sponsors very much for their support to the Computer Graphics community.
<h1 style="color:#D4AF37">Gold</h1>
<div class="row-xs-12 sponsors" >
	{% for sponsor in site.data.sponsors[year].list %}
		{% if sponsor.level contains 'gold' %}
			<div class="individualSponsor">
				<a href="{{sponsor.url}}" target="_blank"><img src="{{site.url}}/{{sponsor.image2}}" class="sponsorImagePageGold img-responsive-50" alt="{{sponsor.name}} logo" title="{{sponsor.name}}"></a>
				<span>{{sponsor.description}}</span>
			</div>
		{% endif %}
	{% endfor %}
</div>
<div class="row-xs-12 row-sm-6 line"></div>

<h1 style="color:#C0C0C0">Silver</h1>
<div class="row-xs-12 sponsors" >
	{% for sponsor in site.data.sponsors[year].list %}
		{% if sponsor.level contains 'silver' %}
			<div class="individualSponsor">
				<a href="{{sponsor.url}}" target="_blank"><img src="{{site.url}}/{{sponsor.image2}}" class="sponsorImagePageSilver img-responsive-50" alt="{{sponsor.name}} logo" title="{{sponsor.name}}"></a>
				<span>{{sponsor.description}}</span>
			</div>
		{% endif %}
	{% endfor %}
</div>
<div class="row-xs-12 row-sm-6 line"></div>

<div class="row-xs-12 sponsors" >
	{% for sponsor in site.data.sponsors[year].list %}
		{% if sponsor.level contains 'paperAward' %}
			<div class="individualSponsor">
				<a href="{{sponsor.url}}" target="_blank"><img src="{{site.url}}/{{sponsor.image}}" class="sponsorImagePageBestPaper img-responsive-50" alt="{{sponsor.name}} logo" title="{{sponsor.name}}"></a>
				<span><b>Best paper award sponsor</b></span>
				<!--<span>{{sponsor.description}}</span>-->
			</div>
		{% endif %}
	{% endfor %}
</div>
<!--<div class="row-xs-12 row-sm-6 line"></div>

<h1 style="color:#cd7f32">Bronze</h1>
<div class="row-xs-12 sponsors" >
	{% for sponsor in site.data.sponsors[year].list %}
		{% if sponsor.level contains 'bronze' %}
			<div class="individualSponsor">
				<a href="{{sponsor.url}}" target="_blank"><img src="{{site.url}}/{{sponsor.image2}}" class="sponsorImagePageBronze img-responsive-50" alt="{{sponsor.name}} logo" title="{{sponsor.name}}"></a>
				<span>{{sponsor.description}}</span>
			</div>
		{% endif %}
	{% endfor %}
</div>-->
