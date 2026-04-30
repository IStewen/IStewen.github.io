---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

## Journal Articles

{% for post in site.publications reversed %}
  {% if post.papertype == "journal" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Book Contributions

{% for post in site.publications reversed %}
  {% if post.papertype == "book" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Working Papers

{% for post in site.publications reversed %}
  {% if post.papertype == "workingpaper" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
