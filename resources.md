---
layout: page
title: resources
permalink: /resources/
---

{% for resource in site.resources %}
<div class="project ">
    <div class="thumbnail">
        <a href="{{ site.baseurl }}{{ resource.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ resource.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}
        <span>
            <h1>{{ resource.title }}</h1>
            <br/>
            <p>{{ resource.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endfor %}
