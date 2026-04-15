---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<!-- CV ACTIONS -->
<div class="cv-actions">

  <span class="cv-action-group">
    <button onclick="window.print()" class="cv-btn">Print CV</button>
    <a href="/files/cv_en.pdf" target="_blank" class="cv-btn">PDF</a>
  </span>

  <span class="cv-divider">|</span>

  <span class="cv-action-group">
    <a href="/files/cv_en.pdf" target="_blank" class="cv-lang">EN</a>
    <a href="/files/cv_pt.pdf" target="_blank" class="cv-lang">PT</a>
    <a href="/files/cv_fr.pdf" target="_blank" class="cv-lang">FR</a>
  </span>

</div>

<hr>

Education
======
* M.Sc. in Computer Science (in progress), PUC-Rio, 2025–
* B.Sc. in Biomedical Engineering, UFPE, 2019–2025  
  * Exchange program in Biomedical Engineering, Aix-Marseille Université, France (2023–2024)
  * Undergraduate Research Fellow (CNPq, 2022–2023)

Work experience
======

<div class="cv-section">

  <details>
    <summary>
      <span class="cv-title">AI Researcher</span> — TecGraf, PUC-Rio (Dec 2025 – Present)
    </summary>
    <div class="cv-content">
      <ul>
        <li>Developed neural decoding pipelines using EEG data in Python (MNE, SciPy), including preprocessing, feature engineering, and multichannel time-series analysis.</li>
        <li>Implemented machine learning and deep learning models.</li>
        <li>Applied explainable AI techniques for model interpretation and spatiotemporal relevance mapping.</li>
      </ul>
    </div>
  </details>

  <details>
    <summary>
      <span class="cv-title">AI Research Intern</span> — iCEIS, Recife (Sep 2024 – Aug 2025)
    </summary>
    <div class="cv-content">
      <ul>
        <li>Worked on AI models applied to EEG data for autism diagnosis support.</li>
        <li>Built data pipelines including preprocessing, dimensionality reduction, and feature engineering.</li>
        <li>Implemented and optimized ML/DL models for classification of neural patterns.</li>
        <li>Co-authored publications in CBIC 2025 and IEEE LA-CCI 2025.</li>
      </ul>
    </div>
  </details>

  <details>
    <summary>
      <span class="cv-title">Research Intern in Neuroengineering</span> — Institut de Neurosciences de la Timone, Marseille (Feb 2024 – May 2024)
    </summary>
    <div class="cv-content">
      <ul>
        <li>Applied machine learning models to predict motor parameters from neural signals.</li>
        <li>Worked with high-dimensional time-series data and feature selection.</li>
      </ul>
    </div>
  </details>

  <details>
    <summary>
      <span class="cv-title">Product Owner & Co-founder</span> — Habitus Tech, Recife (Jul 2022 – Jul 2024)
    </summary>
    <div class="cv-content">
      <ul>
        <li>Led product strategy and development of tech solutions.</li>
        <li>Designed interfaces and conducted usability testing.</li>
        <li>Worked on documentation and user experience optimization.</li>
      </ul>
    </div>
  </details>

</div>

Skills
======
* Computational Neuroscience  
* Python (NumPy, Pandas, Scikit-learn, PyTorch)  
* Signal Processing (EEG, EMG)  
* Machine Learning & Deep Learning  
* Data Analysis  
* SQL, Git, Jupyter  

Languages
======
* English (C2)  
* French (B2 – DELF)  
* Spanish (B2 – SIELE)  

<style>
.cv-section details {
  margin-bottom: 12px;
}

.cv-section summary {
  cursor: pointer;
}

.cv-title {
  color: #2e7d32;
  font-weight: bold;
}

.cv-content {
  margin-left: 15px;
  margin-top: 8px;
}

.cv-content ul {
  margin: 0;
  padding-left: 18px;
}

/* KEYWORD HIGHLIGHT */
.highlight {
  color: #2e7d32;
  font-weight: 600;
}

/* CV ACTIONS */
.cv-actions {
  display: flex;
  align-items: center;
  gap: 10px;
  margin-bottom: 10px;
  font-size: 0.9em;
}

.cv-btn {
  background: none;
  border: 1px solid #2e7d32;
  color: #2e7d32;
  padding: 4px 10px;
  border-radius: 6px;
  cursor: pointer;
  text-decoration: none;
  font-weight: 500;
}

.cv-btn:hover {
  background: #2e7d32;
  color: white;
}

.cv-lang {
  margin: 0 4px;
  color: #2e7d32;
  text-decoration: none;
  font-weight: bold;
}

.cv-lang:hover {
  text-decoration: underline;
}

.cv-divider {
  color: #aaa;
}
</style>

<script>
document.addEventListener("DOMContentLoaded", function() {

  const keywords = [
    "EEG",
    "machine learning",
    "deep learning",
    "Python",
    "XAI",
    "MNE",
    "SciPy",
    "PyTorch",
    "scikit-learn",
    "time-series",
    "signal processing"
  ];

  const content = document.querySelectorAll(".cv-content li");

  content.forEach(item => {
    let text = item.innerHTML;

    keywords.forEach(keyword => {
      const regex = new RegExp(`(${keyword})`, "gi");
      text = text.replace(regex, '<span class="highlight">$1</span>');
    });

    item.innerHTML = text;
  });

});
</script>
