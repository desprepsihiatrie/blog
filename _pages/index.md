---
layout: page
title: Home
id: home
permalink: /
---

# Salut 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Take a look at <span style="font-weight: bold">[[Your first note]]</span> to get started on your exploration.
</p>

Creierul uman este capabil să învețe, să se adapteze și să evolueze pe tot parcursul vieții. Este un instrument de procesare a informațiilor extrem de complex, care poate crea, imagina și înțelege lumea din jurul nostru. Este adevărat că încă avem mult de învățat despre funcționarea creierului, dar ceea ce știm deja este suficient pentru a ne da seama că acesta este un organ uimitor și fascinant!

Sunt doctor Marius Motoi.
![Dr  Marius Motoi](https://github.com/desprepsihiatrie/blog/assets/139854003/9ccbade5-fe21-44f8-bdad-89be1efc55a6)


<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
