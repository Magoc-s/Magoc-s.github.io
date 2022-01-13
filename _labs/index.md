---
title: Labs
permalink: /labs/
hidden: True
show_toc: true
---

This course has some labs, and they're great.

## Content {#lab-content}

{% for lab in site.labs %}
{% unless lab.hidden %}
{% if lab.title contains ":" %}
  {% assign tag = lab.title | split: ":" | first %}
{% endif %}
{% assign title = lab.title %}
{% assign link_url = lab.url | prepend: site.baseurl %}
{% assign text = lab.summary | strip_html %}

<h3><a href="{{ link_url }}">{{ title }}</a></h3>

{% comment %}
<p>{{ text }} <a href="{{ link_url }}">(link)</a></p>
{% endcomment %}

{% endunless %}
{% endfor %}
