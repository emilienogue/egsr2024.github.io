---
layout: cvmp-default
title: Sponsors
year: 2024
---

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        .sponsorContainer {
            padding: 20px; /* Adjust the padding value as needed */
        }

        .sponsorImagePageGold {
            max-width: 70%; /* Set the maximum width to 80% of the container */
            height: auto; /* Maintain the aspect ratio */
        }

        .sponsorImagePageSilver {
            max-width: 45%; /* Set the maximum width to 60% of the container */
            height: auto; /* Maintain the aspect ratio */
        }
        
        .sponsorImagePageSilverBestPaperAward {
            max-width: 50%; /* Adjust the maximum width as needed */
            height: auto; /* Maintain the aspect ratio */
        }
    </style>
</head>

{% if page.year != null %}
    {% assign year = page.year %}
{% else %}
    {% assign year = site.data.egsr.current-year %}
{% endif %}
We thank all our Sponsors very much for their support to the Computer Graphics community.
<h1 style="color:#D4AF37">Gold</h1>
<div class="row-xs-12 sponsors" >
    {% for sponsor in site.data.sponsors[year] %}
        {% if sponsor.level contains 'gold' %}
            <div class="individualSponsor sponsorContainer">
                <a href="{{sponsor.url}}" target="_blank"><img src="{{site.url}}/{{sponsor.image}}" class="sponsorImagePageGold" alt="{{sponsor.name}} logo" title="{{sponsor.name}}"></a>
                <p>{{sponsor.description}}</p>
            </div>
        {% endif %}
    {% endfor %}
</div>

<!--<div class="row-xs-12 row-sm-6 line"></div>-->
<!---->
<!--<h1 style="color:#cd7f32">Bronze</h1>-->
<!--<div class="row-xs-12 sponsors" >-->
<!--    {% for sponsor in site.data.sponsors[year].list %}-->
<!--        {% if sponsor.level contains 'bronze' %}-->
<!--            <div class="individualSponsor">-->
<!--                <a href="{{sponsor.url}}" target="_blank"><img src="{{site.url}}/{{sponsor.image2}}" class="sponsorImagePageBronze" alt="{{sponsor.name}} logo" title="{{sponsor.name}}"></a>-->
<!--                <span>{{sponsor.description}}</span>-->
<!--            </div>-->
<!--        {% endif %}-->
<!--    {% endfor %}-->
<!--</div>-->

<div class="row-xs-12 row-sm-6 line"></div>

<h1 style="color:#C0C0C0">Silver</h1>
<div class="row-xs-12 sponsors" >
    {% assign silverSponsors = site.data.sponsors[year] | where: "level", "silver" %}
    {% assign silverBestPaperAwardSponsors = site.data.sponsors[year] | where: "level", "silver2" %}

    {% for sponsor in silverSponsors %}
        <div class="individualSponsor sponsorContainer">
            <a href="{{sponsor.url}}" target="_blank"><img src="{{site.url}}/{{sponsor.image}}" class="sponsorImagePageSilver" alt="{{sponsor.name}} logo" title="{{sponsor.name}}"></a>
            <p>{{sponsor.description}}</p>
        </div>
    {% endfor %}

    {% if silverBestPaperAwardSponsors.size > 0 %}
        <h2 style="color:black">Best Paper Award</h2>
        {% for sponsor in silverBestPaperAwardSponsors %}
            <div class="individualSponsor sponsorContainer">
                <a href="{{sponsor.url}}" target="_blank"><img src="{{site.url}}/{{sponsor.image}}" class="sponsorImagePageSilverBestPaperAward" alt="{{sponsor.name}} logo" title="{{sponsor.name}}"></a>
                <p>{{sponsor.description}}</p>
            </div>
        {% endfor %}
    {% endif %}
</div>
