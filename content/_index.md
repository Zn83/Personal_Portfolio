---
title: "Accueil"
---

<style>
.profile-container {
  display: flex;
  align-items: flex-start;
  justify-content: center;
  flex-wrap: wrap;
  gap: 1rem;
  max-width: 900px;
  margin: 2rem auto;
}

.profile-photo {
  width: 180px;
  height: 180px;
  border-radius: 50%;
  object-fit: cover;
}

.profile-text {
  flex: 1 1 300px;
  max-width: 500px;
  text-align: left;
}

/* .profile-text h1 { background: rgba(255,0,0,0.1); }
.profile-text h2 { background: rgba(0,255,0,0.1); }
.profile-text h4 { background: rgba(0,0,255,0.1); } */

.profile-text h1 {
  margin: 2;
  font-size: 2rem;
}

.profile-text h2 {
  margin: 1.5rem 0 0;
  font-weight: 400;
}

.profile-text h4 {
  margin: 1rem 0 0; /* Top Left Bottom */
  font-weight: 200;
}

#typed-text {
  white-space: pre-wrap;
  display: inline;
}

#cursor {
  animation: blink 1s infinite;
  font-weight: bold;
}

@keyframes blink {
  0%, 100% { opacity: 1; }
  50% { opacity: 0; }
}

/* Les tabs */
.tabs {
  max-width: 800px;
  margin: 2rem auto;
  font-family: inherit;
}

/* On masque les radio buttons mais on garde leur marge à gauche */
input[type="radio"] {
  display: none;
  margin-left: 1rem;
}

/* Navigation */
.tabs-nav {
  display: flex;
  justify-content: flex-start; /* Aligne à gauche */
  gap: 0rem;
  margin-bottom: 0rem;
}

/* Tab labels */
.tab-label {
  padding: 0.5rem 1rem;
  cursor: pointer;
  background: #eee;
  color: #000;
  border-radius: 8px 8px 0 0;
  transition: all 0.3s ease;
  font-weight: 500;
  position: relative;
}

.tab-label:hover {
  background-color: #ddd;
  transform: translateY(-2px);
}

/* Soulignement animé */
.tab-label::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -3px;
  height: 2px;
  width: 0;
  background: #000;
  transition: width 0.3s ease;
}

.tab-label:hover::after {
  width: 100%;
}

/* Onglet actif */
#tab1:checked ~ .tabs-nav label[for="tab1"]::after,
#tab2:checked ~ .tabs-nav label[for="tab2"]::after,
#tab3:checked ~ .tabs-nav label[for="tab3"]::after,
#tab4:checked ~ .tabs-nav label[for="tab4"]::after {
  width: 100%;
}

/* Contenu */
.tab-content {
  display: none;
  padding: 2rem;
  background: #f9f9f9;
  border-radius: 0 8px 8px 8px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.1);
  animation: fadeIn 0.4s ease;
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}

#tab1:checked ~ .content #content1,
#tab2:checked ~ .content #content2,
#tab3:checked ~ .content #content3,
#tab4:checked ~ .content #content4 {
  display: block;
}

/* 2 colonnes pour skills */
.skills-columns {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1rem;
}

/* 🌙 Dark mode */
.dark .tab-label {
  background: #333;
  color: #fff;
}

.dark .tab-label:hover {
  background: #444;
}

.dark .tab-content {
  background: #1e1e1e;
  color: #eee;
  border: 1px solid #444;
}

.dark .tab-label::after {
  background: #fff;
}

.date {
  color: #888;
  font-size: 0.9rem;
}

.dark .date {
  color: #aaa;
}


</style>

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


<section id="about" style="margin-top: 4rem;">
  <h2 style="text-align:left;">About Me</h2>

  <style>

</style>
  <div class="tabs">
    <input type="radio" name="tabs" id="tab1" checked>
    <input type="radio" name="tabs" id="tab2">
    <input type="radio" name="tabs" id="tab3">
    <input type="radio" name="tabs" id="tab4">

  <div class="tabs-nav">
      <div class="tabs-nav">
        <label for="tab1" class="tab-label">💻 Skills</label>
        <label for="tab2" class="tab-label">💼 Experiences</label>
        <label for="tab3" class="tab-label">🎓 Education</label>
        <label for="tab4" class="tab-label">📜 Certifications</label>
</div>
    </div>

  <div class="content">
      <div id="content1" class="tab-content">
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
      <div id="content2" class="tab-content">
        <ul>
            <li><span class="date">2024 – Present</span><span> Digital Transformation Engineer - Alstom - Denmark</span></li>
            <li><span class="date">2022 – 2024</span><span> Test and Commissioning Engineer - Alstom - Denmark</span></li>
        </ul>
      </div>
      <div id="content3" class="tab-content">
        <ul style="padding: 0;">
          <li><span class="date">2021 – 2022</span><span> M. Sc - Linköping Institute of Technology – Sweden</span></li>
          <li><span class="date">2019 – 2022</span><span> M.Sc - Arts et Métiers ParisTech – France</span></li>
        </ul>
      </div>
      <div id="content4" class="tab-content">
        <ul>
          <li><span class="date">2024</span><span> Alstom - Six Sigma Yellow Belt Certification</span></li>
        </ul>
      </div>
    </div>
  </div>
</section>

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