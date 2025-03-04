---
layout: plugin
title: AutoSuspend
project_url: https://github.com/jurassicplayer/decky-autosuspend
category: Active
available_in_store: True
redirect: True
---
{% assign store = site.data[page.title] %}
{% assign name = page.title | default: store.name %}
{% assign author = page.author | default: store.author %}
{% assign description = page.description | default: store.description %}
{% assign tags = page.tags | default: store.tags %}
{% assign versions = page.versions | default: store.versions %}
{% assign image_url = page.image_url | default: store.image_url %}
{% assign default_image = site.baseurl | append: "/assets/images/placeholder_screenshot.png" %}
{% assign image_url = image_url | default: default_image %}
{% assign created = page.created | default: store.created %}
{% assign updated = page.updated | default: store.updated %}

{{ name }} v{{ versions[0].name }} is a cool plugin created by {{ author }}, initially released on {{ created }} and last updated on {{ updated }}, it is described as: {{ description }}
<br />
Also there are tags: {{ tags | jsonify }}