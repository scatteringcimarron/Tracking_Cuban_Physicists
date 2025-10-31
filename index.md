---
layout: default
title: Welcome
---

Welcome to the Scattering Cimarrón webpage! 

This project investigates the academic and professional trajectories of Cuban physicists. It aims to understand what motivates individuals to choose this career path, which factors influence their decision to remain in or leave the academic field, and how personal, social, and economic expectations play a role. 

Through interviews, surveys, and document analysis, the project seeks to build a database that helps identify common patterns. It also aims to compare these trajectories with international experiences to understand how the Cuban context aligns with or differs from global trends. 

If you would like to learn more about the project’s scope, methods, and goals, we invite you to explore the <a href="{{ site.baseurl }}/Project/">Project Overview</a> page. If you want to see its preliminary results, please go to <a href="{{ site.baseurl }}/Promo_2010_2024/">FF-UH Promotions 2010–2024</a>. To meet the team behind this initiative, you can visit the <a href="{{ site.baseurl }}/Aboutus/">About Us</a> section and if you want to contact us you can do it at <a href="mailto:scatteringcimarron@gmail.com">scatteringcimarron@gmail.com</a>.

**If you are a Cuban physicist, we warmly invite you to contribute to the project by completing its current [survey](https://docs.google.com/forms/d/e/1FAIpQLSfGiiMZC318qADo4sACnMVblrxAcXENCLykBp2Od84bQNqNnA/viewform).**

<!-- ===== Page views counter (CountAPI with automatic fallback) ===== -->
<p id="page-views" style="text-align:center; margin-top:28px; font-size:0.95rem; color:#555;">
  👁️ Loading views...
</p>

<script>
  (async () => {
    const NS = 'scatteringcimarron';   // cambia si quieres separar entornos
    const KEY = 'welcome';              // único por página
    const ENDPOINT = 'https://api.countapi.xyz';
    const el = document.getElementById('page-views');

    try {
      // 1) Crear la clave si no existe (no rompe si ya existe)
      await fetch(`${ENDPOINT}/create?namespace=${encodeURIComponent(NS)}&key=${encodeURIComponent(KEY)}&value=0`, { mode: 'cors' }).catch(() => {});
      // 2) Incrementar contador y mostrar
      const res = await fetch(`${ENDPOINT}/hit/${encodeURIComponent(NS)}/${encodeURIComponent(KEY)}`, { mode: 'cors' });
      if (!res.ok) throw new Error('CountAPI not ok: ' + res.status);
      const data = await res.json();
      el.textContent = `👁️ ${data.value} views`;
    } catch (err) {
      // 3) Fallback: badge estático para que siempre se vea algo
      el.innerHTML = `
        <img src="https://visitorbadge.io/status?path=${encodeURIComponent(NS + '.' + KEY)}&label=Page%20views&style=flat&color=ff7a59"
             alt="Page views for Welcome page">
      `;
    }
  })();
</script>

