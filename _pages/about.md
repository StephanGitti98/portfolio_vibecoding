---
permalink: /
title: "Ihm.Space"
layout: glass-home
redirect_from: 
  - /about/
  - /about.html
---

<section class="ihm-hero scroll-reveal" data-delay="0">
  <div class="ihm-hero-content">
    <h1 class="ihm-hero-title">Concept and Visualisation of interactive digital and physical products.</h1>
    <p class="ihm-hero-subtitle">I'm Stephan, a passionate UI designer focused on creating ideas for digital and physical products. I enjoy bringing these two aspects together to craft seamless and engaging user experiences.</p>
    <p class="ihm-hero-location">Based in Nuremberg, Germany</p>
  </div>
</section>

<section class="ihm-work" id="work">
  <div class="ihm-section-header scroll-reveal" data-delay="0">
    <h2 class="ihm-section-title">Work</h2>
  </div>
  
  <div class="ihm-work-grid">
    <a href="/work/viewport/" class="ihm-work-item featured scroll-reveal" data-delay="0">
      <img src="/images/viewport_teaser.png" alt="ViewPort" class="ihm-work-image">
      <div class="ihm-work-info">
        <h3 class="ihm-work-title">ViewPort <span class="ihm-arrow">→</span></h3>
        <span class="ihm-work-category">Remote Office Concept</span>
      </div>
    </a>
    
    <a href="/work/ambientsound/" class="ihm-work-item scroll-reveal" data-delay="100">
      <img src="/images/ambient_teaser.png" alt="Ambient&Sound" class="ihm-work-image">
      <div class="ihm-work-info">
        <h3 class="ihm-work-title">Ambient&Sound <span class="ihm-arrow">→</span></h3>
        <span class="ihm-work-category">Speaker Concept</span>
      </div>
    </a>
    
    <a href="/work/airforce/" class="ihm-work-item scroll-reveal" data-delay="200">
      <img src="/images/airforce_teaser.png" alt="AirForce Keyvisual" class="ihm-work-image">
      <div class="ihm-work-info">
        <h3 class="ihm-work-title">AirForce Keyvisual <span class="ihm-arrow">→</span></h3>
        <span class="ihm-work-category">Brand campaign</span>
      </div>
    </a>
  </div>
</section>

<section class="ihm-about" id="about">
  <div class="ihm-section-header scroll-reveal" data-delay="0">
    <h2 class="ihm-section-title">About</h2>
  </div>
  
  <div class="ihm-about-grid">
    <div class="ihm-about-left scroll-reveal" data-delay="0">
      <p class="ihm-about-text">I started building my skills early as a freelancer and gained experience in various industries. My first project was creating and visualising content for transparent display solutions.</p>
      <p class="ihm-about-text">In recent years, I've worked on supporting startup ideas, optimizing product staging on amazon. And did public relations for medium-sized companies, local organizations for innovative progress and public institutions like universities and museums.</p>
      <p class="ihm-about-text">During my studies, I focused on designing interactive interfaces and graduated in Interaction Design. I continue to educate myself in this field. Since then, I have been working at an agency for industrial communication, contributing to the design and implementation of applications for trade shows, sales, and organization.</p>
      <a href="/cv/" class="ihm-cv-button">View full CV →</a>
    </div>
    
    <div class="ihm-about-right scroll-reveal" data-delay="100">
      <div class="ihm-detail-group">
        <p class="ihm-detail-label">Freelance Designer</p>
        <p class="ihm-detail-value">Multidisciplinary</p>
        <p class="ihm-detail-subtext">Currently - More than 4 years</p>
      </div>
      
      <div class="ihm-detail-group">
        <p class="ihm-detail-label">Bachelor Degree</p>
        <p class="ihm-detail-value">Interaction Design</p>
        <p class="ihm-detail-subtext">2021</p>
      </div>
      
      <div class="ihm-detail-group">
        <p class="ihm-detail-label">Employee</p>
        <p class="ihm-detail-value">UX Designer</p>
        <p class="ihm-detail-subtext">Since 2020</p>
      </div>
    </div>
  </div>
</section>

<section class="ihm-skills" id="skills">
  <div class="ihm-section-header scroll-reveal" data-delay="0">
    <h2 class="ihm-section-title">Concept & Wireframe</h2>
  </div>
  
  <ul class="ihm-skills-list scroll-reveal" data-delay="100">
    <li>User Interface Design</li>
    <li class="muted">3D & Animation</li>
    <li class="muted">Product Visualisation</li>
  </ul>
</section>

<section class="ihm-contact" id="contact">
  <div class="ihm-section-header scroll-reveal" data-delay="0">
    <h2 class="ihm-section-title">Get in touch</h2>
  </div>
  
  <div class="ihm-contact-content scroll-reveal" data-delay="100">
    <h2 class="ihm-contact-title">Let's work together</h2>
    <p class="ihm-contact-text">Do you have a question or just want to talk to me? Write me an email or dm me on LinkedIn.</p>
    <a href="mailto:hello@example.com" class="ihm-contact-button">Email me →</a>
  </div>
</section>

<footer class="ihm-footer scroll-reveal" data-delay="0">
  <div class="ihm-footer-content">
    <div class="ihm-footer-left">
      <p class="ihm-footer-name">Stephan — UI Designer</p>
      <p class="ihm-footer-location">based in Nuremberg</p>
      <p class="ihm-footer-copyright">©2024 to ∞</p>
    </div>
  </div>
</footer>

<script>
// Staggered scroll reveal animation
document.addEventListener('DOMContentLoaded', function() {
  const observerOptions = {
    threshold: 0.15,
    rootMargin: '0px 0px -50px 0px'
  };

  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        const delay = parseInt(entry.target.dataset.delay) || 0;
        setTimeout(() => {
          entry.target.classList.add('revealed');
        }, delay);
        observer.unobserve(entry.target);
      }
    });
  }, observerOptions);

  document.querySelectorAll('.scroll-reveal').forEach(el => {
    observer.observe(el);
  });
});
</script>
