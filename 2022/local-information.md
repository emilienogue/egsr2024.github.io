---
layout: egsr-default
title: Local Information
year: 2022
---

{% if page.year != null %}
	{% assign year = page.year %}
{% else %}
	{% assign year = site.data.egsr.current-year %}
{% endif %}
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.8.0/dist/leaflet.css" integrity="sha512-hoalWLoI8r4UszCkZ5kL8vayOGVae1oxXe/2A4AO6J9+580uKHDO3JdHb7NzwwzK5xr/Fs0W40kiNHxM9vyTtQ==" crossorigin="">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css" crossorigin="">
<script src="https://unpkg.com/leaflet@1.8.0/dist/leaflet.js" integrity="sha512-BB3hKbKWOc9Ez/TAwyWxNXeoV9c1v6FIeYiBieIWkpLjauysF18NzgR1MBNBXf8/KABdlkX68nAhlwcDFLGPCQ==" crossorigin=""></script>


<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/Leaflet.awesome-markers/2.0.2/leaflet.awesome-markers.css" />
<script src="https://cdnjs.cloudflare.com/ajax/libs/Leaflet.awesome-markers/2.0.2/leaflet.awesome-markers.min.js"></script>
<style>

.leaflet-container {
  height: 600px;
  width: 100%;
  max-width: 100%;
  max-height: 100%;
  font-size: 14px;
}

.info {
  padding: 6px 8px;
  font: 14px/16px Arial, Helvetica, sans-serif;
  background: white;
  background: rgba(255, 255, 255, 0.8);
  box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
  border-radius: 5px;
}

.info h4 {
  margin: 0 0 5px;
  color: #777;
}

.awesome-marker i.large {
  font-size: 20px;
}

.awesome-marker i.medium {
  font-size: 14px;
}
</style>

## Conference Venue

