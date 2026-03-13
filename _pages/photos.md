---
layout: archive
title: "Photos"
permalink: /photos/
author_profile: false
---

<div class="photo-masonry">

  <div class="photo-card">
    <img src="/images/GioWistful.jpg" alt="Giovanna in deep reflection" onclick="openLightbox('/images/GioWistful.jpg', 'Giovanna in deep reflection')">
    <div class="photo-overlay">
      Giovanna in deep reflection
    </div>
  </div>

  <div class="photo-card">
    <img src="/images/GioKelleyNewScrubs.jpg" alt="Brand new scrubs" onclick="openLightbox('/images/GioKelleyNewScrubs.jpg', 'Brand new scrubs')">
    <div class="photo-overlay">
      Brand new scrubs
    </div>
  </div>

  <div class="photo-card">
    <img src="/images/AryanWithData.jpg" alt="Aryan making discoveries" onclick="openLightbox('/images/AryanWithData.jpg', 'Aryan making discoveries')">
    <div class="photo-overlay">
      Aryan making discoveries
    </div>
  </div>

  <div class="photo-card">
    <img src="/images/RisArWorking.jpg" alt="That histology though" onclick="openLightbox('/images/RisArWorking.jpg', 'That histology though')">
    <div class="photo-overlay">
      That histology though
    </div>
  </div>

  <div class="photo-card">
    <img src="/images/GZRNworking.jpg" alt="In the lab we are all family" onclick="openLightbox('/images/GZRNworking.jpg', 'In the lab we are all family')">
    <div class="photo-overlay">
      In the lab we are all family
    </div>
  </div>

  <div class="photo-card">
    <img src="/images/GioPup.jpg" alt="Lab mascot" onclick="openLightbox('/images/GioPup.jpg', 'Lab mascot')">
    <div class="photo-overlay">
      Lab mascot
    </div>
  </div>

</div>

<div id="lightbox" class="lightbox" onclick="closeLightbox(event)">
  <span class="lightbox-close" onclick="closeLightbox(event)">&times;</span>
  <img id="lightbox-img" class="lightbox-content" src="" alt="">
  <div id="lightbox-caption" class="lightbox-caption"></div>
</div>

<script>
  function openLightbox(src, caption) {
    document.getElementById('lightbox').style.display = 'flex';
    document.getElementById('lightbox-img').src = src;
    document.getElementById('lightbox-caption').textContent = caption;
    document.body.style.overflow = 'hidden';
  }

  function closeLightbox(event) {
    if (
      event.target.id === 'lightbox' ||
      event.target.classList.contains('lightbox-close')
    ) {
      document.getElementById('lightbox').style.display = 'none';
      document.getElementById('lightbox-img').src = '';
      document.body.style.overflow = '';
    }
  }

  document.addEventListener('keydown', function(event) {
    if (event.key === 'Escape') {
      document.getElementById('lightbox').style.display = 'none';
      document.getElementById('lightbox-img').src = '';
      document.body.style.overflow = '';
    }
  });
</script>
