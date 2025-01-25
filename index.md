---
layout: default
title: "Répertoire d'analyses générées par LLM"
---

## Liste des analyses disponibles  :
<ul>
{% for file in site.static_files %}
    {% if file.extname == ".html" and file.path != "/index.html" %}
        <li><a href="{{ file.path | relative_url }}">{{ file.basename }}</a></li>
    {% endif %}
{% endfor %}
</ul>
