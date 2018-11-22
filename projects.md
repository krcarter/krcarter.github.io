---
layout: page
title: Projects
permalink: /projects/
---

{% for project in site.projects %}

<div class="project ">
    <div class="thumbnail">
        {% if project.redirect %}
        <a href="{{ project.redirect }}" target="_blank">
        {% else %}
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% endif %}
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endfor %}
