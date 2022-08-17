---
layout: null
title: 404
permalink: /apps
---
{
    "name": "{{ site.title }}",
    "apps": [
        {% for post in site.posts %}
            {
                "name": "{{ post.title }}",
                "version": "{{ post.version }}",
                "downloadURL": "{{ post.down }}",
                "iconURL": "{{ post.image }}"
            }
        {% endfor %}
    ]
}
