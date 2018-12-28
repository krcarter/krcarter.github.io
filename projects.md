---
layout: page
title: Projects
permalink: /projects/
---

Here are a few of my projects I have work on over the years. These projects are from classes I have taken, programs that I have been a part of, and personal hobby projects that I have undertaken.

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
