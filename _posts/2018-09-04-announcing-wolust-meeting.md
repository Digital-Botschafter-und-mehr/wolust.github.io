---
title: Nächster Wolust
layout: post
date: '2018-09-05 17:30:00'
update_date: ''
summary: 06.11.2018 19:30 Uhr im Timescafe
categories: Ort Zeit
description: Das ist der Terminkalender der Linux User Gruppe Worms
---

<strong>Wormser Linux Stammtisch Termine</strong><br />

Wer sich für Linux oder andere freie Betriebssysteme interessiert und aus der Gegend in und um Worms kommt, der ist bei uns herzlich willkommen. Stelle Deine Projekte, Probleme und Lösungen vor! Tipps für Anfänger und Umsteiger.
<ul>
<li>
{% assign next = site.data.daten.linuxuser[0] %}
{{next.meeting}} :
<strong> {{next.tag}}.{{next.monat}}.{{next.jahr}} 19:30 im {{next.ort}} </strong>
</li>
</ul>
Weitere Treffen ohne Gewähr:
<ul>
{% for treffen  in site.data.daten.linuxuser %}
   {% if treffen.meeting <> "Nächstes Treffen" %}
 <li>
 {{treffen.meeting}} :
     {{treffen.tag }}.{{treffen.monat}}.{{treffen.jahr}} {{treffen.ort}}
 </li>  
  {% endif %}
{% endfor %}
</ul>


{% include share_buttons.html %}