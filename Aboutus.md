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
}
.btn--ghost {
  background: transparent;
  border: 1px solid rgba(0,0,0,0.06);
}
.btn--primary {
  background: linear-gradient(90deg,#a45b3c,#ff7a59);
  color: #fff;
}

/* Modal (popup) */
.modal-backdrop {
  position: fixed;
  inset: 0;
  background: rgba(2,6,23,0.6);
  display: none;
  align-items: center;
  justify-content: center;
  z-index: 1200;
}
.modal-backdrop.open { display:flex; }

.modal {
  background: white;
  color: #0b1220;
  max-width: 880px;
  width: calc(100% - 40px);
  border-radius: 12px;
  padding: 20px;
  box-shadow: 0 20px 60px rgba(2,6,23,0.3);
  outline: none;
}
.modal .modal-grid {
  display:grid;
  grid-template-columns: 160px 1fr;
  gap:18px;
  align-items:start;
}
.modal .photo { width:160px; height:160px; margin:0; box-shadow:none; }
.modal h3 { margin: 0 0 6px 0; }
.modal .meta { color: #6b7280; margin-bottom: 8px; }

/* Responsive modal */
@media (max-width: 720px) {
  .modal .modal-grid { grid-template-columns: 1fr; }
  .modal .photo { width:120px; height:120px; margin: 0 auto 6px auto; }
}

/* Decorative badges */
.badges { display:flex; gap:8px; justify-content:center; margin-top:10px; }
.badge { padding:6px 8px; border-radius:999px; background:rgba(0,0,0,0.04); font-size:.82rem; color:#374151; }

/* Optional dark mode */
@media (prefers-color-scheme: dark) {
  .member { color: #e6eef8; }
  .member p.summary { color: #cbd5e1; }
  .modal { background:#081024; color: #e6eef8; }
  .modal .meta { color:#9ca3af; }
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
  <article class="member" data-bio="bio-bety">
    <div class="photo">
      <img src="{{ site.baseurl }}/assets/images/IMG_Bety.jpg" alt="Beatriz Rodríguez Hernández">
    </div>
    <h3>Beatriz Rodríguez Hernández</h3>
    <div class="role">Principal Investigator · Research Design</div>
    <p class="summary">
      Beatriz developed the original concept and research questions behind this project. She leads survey design and the interpretation of collected data.
    </p>

    <div class="actions">
      <button class="btn btn--ghost" data-open="bio-bety">Read more</button>
      <a class="btn btn--primary" href="mailto:scatteringcimarron@gmail.com">Contact</a>
    </div>
  </article>

  <!-- ===== Member 2 ===== -->
  <article class="member" data-bio="bio-gretel">
    <div class="photo">
      <img src="{{ site.baseurl }}/assets/images/20250124_144716.jpg" alt="Gretel Quintero Angulo">
    </div>
    <h3>Gretel Quintero Angulo</h3>
    <div class="role">Project Coordination · Data Analysis</div>
    <p class="summary">
      Gretel coordinates the project’s structure and workflow, contributing to data analysis, results presentation, and the technical, content, and design development of the project’s website.
    </p>

    <div class="actions">
      <button class="btn btn--ghost" data-open="bio-gretel">Read more</button>
      <a class="btn btn--primary" href="mailto:scatteringcimarron@gmail.com">Contact</a>
    </div>
  </article>

  <!-- ===== Member 3 ===== -->
  <article class="member" data-bio="bio-du">
    <div class="photo">
      <img src="{{ site.baseurl }}/assets/images/du.jpg" alt="Duvier Suárez Fontanella">
    </div>
    <h3>Duvier Suárez Fontanella</h3>
    <div class="role">Technical Lead · Data Engineering</div>
    <p class="summary">
      Duvier oversees the technical methodologies, ensuring the data is processed, visualized, and analyzed with precision and clarity.
    </p>

    <div class="actions">
      <button class="btn btn--ghost" data-open="bio-du">Read more</button>
      <a class="btn btn--primary" href="mailto:scatteringcimarron@gmail.com">Contact</a>
    </div>
  </article>
</div>

<!-- ===== Modal for full bios ===== -->
<div id="modal-root">
  <div class="modal-backdrop" id="modal-backdrop" aria-hidden="true">
    <div class="modal" id="modal-content">
      <div class="modal-grid">
        <div class="photo" id="modal-photo">
          <img src="" alt="">
        </div>
        <div>
          <h3 id="modal-name">Name</h3>
          <div class="meta" id="modal-role">Role</div>
          <div id="modal-bio"></div>
          <div style="margin-top:8px; display:flex; gap:8px;">
            <a id="modal-email" class="btn btn--primary" href="#">Contact</a>
            <button id="modal-close" class="btn btn--ghost">Close</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<script>
(() => {
  const backdrop = document.getElementById('modal-backdrop');
  const modal = document.getElementById('modal-content');
  const modalName = document.getElementById('modal-name');
  const modalRole = document.getElementById('modal-role');
  const modalBio = document.getElementById('modal-bio');
  const modalPhoto = document.querySelector('#modal-photo img');
  const modalEmail = document.getElementById('modal-email');
  const modalClose = document.getElementById('modal-close');

  const bios = {
    "bio-bety": {
      name: "Beatriz Rodríguez Hernández",
      role: "Principal Investigator · Research Design",
      photo: "{{ site.baseurl }}/assets/images/IMG_Bety.jpg",
      email: "scatteringcimarron@gmail.com",
      text: `<p><strong>Beatriz</strong> is the creator of the project and developed the original concept and research questions. She designed the survey instruments and leads the analysis and interpretation of the data. Her work ensures the research methods capture the complexity of academic and professional trajectories, enabling solid, meaningful conclusions.</p>`
    },
    "bio-gretel": {
      name: "Gretel Quintero Angulo",
      role: "Project Coordination · Data Analysis",
      photo: "{{ site.baseurl }}/assets/images/20250124_144716.jpg",
      email: "scatteringcimarron@gmail.com",
      text: `<p><strong>Gretel</strong> coordinates the project’s structure and workflow. Her work includes data collection and analysis, preparation and presentation of research results, and the technical and content development of the project’s website. She also contributes to the project’s design to ensure its outcomes are coherent, engaging, and accessible.</p>`
    },
    "bio-du": {
      name: "Duvier Suárez Fontanella",
      role: "Technical Lead · Data Engineering",
      photo: "{{ site.baseurl }}/assets/images/du.jpg",
      email: "scatteringcimarron@gmail.com",
      text: `<p><strong>Duvier</strong> leads the technical aspects of the project, focusing on data processing, metrics, website deveplopment and visualization strategies. His expertise ensures that data analysis is rigorous and accessible, transforming complex information into clear, actionable insights.</p>`
    }
  };

  document.querySelectorAll('[data-open]').forEach(btn => {
    btn.addEventListener('click', () => {
      const key = btn.getAttribute('data-open');
      const data = bios[key];
      modalName.textContent = data.name;
      modalRole.textContent = data.role;
      modalBio.innerHTML = data.text;
      modalPhoto.src = data.photo;
      modalPhoto.alt = data.name;
      modalEmail.href = "mailto:" + data.email;
      backdrop.classList.add('open');
      document.body.style.overflow = 'hidden';
    });
  });

  function closeModal() {
    backdrop.classList.remove('open');
    document.body.style.overflow = '';
  }

  modalClose.addEventListener('click', closeModal);
  backdrop.addEventListener('click', e => { if (e.target === backdrop) closeModal(); });
  document.addEventListener('keydown', e => { if (e.key === 'Escape') closeModal(); });
})();
</script>
