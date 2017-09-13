---
layout: page
title: Photography
custom-title: none
permalink: /photography/
published: true
---

<h2 class="text-center">Through my eyes...</h2>

<br>

<div class="experience-wrapper">
  {% for photo in site.data.photography %}
  <div class="gallery_product col-lg-4 col-md-4 col-sm-4 col-xs-6">
      <a type="button" class="btn btn-sm" data-toggle="modal" data-target="#{{ photo.id }}Modal">
          <img src="{{ site.url}}/images/pages/photography/{{ photo.location }}" class="img-thumbnail" alt="{{ photo.title }}">
      </a>
  </div>
  <!-- Modal -->
  <div class="modal fade" id="{{ photo.id }}Modal" tabindex="-1" role="dialog" aria-labelledby="{{ photo.id }}ModalLabel" aria-hidden="true">
    <div class="modal-dialog" role="document">
      <div class="modal-content">
        <div class="modal-body">
            <img src="{{ site.url}}/images/pages/photography/{{ photo.location }}" alt="{{ photo.title }}" class="img-rounded">
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
        </div>
      </div>
    </div>
  </div>
  {% endfor %}
</div>
