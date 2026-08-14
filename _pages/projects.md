---
title:
layout: default
permalink: /projects/
published: true
---


<div class="ProjectContainer">

  <h2 class="ProjectSectionTitle">University of Tübingen &mdash; Postdoc</h2>
  <div class="gallery">

  {% for project in site.projects %}
  {% if project.affiliation == "Tuebingen" %}

  {% if project.redirect %}
  <div class="projectTile">
          <a href="{{ project.redirect }}" target="_blank">
          <span>
              <h2>{{ project.title }}</h2>
              <br/>
              <p>{{ project.description }}</p>
          </span>
          </a>
  </div>

  {% else %}

  <div class="projectTile">
          <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
          <span>
              <h2>{{ project.title }}</h2>
              <br/>
              <p>{{ project.description }}</p>
          </span>
          </a>
  </div>

  {% endif %}

  {% endif %}
  {% endfor %}

	</div>

  <h2 class="ProjectSectionTitle">University of Plymouth &mdash; PhD</h2>
  <div class="gallery">

  {% for project in site.projects %}
  {% if project.affiliation == "Plymouth" %}

  {% if project.redirect %}
  <div class="projectTile">
          <a href="{{ project.redirect }}" target="_blank">
          <span>
              <h2>{{ project.title }}</h2>
              <br/>
              <p>{{ project.description }}</p>
          </span>
          </a>
  </div>

  {% else %}

  <div class="projectTile">
          <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
          <span>
              <h2>{{ project.title }}</h2>
              <br/>
              <p>{{ project.description }}</p>
          </span>
          </a>
  </div>

  {% endif %}

  {% endif %}
  {% endfor %}

	</div>

</div>
