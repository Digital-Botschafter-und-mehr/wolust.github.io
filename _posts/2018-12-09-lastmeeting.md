---
title: Die Treffen 2019
layout: post
date: '2018-12-03 06:34:00'
categories: treffen
summary: dummy
description: Kurzer Report der Wolust Stammtische 2019
---

<ul>
 {% for review  in site.data.review19.linuxuser %}
    <li>  {{ review.inhalt }} </li>
 {% endfor %}
</ul>