---
title: "Accueil"
---

<div class="content-wrapper">

<div class="intro-cv">
  <div class="location">
    <i class="fa-solid fa-location-dot"></i> Copenhagen
  </div>
</div>
<!-- Bloc centré avec photo -->
<div class="profile-container">
  <img src="/Personal_Portfolio/images/Corporate_detouree_carree.png"
       alt="Ma photo" class="profile-photo"/>
  <div class="profile-text">
    <h1 style="transition: transform 0.3s ease;"
        onmouseover="this.style.transform='scale(1.1)'"
        onmouseout="this.style.transform='scale(1)'">Zian Cassassolles</h1>
    <h2 style="transition: transform 0.3s ease"
        onmouseover="this.style.transform='scale(1.1)'"
        onmouseout="this.style.transform='scale(1)'">Digital Transformation Engineer<span style="color:#9013fe">.</span></h2>
    <h4 style="max-width: 600px;min-height: 7rem;"><span style="color:#9013fe">></span><span id="typed-text" style="white-space: pre-wrap;"></span><span id="cursor">|</span>
    </h4>
  </div>
</div>

<!-- Début CV -->
<h2 style="text-align:left;">Resume</h2>
<!-- Début Intro -->
<div class="intro-cv">
<p>
  Hi, I'm Zian, an ambitious and proactive engineer with a passion for science, digital transformation, data and finance.
  My mission: to drive operational excellence and deliver measurable impact through smart process optimisation and data-driven decision-making.
</p>
<!-- <p class="separateur"></p> -->
</div>
<section id="about" style="margin-top: 0rem;">
  <!-- Première tab -->
  <div class="tabs">
    <input type="radio" name="tabs" id="tab1" checked>
    <input type="radio" name="tabs" id="tab2">
    <input type="radio" name="tabs" id="tab3">
    <input type="radio" name="tabs" id="tab4">

  <div class="tabs-nav">
      <div class="tabs-nav">
        <label for="tab1" class="tab-label">💼 Experience</label>
        <label for="tab2" class="tab-label">🎓 Education</label>
        <label for="tab3" class="tab-label">📜 Certifications</label>
</div>
    </div>

  <div class="content">
      <div id="content1" class="tab-content">
        <ul>
          <h3 class="tab-title-entry">Digital Transformation Engineer<span class="date">2024 – Present</span>
          </h3>
          <li class="location">Alstom - Copenhagen, Denmark</li>
            <li class="item">Designed ETL pipelines and global dashboards to monitor project progress, enhancing project transparency and decision-making.</li>
            <li class="item last-item">Web interface</li>
        </ul>
        <ul>
          <h3 class="tab-title-entry with-separator">Test and Commissioning Engineer</span> <span class="date">2022 – 2024</h3>
          <li class="location">Alstom - Copenhagen, Denmark</li>
            <li></li>
        </ul>
      </div>
      <div id="content2" class="tab-content">
        <ul style="padding: 0;">
          <li><span class="date">2021 – 2022</span><span> M. Sc - Linköping Institute of Technology – Sweden</span></li>
          <li><span class="date">2019 – 2022</span><span> M.Sc - Arts et Métiers ParisTech – France</span></li>
        </ul>
      </div>
      <div id="content3" class="tab-content">
        <ul>
          <li>Alstom - Six Sigma Yellow Belt Certification <span class="date">2024</span></li>
        </ul>
      </div>
      <div id="content4" class="tab-content">
      </div>
    </div>
  </div>
</section>

<!-- Deuxième tab -->
<section id="second-tabs" style="margin-top: 1rem;">
  <h2 style="text-align:left;">Strenghts</h2>

  <!-- <div class="tabs">
    <input type="radio" name="tabs2" id="tab2-1" checked>
    <input type="radio" name="tabs2" id="tab2-2">
    <input type="radio" name="tabs2" id="tab2-3">
    <div class="tabs-nav">
      <label for="tab2-1" class="tab-label">🚀 Projects</label>
      <label for="tab2-2" class="tab-label">🌍 Passions</label>
      <label for="tab2-3" class="tab-label">📸 Media</label>
    </div>
    <div class="content">
      <div id="content2-1" class="tab-content">
        <div class="skills-columns">
          <ul>
            <h3 style="text-align:center;margin-bottom: 1rem">🔧  Competencies</h3>
            <li>Data Analysis</li>
            <li>Project Management</li>
          </ul>
          <ul>
            <h3 style="text-align:center;margin-bottom: 1rem">⚙️ Tools</h3>
            <li>Ms Office, PowerBI, PowerApps</li>
            <li>Python - Django, Pandas</li>
            <li>HTML / CSS / JavaScript</li>
          </ul>
        </div>
      </div>
      <div id="content2-2" class="tab-content">
        <p>→ Sports, voyage, drone, musique…</p>
      </div>
      <div id="content2-3" class="tab-content">
        <p>→ Gallerie photos ou vidéos ?</p>
      </div>
    </div>
  </div> -->
</section>

<!-- Script typing machine -->
<script>
  const phrases = [
    " From raw data to real decisions — turning numbers into narratives that move business forward.",
    " Digital transformation starts with data — because insight drives impact.",
    " You can’t optimize what you don’t understand — and data is the language of understanding."
  ];

  const textEl = document.getElementById("typed-text");
  const cursorEl = document.getElementById("cursor");
  let phraseIndex = 0;
  let charIndex = 0;
  let isDeleting = false;

  function type() {
    const currentPhrase = phrases[phraseIndex];
    const displayedText = currentPhrase.substring(0, charIndex);
    textEl.textContent = displayedText;

    if (!isDeleting && charIndex < currentPhrase.length) {
      charIndex++;
      setTimeout(type, 20);
    } else if (!isDeleting && charIndex === currentPhrase.length) {
      // Wait before deleting
      setTimeout(() => {
        isDeleting = true;
        type();
      }, 4000);
    } else if (isDeleting && charIndex > 0) {
      charIndex--;
      setTimeout(type, 10);
    } else if (isDeleting && charIndex === 0) {
      // Move to next phrase
      isDeleting = false;
      phraseIndex = (phraseIndex + 1) % phrases.length;
      setTimeout(type, 500);
    }
  }

  document.addEventListener("DOMContentLoaded", () => {
    type();
  });
</script>

</div>