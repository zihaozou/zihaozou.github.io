---
layout: page
permalink: /gallery/
title: Gallery
description: My everyday life
nav: true
nav_order: 1
gallery_path: gallery/my_life
---
<!-- _pages/gallery.md -->
<div class="gallery" id="gallery">
    {% for image in site.static_files %}
        {% if image.path contains 'gallery/my_life' %}
            <div class="gallery-item">
                <div class="content"><img src="{{ site.baseurl }}{{ image.path }}" alt=""></div>
            </div>
        {% endif %}
    {% endfor %}
</div>
