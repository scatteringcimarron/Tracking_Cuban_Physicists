---
layout: default
title: Welcome
---

Welcome to the Scattering Cimarrón webpage! 

This project investigates the academic and professional trajectories of Cuban physicists. It aims to understand what motivates individuals to choose this career path, which factors influence their decision to remain in or leave the academic field, and how personal, social, and economic expectations play a role. 

Through interviews, surveys, and document analysis, the project seeks to build a database that helps identify common patterns. It also aims to compare these trajectories with international experiences to understand how the Cuban context aligns with or differs from global trends. 

If you would like to learn more about the project’s scope, methods, and goals, we invite you to explore the <a href="{{ site.baseurl }}/Project/">Project Overview</a> page. If you want to see its preliminary results, please go to <a href="{{ site.baseurl }}/Promo_2010_2024/">FF-UH Promotions 2010–2024</a>. To meet the team behind this initiative, you can visit the <a href="{{ site.baseurl }}/Aboutus/">About Us</a> section and if you want to contact us you can do it at <a href="mailto:scatteringcimarron@gmail.com">scatteringcimarron@gmail.com</a>.

**If you are a Cuban physicist, we warmly invite you to contribute to the project by completing its current [survey](https://docs.google.com/forms/d/e/1FAIpQLSfGiiMZC318qADo4sACnMVblrxAcXENCLykBp2Od84bQNqNnA/viewform).**

<!-- ===== Page views counter ===== -->
<p id="page-views" style="text-align:center; margin-top:28px; font-size:0.95rem; color:#555;">
  👁️ Loading views...
</p>

<script>
  // Simple view counter using CountAPI
  fetch('https://api.countapi.xyz/hit/scatteringcimarron/welcome')
    .then(response => response.json())
    .then(data => {
      document.getElementById('page-views').textContent = `👁️ ${data.value} views`;
    })
    .catch(() => {
      document.getElementById('page-views').textContent = '👁️ Views unavailable';
    });
</script>