The conference takes place at the Philosophical Faculty of Charles University at <code>Celetná 20</code> right in the city center of old town Prague 1 (see [map](#map) below). This building is known for its kafkaesque labyrinth structure, so we assembled you a guide to find the registration and the <span class="lead"><span class="label label-primary">blue lecture hall</span></span> (modrá posluchárna).
<div class="row">
  <div class="col-sm-6 col-md-4">
    <div class="thumbnail">
      <img src="/img/2022/Celetna20_entry-1.jpg">
      <div class="caption">
        <span class="lead"><span class="label label-primary">1</span></span> Take the big wooden double door at house number 20.
      </div>
    </div>
  </div>
  <div class="col-sm-6 col-md-4">
    <div class="thumbnail">
      <img src="/img/2022/Celetna20_entry-2.jpg">
      <div class="caption">
        <span class="lead"><span class="label label-primary">2</span></span> Cross the hallway straight ...
      </div>
    </div>
  </div>
  <div class="clearfix visible-sm hidden-md hidden-lg"></div>
  <div class="col-sm-6 col-md-4">
    <div class="thumbnail">
      <img src="/img/2022/Celetna20_entry-3.jpg">
      <div class="caption">
        <span class="lead"><span class="label label-primary">3</span></span> and take the glass door at the end. In the small courtyard go through the arch on the right.
      </div>
    </div>
  </div>
  <div class="clearfix hidden-sm visible-md visible-lg"></div>
  <div class="col-sm-6 col-md-4">
    <div class="thumbnail">
      <img src="/img/2022/Celetna20_entry-4.jpg">
      <div class="caption">
        <span class="lead"><span class="label label-primary">4</span></span> Go through the short passage behind it, to the next courtyard.
      </div>
    </div>
  </div>
  <div class="clearfix visible-sm hidden-md hidden-lg"></div>
  <div class="col-sm-6 col-md-4">
    <div class="thumbnail">
      <img src="/img/2022/Celetna20_entry-5.jpg">
      <div class="caption">
        <span class="lead"><span class="label label-primary">5</span></span> Walk to the other end of this courtyard ...
      </div>
    </div>
  </div>
  <div class="col-sm-6 col-md-4">
    <div class="thumbnail">
      <img src="/img/2022/Celetna20_entry-6.jpg">
      <div class="caption">
        <span class="lead"><span class="label label-primary">6</span></span> until you arrive at the EGSR 2022 venue.
      </div>
    </div>
  </div>
</div>

<div class="alert alert-info" role="alert">
<i class="fa-solid fa-circle-info"></i> This is also where <a href="http://egsr2011.mff.cuni.cz/">EGSR 2011</a> took place if any of you remember.
</div>

## Reception Venue
The conference reception takes place in the *Refectory* - a ceremonial hall -  at <code>Malostranské náměstí 25</code> (see [map](#map) below) on Monday 7pm. The building is an old monastery from the 17th century and now home to the computer science section of Charles University.

<div class="row">
  <div class="col-sm-6 col-md-4">
    <div class="thumbnail">
      <img src="/img/2022/MalostranskeNam25_entry.jpg">
      <div class="caption">
        Take the door on the right, when you look across the square. The entrance is at the north-east corner of the building.
      </div>
    </div>
  </div>
</div>

<div class="alert alert-info">
<i class="fa-solid fa-compass"></i> 
Take tram 15 from Náměstí Republiky tram station to Malostranské náměstí (see <a href="/2022/local-information#map">map</a>). The tram leaves 18:21, 18:31, 18:41, 18:51, 19:01, 19:11 or check the <a href="https://www.dpp.cz/en/current-departures?cis=47133&ds=N%C3%A1m%C4%9Bst%C3%AD%20Republiky">live departures</a> for 15 (on platform B). <br>
Or take a beautiful <a href="https://en.mapy.cz/s/panujemada">30 minute walk across Charles Bridge</a>: Walk west-wards towards the castle and you can't miss it.
</div>

## Payments
Czech Republic uses it's own currency, the Czech Krown (CZK, Kč). The exchange rate is about 1€ ≈ 25 CZK, so as a quick conversion help, you can multiply by four to get the amount in Euro cents. Here is a handy conversion table:

| CZK  | Euro |
|------|------|
| 25   | 1    |
| 50   | 2    |
| 100  | 4    |
| 500  | 20   |
| 1000 | 40   |

You can pay by (credit + debit) card almost everywhere - even small amounts - except for some rare cases where they only accept cash. Beware: Euro and Dollar payments may be accepted in some touristy places, but at bad conversion rates. 

### Exchanges
Prague is littered with shady exchanges and ATMs with crazy fees (eg. blue + yellow Euronet ATMs) - especially in the city center and at the airport. Avoid these places and instead get some cash from a bank ATM (Česká spořitelna, KB, Fio, Air, Equa). Make sure to always withdraw in CZK, such that your home bank handles the conversion at your known fee & rate. Online banks like Revolut and (Transfer)Wise are transparent about their fees and will give you the exact market conversion rate.
If you must use a cash exchange, here is a list of [honest exchange places](https://honest.blog/honest-exchange-places/). [Honest guide video](https://www.youtube.com/watch?v=_vq_YJjHoRs)

## Public Transport

Prague has a good and affordable public transport system that relies on a dense network of trams, three metro lines (<span class="label label-success">A</span>, <span class="label label-warning">B</span>, <span class="label label-danger">C</span>), buses, ferries, a funicular and local trains. All of these are included in a ticket for the duration of its validity and within the boundaries of Prague. 

### Finding connections
Finding a good connection works best with the [DPP Website](https://www.dpp.cz/en), the [official Prague transport app (PID litacka)](https://app.pidlitacka.cz/), and mostly also with Google Maps.

### Tickets
We recommend you **get the 3-day / 72 hours ticket** for 330 CZK / 13 €, which is available at every tram/metro/(bus) stop from the [yellow vending machines](https://www.dpp.cz/en/fares/list-of-points-of-sales?filter=1&ticket=1) (card payment only), the official information centers and at most little tobacco/newspaper shops (Trafika). Alternatively you can use the [official Prague transport app](https://app.pidlitacka.cz/) to buy tickets from your phone. In a pinch, short-term tickets are also available [inside the trams (card payment only)](https://www.dpp.cz/en/fares/cashless-payment-of-fare).

### From the airport to the city center
Buy an (at least) 90 minute ticket at one of the two DPP (Prague transport) information centers, or at the yellow vending machine on the bus stop. You can already use your 72hours ticket for that too. There is an Airport Express (AE) bus line to the main train station, but for an extra fee. We (and the [Honest Guide](https://www.youtube.com/watch?v=57WeRN0Nrb4)) recommend the following route:

<div class="alert alert-info">
Take bus 119 (every 2-5 minutes) to Nádraží Veleslavín (final stop), transfer to green Metro <span class="label label-success">A</span> in the direction Skalka/Hostivař (right side when you come down) to get to the city center (Staroměstská, Můstek (connection to <span class="label label-warning">B</span>), Muzeum (connection to <span class="label label-danger">C</span>)).
</div>

### Taxis
Taxis have been famous means of scamming people in the past. It gotten way better nowadays, but you should always ask for the estimated price upfront and potentially compare to what Uber would charge you for the same route. You can safely use Uber, Bolt and similar apps in Prague.

## Culture
If you're looking for current cultural events visit [goout.net](https://goout.net/en/prague/events/leznyvlkk/).

### Mini Czech Course

| English              | Czech               | Phonetic simplified  |
|----------------------|---------------------|----------------------|
| Good day             | Dobrý den           | Dobri den            |
| Hello (informal)     | Ahoj                | Ahoi                 |
| Thank you            | Děkuji / Děkuju     | Djekuji              |
| Please               | Prosím              |                      |
| Beer                 | Pivo                |                      |
| A large beer please. | Velké pivo, prosím. | Velke pivo prosim    |
| A small beer please. | Malé pivo, prosím.  | Male pivo prosim     |
| Yes                  | Ano                 | (joo)                |
| No                   | Ne                  |                      |
| Goodbye              | Nashledanou         | Naskledanou (Naskle) |

### Good behaviour
 - Escalators: Stand on the right, walk on the left.
 - Trams, Metro: Let people out, before you enter.
 - Free up seats (marked, close to the door) for elderly and pregnant women in public transport.
 - Help lifting strollers into the tram.
 - Trams have absolute priority in traffic. Beware when crossing the tracks - especially in front of a standing tram - **they will run you over** (or at least ring at you).
 - Tips are not included but also not compulsory. Common tips are 10-15% or rounding up (5-10 CZK).
 - Don't enter parks on rented scooters ("No Segway" signage). This is a plague.
 - Be a real local: If you spot the [orange maintenance tram](https://www.dpp.cz/en/entertainment-and-experience/events-and-attractions/lubricating-tram) take a picture. PRG ❤️ its oiling tram - to the point where it has a live webcam on the back.
 - Keep quiet after 10pm.

### Bars and Restaurants
We have collected a number of recommendations for restaurants, bars and pubs in this interactive map below. There are some for the touristy city center, but most of them are further outside to give you an impression of the real Prague. We encourage you to explore the city beyond the tourist attractions - hop on a tram and make use of your ticket!

<div class="alert alert-info">
<i class="fa-solid fa-circle-info"></i>
Use the menu on the top-right of the map to enable the category you are interested in.<br>Click on points, lines and areas for a popup.
</div>
<div id="map" class="leaflet-container" />
<script src="/2022/map.js"></script>