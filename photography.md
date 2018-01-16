---
layout: page
title: Photography
custom-title: none
permalink: /photography/
published: true
---

<h2 class="text-center">through my eyes ... and a lens</h2>

<br>


<section id="photos">
    {% for photo in site.data.photography %}
    <a class="photoImg" href="{{ site.url }}{{ site.page_img_path }}/photography/{{ photo.location }}">
        <img class='img-responsive' src="{{ site.url }}{{ site.page_img_path }}/photography/tn/{{ photo.location | remove: '.jpg' }}_tn.jpg" alt="{{ photo.title }}" />
    </a>
    {% endfor %}
</section>


<script type="text/javascript">
    $(document).ready(function() {
        $("#photos").lightGallery({
            download: false,
            controls: false,
            hideBarsDelay:600,
            thumbMargin: 0,
            speed: 400,
            showThumbByDefault: false
        }); 
    });
</script>
