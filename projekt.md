---
layout: page
title: "Projekt Freigeist"
lang: de
permalink: /projekt/
---

<div class="overview">
    <h2>Über das Projekt</h2>
    <p>Das Projekt Freigeist ist ein metakreatives Experiment zur Analyse, Simulation und Dekonstruktion des Menschseins in der Ära künstlicher Intelligenz. Hier findest du alle Beiträge, die im Rahmen dieses Projekts entstanden sind.</p>
</div>

<section>
    <h2>Alle Beiträge</h2>
    <ul class="post-list">
        {% for post in site.posts %}
        {% if post.lang == 'de' %}
        <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
        {% endif %}
        {% endfor %}
    </ul>
</section>