---
layout: nl-page
title: OpenStreetMap - De editeerbare kaart!
excerpt: "OpenStreetMap - The editable map of the world!"
search_omit: true
---
OpenStreetMap (OSM), of kortweg OSM, is een internationaal open data project met als doel een editeerbare map te maken van de ganse wereld. De Belgische tak maakt deel uit van de meer dan 2 miljoen wereldwijd geregistreerde gebruikers.

# Wat is de OpenStreetMap community?

Sinds 2004 worden er van over de hele wereld gegevens verzameld over wegen, spoorwegen, rivieren, bossen, zieken-huizen, restaurants, enz. Die gegevens worden opgeslagen in een database die gratis toegankelijke is voor iedereen, wat er voor zorgt dat je zelf aan de slag kan gaan met de beschikbare data. 

Onze community werk aan het collecteren, aanpassen en toevoegen van data aan OSM.  De meeste van ons zijn 'mappers'.  Het mappen zelf is niet alleen meer weggelegd voor de meer technische of professionele gebruikers. Iedereen kan onze rangen vervoegen.

Het invoeren van informatie en aanpassen van de gegevens steunt volledig op vrijwilligers. Ook als jij de kaart graag anders en beter zou zien... iedereen kan bijdragen!

# Waarom zou je je eigen map willen maken, is google maps niet genoeg?

In de eerste plaats, goede kaarten zijn niet altijd beschikbaar.  Zelfs grote bedrijven zoals Google en TomTom hebben fouten.  Vergelijk het met een gedrukte encyclopedie, waar maar een paar personen aan mogen werken vs. Wikipedia, waar iedereen kan inspringen.   OSM werkt op gelijkaardige wijze.  Men zegt wel eens : OSM is de wikipedia van de kaart.

In de tweede plaats,  commerciële en andere belangen liggen in de weg van correctheid en compleetheid.   Als enkel de staat of grote bedrijven bepalen wat er op een kaart komt, dan zou het maar een saaie boel zijn waar enkel 'officiële' data op de kaart geraakt.   Enkel wegen die voor hen de moeite zijn.  

Onze community zorgt hier voor een rijke, diverse kaart.  Waar de som van de persoonlijke interesses van de mappers zorgen voor een mix en rijkdom aan informatie waar ieders zijn stukje kan uithalen waarin hij zich interesseert.  Als voorbeeld kan je het rijke netwerk aan wandel en fietsroutes raadplegen, gemaakt door enthousiaste wandelaars en fietsers voor hun avontuurlijke collegas.

Maar vooral: onze data is open.  Iedereen kan zonder al te veel verplichtingen de data download en ermee expirimenteren.  Wij geloven dat een samenwerking zoals deze moet samengaan met gratis ter beschikking stellen van het resultaat om op lange termijn succesvol te blijven.

# Blog

<ul class="post-list">
{% for post in site.categories.blog %} 
	{% if post.categories contains 'nl' %}
		<li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
	{% endif %}
{% endfor %}
</ul>
