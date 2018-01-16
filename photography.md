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


<!-- <div class="demo-gallery">
<ul id="lightgallery" class="list-unstyled center-block">
    {% for photo in site.data.photography %}
    <li class="col-xs-6 col-sm-4 col-md-3 center-block" data-src="{{ site.url }}{{ site.page_img_path }}/photography/{{ photo.location }}" data-sub-html="<p>{{ photo.title }}</p>" style="margin:0px; padding:0px;">
        <a href="">
            <img class='img-responsive center-block' src="{{ site.url }}{{ site.page_img_path }}/photography/tn/{{ photo.location | remove: '.jpg' }}_tn.jpg" alt="{{ photo.title }}" />
        </a>
    </li>
    {% endfor %}
</ul>
</div> -->

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
