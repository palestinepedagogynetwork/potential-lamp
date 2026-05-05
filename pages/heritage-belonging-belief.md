---
title: Heritage, Belonging, and Belief
layout: page
permalink: /collections/heritagebelongingbelief.html
---

<div class="container my-4">
  <div class="row justify-content-center">
    <div class="col-lg-9">

      <h1>Heritage, Belonging, and Belief</h1>

      <img src="{{ '/assets/img/heritage.jpg' | relative_url }}" 
           alt="Heritage, Belonging, and Belief" 
           class="img-fluid d-block mx-auto mb-4"
           style="max-width:80%;">

      <h2>Introduction Video</h2>

      <div style="max-width:800px; height:400px; background:#f5f5f5; display:flex; align-items:center; justify-content:center; border:2px dashed #ccc; margin:0 auto 1.5rem auto;">
        <p style="color:#777; font-size:1.2rem;">Video coming soon</p>
      </div>

      <h2>Description</h2>

      <p>
      How do Palestinians preserve their identity in the face of violence, displacement, and the steady pressure of erasure? This collection brings together sources that explore that question across four main forms of cultural transmission. Temporal transmission passes knowledge from one generation to the next. Physical transmission carries heritage through tangible objects. Oral transmission moves through spoken word and conversation, both within and across generations. Spatial transmission addresses migration, diaspora, and displacement, and how scattered communities continue to hold on to their heritage. Whether through time, objects, voice, or place, Palestinians have practiced ongoing acts of preservation to safeguard their identity. This shared, intentional act of preservation also offers something less tangible but equally vital: a sense of hope and continuity in the face of adversity.
      </p>

      <p>
      Most of the sources included are journal articles that examine how heritage is transmitted, including interviews, studies, archival documents, social media posts, and conventional research. The collection also includes other forms of media, including books and documentary films. The film <i>Stallions of Palestine</i>, for example, looks at how horses have become a core part of Palestinian identity, symbolizing resilience, pride, and cultural continuity amidst destruction. In doing so, horses represent a living history that merges endurance with heritage. Amongst the books, anthropologist Celia Rothenberg’s <i>Spirits of Palestine: Gender, Society, and the Stories of the Jinn</i> examines daily life in the West Bank village, showing how villagers claim spiritual and physical agency under occupation. Taken together, these works draw on diverse forms of media, foreground Palestinian voices, and remain accessible to a wide range of readers.
      </p>

      <p>
      Many of the sources explore Palestinian identity and heritage in diaspora communities and other contexts of displacement. These include Palestinian communities living in refugee camps, as well as Palestinians who immigrated, by force or by choice, to countries such as Australia and Chile. Several sources also examine the role of the digital world and new technologies in propagating Palestinian heritage and identity. These works explore how displaced communities build “postspatial” identities, held together by memory and connection rather than physical territory. Drawing largely on ethnographic interviews and conversations with displaced people and diaspora members, these works show how Palestinians weave their attachment to their homeland into the lives they build in new communities, through everything from food and family ritual to digital archives. Other sources highlight Palestinian women and queer communities as figures of resilience and resistance, with particular attention to women, who have long served as custodians of cultural knowledge, ritual tradition, and craft.
      </p>

      <h2>Sources</h2>
      <div class="row">
      {% for item in site.data.cluster-collection-metadata %}
      {% if item["Assigned Collection"] == "Heritage, Belonging, and Belief" %}
    
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