---
layout: page
title: gallery
permalink: /gallery/
nav: true
---


{% for image in site.static_files %}
<!--
  {% if image.path contains 'gallery' %}
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
<script type="text/javascript" src="{{ site.baseurl }}/assets/js/lightbox.js"></script>
<link rel="stylesheet" href="{{ site.baseurl }}/assets/css/lightbox.css">
