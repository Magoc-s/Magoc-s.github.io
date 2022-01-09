---
title: Lectures
permalink: /lectures/
hidden: True
layout: default
toc: true
---

This page is code-driven to display a list of all files in this `_lectures` directory and provide links to them. Essentially you can just add new documents into the `_lectures` directory and when the website is rebuilt, they will automatically be listed here. This is a good example of liquid tags (to see the liquid tags you must view the source file, not the built web page.)

These links could also be links to PDF (or other) documents, if your lecture slides/videos are not easily embedded in a web page. How you do this is up to you.

## Lecture Slides

{% comment %}
{% include cardlist.html cards=site.lectures %}
{% endcomment %}

  {% for lecture in site.lectures %}
  {% unless lecture.hidden %}
  {% if lecture.title contains ":" %}
    {% assign tag = lecture.title | split: ":" | first %}
  {% endif %}
  {% assign title = lecture.title %}
  {% assign link_url = lecture.url | prepend: site.baseurl %}
  {% assign text = lecture.summary | strip_html %}

  <h4><a href="{{ link_url }}">{{ title }}</a></h4>

  <p>{{ text }} <a href="{{ link_url }}">(link)</a></p>

  {% endunless %}
  {% endfor %}