---
title: Nächster Wolust
layout: post
date: Jan 01, 2019 8:00 PM
update_date: "''"
categories: Ort Zeit
description: Das ist der Terminkalender der Linux User Gruppe Worms
summary-date: summary braucht man hier nicht mehr
last_modified_at: Apr 17, 2019 8:00 PM
---

<ul>
<li>Wormser Linux Stammtisch Termine</li>
</ul>
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

[Kalender/ICS]({{ site.baseurl }}{% link wolust.ics %})


{% include share_buttons.html %}