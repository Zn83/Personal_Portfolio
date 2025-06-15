---
title: "Accueil"
---

<div style="text-align:center; margin-top:2rem;">
  <img src="/Personal_Portfolio/images/Corporate_detouree_carree.png"
       alt="Ma photo"
       style="width: 180px; height: 180px; border-radius: 50%; object-fit: cover; display: block; margin: 0 auto;">
  <h1 style="transition: transform 0.3s ease; display: inline-block;"
      onmouseover="this.style.transform='scale(1.1)'"
      onmouseout="this.style.transform='scale(1)'">
    Zian
  </h1>
  <h2>Digital Transformation Engineer<span style="color:#9013fe">.</span></h2>
</div>

<style>
  .tabs {
    max-width: 800px;
    margin: 2rem auto;
  }
  input[type="radio"] {
    display: none;
  }
  .tab-label {
    display: inline-block;
    padding: 0.5rem 1rem;
    cursor: pointer;
    background: #787878;
    margin-right: 5px;
    border-radius: 5px 5px 0 0;
  }
  .tab-content {
    border: 1px solid #eee;
    padding: 1rem;
    display: none;
    background: #f9f9f9;
    border-radius: 0 0 5px 5px;
  }
  #tab1:checked ~ .content #content1,
  #tab2:checked ~ .content #content2,
  #tab3:checked ~ .content #content3 {
    display: block;
  }
  #tab1:checked ~ .tabs-nav label[for="tab1"],
  #tab2:checked ~ .tabs-nav label[for="tab2"],
  #tab3:checked ~ .tabs-nav label[for="tab3"] {
    background: #ddd;
  }
</style>

<section id="about" style="margin-top: 4rem;">
  <h2 style="text-align:left;">À propos</h2>

  <style>
/* Container global */
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
  margin-bottom: 1rem;
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
#tab3:checked ~ .tabs-nav label[for="tab3"]::after {
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
#tab3:checked ~ .content #content3 {
  display: block;
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
</style>
  <div class="tabs">
    <input type="radio" name="tabs" id="tab1" checked>
    <input type="radio" name="tabs" id="tab2">
    <input type="radio" name="tabs" id="tab3">

  <div class="tabs-nav">
      <div class="tabs-nav">
        <label for="tab1" class="tab-label">💻 Skills</label>
        <label for="tab2" class="tab-label">🎓 Education</label>
        <label for="tab3" class="tab-label">📜 Certifications</label>
</div>
    </div>

  <div class="content">
      <div id="content1" class="tab-content">
        <ul>
          <li>Data Analysis</li>
          <li>Project Management</li>
          <li>HTML / CSS / JavaScript</li>
          <li>Python / Django</li>
        </ul>
      </div>
      <div id="content2" class="tab-content">
        <ul>
          <li>M. Sc - Linköping Institute of Technology – Sweden</li>
          <li>M.Sc - Arts et Métiers ParisTech – France</li>
        </ul>
      </div>
      <div id="content3" class="tab-content">
        <ul>
          <li>Alstom - Six Sigma Yellow Belt Certification</li>
        </ul>
      </div>
    </div>
  </div>
</section>