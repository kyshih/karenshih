---
layout: page
title: photoportfolio
permalink: /photoportfolio/
nav: true
---


{% for image in site.static_files %}
<!--
    {% if image.path contains 'photoportfolio' %}

-->
<div class="project">
    <div class= "thumbnail">
        <a href="{{ site.baseurl }}{{ image.path }}">
            <img class="thumbnail" src="{{ site.baseurl }}{{ image.path }}" />
        </a>
    </div>
</div>

<!--
    {% endif %}
-->
{% endfor %}




<!-- this is for the lightbox --> 
<script type="text/javascript" src="{{ site.baseurl }}/js/lightbox.js"></script>
<link rel="stylesheet" href="{{ site.baseurl }}/css/lightbox.css">
