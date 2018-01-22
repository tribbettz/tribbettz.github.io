---
layout: page
title: Experience
custom-title: none
permalink: /experience/
---

<div class="experience-wrapper">
  {% for row in site.data.experience %}
    <div class="card text-center">
      <div class="card-body">
        <h4 class="card-title">{{ row.company }}</h4>
        <p class="post-meta">{{ row.started }} - {{ row.ended }}</p>
        <p class="card-text"> <i>{{ row.blurb | remove_first: "<br>&emsp;" | truncatewords: 30 }}</i></p>
        <button type="button" class="btn btn-primary btn-sm" data-toggle="modal" data-target="#{{ row.id }}Modal">Read More...</button>
        
        <!-- Modal -->
        <div class="modal fade" id="{{ row.id }}Modal" tabindex="-1" role="dialog" aria-labelledby="{{ row.id }}ModalLabel" aria-hidden="true">
          <div class="modal-dialog" role="document">
            <div class="modal-content">
              {% if row.image %}
              <div class="modal-header">
                <img class="aboutImage" src="{{ site.url }}{{ site.page_img_path }}/experience/{{ row.image }}" alt="{{ row.company }}">
              </div>
              {% endif %}
              <div class="modal-body">
                <h4 class="modal-title" id="{{ row.id }}ModalLabel">{{ row.company }}</h4>
                <h5 class="post-meta">{{ row.position }}</h5>
                <h6 class="post-meta">{{ row.started }} - {{ row.ended }}</h6>
                {{ row.blurb }}
                <br><br>
              </div>
              <div class="modal-footer">
                <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    {% if forloop.last != true %}
        <hr>
    {% endif %}
  {% endfor %}
</div>
