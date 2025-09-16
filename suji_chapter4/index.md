---
title: "Suji Chapter 4 Notes"
layout: default
permalink: /suji_chapter4/
---

# Chapter 4 Notes

Here are my notes for the fourth chapter. Feel free to use them for your studies!

{% for image in site.static_files %}
    {% if image.path contains '/suji_chapter4/' %}
        {% unless image.path contains 'index.md' %} <!-- This excludes this file if it's copied into the folder -->
        <div class="note-image">
            <img src="{{ site.baseurl }}{{ image.path }}" alt="Chapter 4 Note: {{ image.basename }}">
            <p><strong>Image:</strong> {{ image.basename }}</p>
        </div>
        <hr>
        {% endunless %}
    {% endif %}
{% endfor %}
