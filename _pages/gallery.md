---
layout: archive
title: "Gallery"
permalink: /gallery/
author_profile: true
---

<style>
.gallery-container {
  margin: 20px 0;
}

.gallery-section {
  margin-bottom: 40px;
}

.gallery-section h2 {
  color: #494e52;
  border-bottom: 2px solid #f2f3f3;
  padding-bottom: 10px;
  margin-bottom: 20px;
  font-size: 1.5em;
}

.image-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
  margin-bottom: 30px;
}

.image-item {
  background: #fff;
  border-radius: 8px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  overflow: hidden;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.image-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 5px 20px rgba(0,0,0,0.15);
}

.image-item img {
  width: 100%;
  height: 250px;
  object-fit: cover;
  display: block;
}

.image-caption {
  padding: 15px;
  text-align: center;
}

.image-caption h3 {
  margin: 0 0 8px 0;
  font-size: 1.1em;
  color: #333;
}

.image-caption p {
  margin: 0;
  color: #666;
  font-size: 0.9em;
  line-height: 1.4;
}

.lightbox {
  display: none;
  position: fixed;
  z-index: 1000;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0,0,0,0.9);
}

.lightbox-content {
  display: block;
  margin: auto;
  max-width: 90%;
  max-height: 90%;
  margin-top: 2%;
}

.close {
  position: absolute;
  top: 15px;
  right: 35px;
  color: #f1f1f1;
  font-size: 40px;
  font-weight: bold;
  cursor: pointer;
}

.close:hover {
  color: #bbb;
}

@media (max-width: 768px) {
  .image-grid {
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 15px;
  }
  
  .image-item img {
    height: 200px;
  }
}
</style>

<div class="gallery-container">
  
  <div class="gallery-section">
    <h2>🏆 Competitions & Awards</h2>
    <div class="image-grid">
      
      <div class="image-item">
        <img src="/images/Huawei ICT Regional Finals Riyadh.DNG" alt="Huawei ICT Competition Regional Finals" onclick="openLightbox('/images/Huawei ICT Regional Finals Riyadh.DNG')">
        <div class="image-caption">
          <h3>Huawei ICT Competition Regional Finals</h3>
          <p>Participating in the Huawei ICT Competition Regional Finals in Riyadh, showcasing technical skills and innovation in ICT.</p>
        </div>
      </div>
      
      <div class="image-item">
        <img src="/images/Huawei ICT Regional Finals Riyadh 02.DNG" alt="Huawei ICT Competition Team" onclick="openLightbox('/images/Huawei ICT Regional Finals Riyadh 02.DNG')">
        <div class="image-caption">
          <h3>ICT Competition Team</h3>
          <p>Team collaboration and technical excellence at the Huawei ICT Competition Regional Finals.</p>
        </div>
      </div>
      
    </div>
  </div>

  <div class="gallery-section">
    <h2>🎓 Conferences & Academic Events</h2>
    <div class="image-grid">
      
      <div class="image-item">
        <img src="/images/AI in Medicine Conference April 2025.DNG" alt="AI in Medicine Conference" onclick="openLightbox('/images/AI in Medicine Conference April 2025.DNG')">
        <div class="image-caption">
          <h3>AI in Medicine Conference</h3>
          <p>Attending the AI in Medicine Conference in April 2025, exploring the intersection of artificial intelligence and healthcare.</p>
        </div>
      </div>
      
      <div class="image-item">
        <img src="/images/MITACS GRI at Dalhousie University.DNG" alt="MITACS GRI at Dalhousie University" onclick="openLightbox('/images/MITACS GRI at Dalhousie University.DNG')">
        <div class="image-caption">
          <h3>MITACS GRI - Dalhousie University</h3>
          <p>Participating in the MITACS Globalink Research Internship program at Dalhousie University, engaging in cutting-edge research.</p>
        </div>
      </div>
      
    </div>
  </div>

  <div class="gallery-section">
    <h2>📸 Professional & Personal</h2>
    <div class="image-grid">
      
      <div class="image-item">
        <img src="/images/bio-photo.jpg" alt="Professional Photo" onclick="openLightbox('/images/bio-photo.jpg')">
        <div class="image-caption">
          <h3>Professional Portrait</h3>
          <p>Professional headshot showcasing my commitment to excellence in software engineering and research.</p>
        </div>
      </div>
      
      <div class="image-item">
        <img src="/images/editing-talk.png" alt="Technical Presentation" onclick="openLightbox('/images/editing-talk.png')">
        <div class="image-caption">
          <h3>Technical Presentation</h3>
          <p>Delivering a technical presentation, sharing knowledge and insights with the community.</p>
        </div>
      </div>
      
    </div>
  </div>

</div>

<!-- Lightbox Modal -->
<div id="lightbox" class="lightbox" onclick="closeLightbox()">
  <span class="close">&times;</span>
  <img class="lightbox-content" id="lightbox-img">
</div>

<script>
function openLightbox(imageSrc) {
  document.getElementById('lightbox').style.display = 'block';
  document.getElementById('lightbox-img').src = imageSrc;
  document.body.style.overflow = 'hidden';
}

function closeLightbox() {
  document.getElementById('lightbox').style.display = 'none';
  document.body.style.overflow = 'auto';
}

// Close lightbox on Escape key
document.addEventListener('keydown', function(event) {
  if (event.key === 'Escape') {
    closeLightbox();
  }
});
</script>