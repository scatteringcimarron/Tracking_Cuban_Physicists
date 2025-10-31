---
layout: default
title: About us
permalink: /Aboutus/
---

<style>
/* ===== Modern "About Us" styles ===== */
.team-hero {
  text-align: center;
  margin: 12px 0 28px;
}
.team-hero h1 {
  font-family: "PT Serif", serif;
  font-size: 2rem;
  margin: 6px 0;
}
.team-hero p.lead {
  color: #6b7280;
  margin: 0;
  font-size: 1rem;
}

/* Grid layout */
.team-grid {
  display: grid;
  gap: 28px;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  align-items: start;
  margin-top: 32px;
}

/* Member card */
.member {
  background: linear-gradient(180deg, rgba(255,255,255,0.02), transparent);
  padding: 20px;
  border-radius: 14px;
  box-shadow: 0 8px 20px rgba(2,6,23,0.06);
  transition: transform .18s ease, box-shadow .18s ease;
  display:flex;
  flex-direction:column;
  gap:12px;
}
.member:hover {
  transform: translateY(-6px);
  box-shadow: 0 18px 40px rgba(2,6,23,0.12);
}

/* Profile photo */
.member .photo {
  width: 120px;
  height: 120px;
  border-radius: 999px;
  overflow: hidden;
  margin: 0 auto;
  box-shadow: 0 6px 18px rgba(2,6,23,0.12);
}
.member .photo img {
  width:100%;
  height:100%;
  object-fit: cover;
  transition: transform .5s ease;
}
.member:hover .photo img { transform: scale(1.05); }

/* Name and role */
.member h3 {
  text-align:center;
  margin: 6px 0 4px;
  font-family: "PT Serif", serif;
  font-size: 1.05rem;
}
.member .role {
  text-align:center;
  color: #6b7280;
  font-size: .92rem;
}

/* Short summary */
.member p.summary {
  color: #374151;
  font-size: .95rem;
  text-align: justify;
  margin: 0;
}

/* Buttons */
.member .actions {
  display:flex;
  gap:8px;
  justify-content:center;
  margin-top: 8px;
}
.btn {
  padding:8px 12px;
  border-radius: 10px;
  border: none;
  cursor:pointer;
  font-weight:700;
  font-size:.9rem;
  text-decoration:none;
  text-align:center;
}
.btn--ghost {
  background: transparent;
  border: 1px solid rgba(0,0,0,0.06);
  color: #374151;
}
.btn--ghost:hover {
  background: rgba(0,0,0,0.04);
}
.btn--primary {
  background: linear-gradient(90deg,#a45b3c,#ff7a59);
  color: #fff;
}

/* Decorative badges */
.badges { display:flex; gap:8px; justify-content:center; margin-top:10px; }
.badge { padding:6px 8px; border-radius:999px; background:rgba(0,0,0,0.04); font-size:.82rem; color:#374151; }

/* Optional dark mode */
@media (prefers-color-scheme: dark) {
  .member { color: #e6eef8; }
  .member p.summary { color: #cbd5e1; }
}
</style>

<div class="team-hero">
  <h1>Meet the <em>cimarrones</em></h1>
  <p class="lead">The team behind the vision, research, and development of this project.</p>

  <div class="badges" aria-hidden="true">
    <span class="badge">🔬 Research</span>
    <span class="badge">📊 Data Analysis</span>
    <span class="badge">🌍 Collaboration</span>
  </div>
</div>

<div class="team-grid">

  <!-- ===== Member 1 ===== -->
  <article class="member">
    <div class="photo">
      <img src="{{ site.baseurl }}/assets/images/IMG_Bety.jpg" alt="Beatriz Rodríguez Hernández">
    </div>
    <h3>Beatriz Rodríguez Hernández</h3>
    <div class="role">Principal Investigator · Research Design</div>
    <p class="summary">
      Beatriz developed the original concept and research questions behind this project. She leads survey design and the interpretation of collected data.
    </p>

    <div class="actions">
      <a class="btn btn--ghost" href="https://www.linkedin.com/in/beatriz-rodriguez-hernandez/" target="_blank">Read more</a>
      <a class="btn btn--primary" href="mailto:scatteringcimarron@gmail.com">Contact</a>
    </div>
  </article>

  <!-- ===== Member 2 ===== -->
  <article class="member">
    <div class="photo">
      <img src="{{ site.baseurl }}/assets/images/20250124_144716.jpg" alt="Gretel Quintero Angulo">
    </div>
    <h3>Gretel Quintero Angulo</h3>
    <div class="role">Project Coordination · Data Analysis</div>
    <p class="summary">
      Gretel coordinates the project’s structure and workflow, contributing to data analysis, results presentation, and the technical, content, and design development of the project’s website.
    </p>

    <div class="actions">
      <a class="btn btn--ghost" href="https://www.linkedin.com/in/gretel-quintero-angulo/" target="_blank">Read more</a>
      <a class="btn btn--primary" href="mailto:scatteringcimarron@gmail.com">Contact</a>
    </div>
  </article>

  <!-- ===== Member 3 ===== -->
  <article class="member">
    <div class="photo">
      <img src="{{ site.baseurl }}/assets/images/du.jpg" alt="Duvier Suárez Fontanella">
    </div>
    <h3>Duvier Suárez Fontanella</h3>
    <div class="role">Technical Lead · Data Engineering</div>
    <p class="summary">
      Duvier oversees the technical methodologies, ensuring the data is processed, visualized, and analyzed with precision and clarity.
    </p>

    <div class="actions">
      <a class="btn btn--ghost" href="https://www.linkedin.com/in/duvier-suarez-fontanella/" target="_blank">Read more</a>
      <a class="btn btn--primary" href="mailto:scatteringcimarron@gmail.com">Contact</a>
    </div>
  </article>
</div>
