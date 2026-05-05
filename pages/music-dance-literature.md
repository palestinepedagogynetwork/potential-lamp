---
title: Music, Dance, and Literature
layout: page
permalink: /collections/musicdanceliterature.html
---

<div class="container my-4">
  <div class="row justify-content-center">
    <div class="col-lg-9">

      <h1>Music, Dance, and Literature</h1>

      <img src="{{ '/assets/img/music.jpg' | relative_url }}" 
           alt="Music, Dance, and Literature" 
           class="img-fluid d-block mx-auto mb-4"
           style="max-width:80%;">

      <h2>Introduction Video</h2>

      <div style="max-width:800px; height:400px; background:#f5f5f5; display:flex; align-items:center; justify-content:center; border:2px dashed #ccc; margin:0 auto 1.5rem auto;">
        <p style="color:#777; font-size:1.2rem;">Video coming soon</p>
      </div>

      <h2>Description</h2>

      <p>How do music, dance, performance, and literature carry a people's identity across borders, generations, and decades of displacement? This collection brings together a wide range of sources that explore how Palestinians express identity, cultural memory, and resistance through music, dance, performance, and literature.</p>

      <p>It spans from ethnomusicological, anthropological, and literary analysis stemming from cultural performance and diaspora studies that highlight how creative practices become sites of cultural continuity and political struggle across geographies and generations.</p>

      <h2>Sources</h2>
      <div class="row">
      {% for item in site.data.cluster-collection-metadata %}
      {% if item["Assigned Collection"] == "Music" %}
      <div class="col-md-4 mb-4">
      <div class="card h-100">
      <div class="card-body">
      <h5 class="card-title">{{ item.Title }}</h5>
        <p><strong>Creator:</strong> {{ item["Creator/Author"] }}</p>
        <p><strong>Type:</strong> {{ item["Item Type"] }}</p>
        <p><strong>Year:</strong> {{ item["Year Published"] }}</p>
        <a href="{{ '/items/' | append: item.objectid | append: '.html' | relative_url }}" 
            class="btn btn-primary">
          View Source
        </a>
        </div>
        </div>
        </div>
      {% endif %}
    {% endfor %}
    </div>
  </div>
</div>