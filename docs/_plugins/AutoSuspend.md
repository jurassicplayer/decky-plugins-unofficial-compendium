---
layout: plugin
title: AutoSuspend
project_url: https://github.com/jurassicplayer/decky-autosuspend
category: Active
available_in_store: True
redirect: true
---
{% assign store = site.data[page.title] %}
{% assign name = page.title | default: store.name %}
{% assign author = page.author | default: store.author %}
{% assign description = page.description | default: store.description %}
{% assign tags = page.tags | default: store.tags %}
{% assign versions = page.versions | default: store.versions %}
{% assign image_url = page.image_url | default: store.image_url %}
{% assign image_url = image_url | default: "assets/images/placeholder_screenshot.png" %}
{% assign created = page.created | default: store.created %}
{% assign updated = page.updated | default: store.updated %}

{{ store | json }}
{{ site | json }}
All this cool text with nothing fancy