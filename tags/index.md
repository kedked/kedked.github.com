---
title: Tags--ked's Space
layout: page
---
{% for tag in site.tags %}
<section id="{{ tag[0] }}">
    <h2>{{ tag[0] }}</h2>
    <ul>
    	{% for post in tag[1] %}
        <li>
            > <a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
        </li>
        {% endfor %}
    </ul>
    </section>
    {% endfor %}