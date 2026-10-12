---
layout: default
title: "Antoine Bourgois"
---

<style>
  :root {
    --ab-bg: #ffffff;
    --ab-card: #f6f8fb;
    --ab-border: #e1e6ee;
    --ab-text: #1c2430;
    --ab-muted: #5b6676;
    --ab-accent: #1f4e8c;
    --ab-accent-soft: #e6eef9;
  }
  @media (prefers-color-scheme: dark) {
    :root {
      --ab-bg: #12161c;
      --ab-card: #1a2029;
      --ab-border: #2a3340;
      --ab-text: #e6eaf0;
      --ab-muted: #9aa5b5;
      --ab-accent: #7fb0f0;
      --ab-accent-soft: #1f2e45;
    }
  }

  .ab { color: var(--ab-text); line-height: 1.6; max-width: 860px; margin: 0 auto; }
  .ab a { color: var(--ab-accent); text-decoration: none; }
  .ab a:hover { text-decoration: underline; }

  .ab-hero { display: flex; gap: 28px; align-items: center; padding: 8px 0 28px; border-bottom: 1px solid var(--ab-border); flex-wrap: wrap; }
  .ab-hero img { width: 160px; height: 160px; object-fit: cover; border-radius: 50%; border: 3px solid var(--ab-accent-soft); box-shadow: 0 4px 14px rgba(0,0,0,.12); }
  .ab-hero h1 { margin: 0 0 4px; font-size: 2rem; letter-spacing: -0.01em; }
  .ab-role { margin: 0 0 12px; color: var(--ab-muted); font-size: 1.02rem; }
  .ab-links { display: flex; flex-wrap: wrap; gap: 8px; margin-top: 12px; }

  .ab-btn { display: inline-block; padding: 5px 12px; font-size: .85rem; border: 1px solid var(--ab-border); border-radius: 999px; background: var(--ab-card); color: var(--ab-accent) !important; transition: all .15s; }
  .ab-btn:hover { background: var(--ab-accent-soft); border-color: var(--ab-accent); text-decoration: none !important; }

  .ab h2 { margin: 36px 0 14px; font-size: 1.25rem; padding-bottom: 6px; border-bottom: 2px solid var(--ab-accent); display: inline-block; }

  .ab-tags { display: flex; flex-wrap: wrap; gap: 8px; margin-top: 12px; }
  .ab-tag { padding: 3px 11px; font-size: .82rem; border-radius: 6px; background: var(--ab-accent-soft); color: var(--ab-accent); }

  .ab-card { background: var(--ab-card); border: 1px solid var(--ab-border); border-left: 4px solid var(--ab-accent); border-radius: 8px; padding: 16px 20px; margin-bottom: 16px; }
  .ab-card h3 { margin: 0 0 4px; font-size: 1.05rem; line-height: 1.35; }
  .ab-card .ab-authors { margin: 0 0 4px; font-size: .95rem; }
  .ab-card .ab-venue { margin: 0 0 10px; font-size: .9rem; color: var(--ab-muted); }
  .ab-year { float: right; margin-left: 12px; font-size: .8rem; font-weight: 600; color: var(--ab-muted); }

  .ab-footer { margin-top: 44px; padding-top: 16px; border-top: 1px solid var(--ab-border); font-size: .85rem; color: var(--ab-muted); }

  @media (max-width: 560px) {
    .ab-hero { justify-content: center; text-align: center; }
    .ab-links { justify-content: center; }
  }
</style>

<div class="ab">

  <header class="ab-hero">
    <img src="assets/img/profile.jpg" alt="Antoine Bourgois">
    <div>
      <h1>Antoine Bourgois</h1>
      <p class="ab-role">PhD student in Natural Language Processing<br>Lattice (CNRS, ENS-PSL, Université Sorbonne Nouvelle)</p>
      <p style="margin:0;">I work on coreference resolution and the computational analysis of French literature.</p>
      <div class="ab-links">
        <a class="ab-btn" href="https://scholar.google.com/citations?user=y13Qx44AAAAJ&hl=en">Google Scholar</a>
        <a class="ab-btn" href="https://github.com/lattice-8094/propp">GitHub</a>
        <a class="ab-btn" href="https://hal.science/hal-05319970">HAL</a>
        <a class="ab-btn" href="https://arxiv.org/abs/2510.15594">arXiv</a>
      </div>
    </div>
  </header>

  <h2>About</h2>
  <p>
    My research looks at how to track characters across entire novels. Most coreference systems are built for short documents, so I build models and annotated corpora for book-length French fiction, then use the output for literary questions such as character gender and narrative structure.
  </p>
  <div class="ab-tags">
    <span class="ab-tag">Coreference resolution</span>
    <span class="ab-tag">Computational literary studies</span>
    <span class="ab-tag">French fiction</span>
    <span class="ab-tag">Long-document NLP</span>
    <span class="ab-tag">Narrative analysis</span>
  </div>

  <h2>Software</h2>
  <div class="ab-card">
    <h3>Propp: Pattern Recognition and Ontologies for Prose Processing</h3>
    <p class="ab-venue">A Natural Language Processing framework for narrative analysis. Includes the trained French coreference pipeline, available as the open-source <code>propp_fr</code> Python library.</p>
    <a class="ab-btn" href="https://github.com/lattice-8094/propp">GitHub repository</a>
    <a class="ab-btn" href="https://lattice-8094.github.io/propp/">Documentation</a>
  </div>

  <h2>Publications</h2>

  <div class="ab-card">
    <span class="ab-year">2025</span>
    <h3>The Elephant in the Coreference Room: Resolving Coreference in Full-Length French Fiction Works</h3>
    <p class="ab-authors"><strong>Antoine Bourgois</strong> and Thierry Poibeau</p>
    <p class="ab-venue">Proceedings of the Eighth Workshop on Computational Models of Reference, Anaphora and Coreference (CRAC 2025), EMNLP 2025, Suzhou, China.</p>
    <a class="ab-btn" href="articles/2025_CRAC_CoreferenceInFrenchNovels.pdf">PDF</a>
    <a class="ab-btn" href="https://arxiv.org/abs/2510.15594">arXiv</a>
    <a class="ab-btn" href="https://hal.science/hal-05319970">HAL</a>
    <a class="ab-btn" href="articles/2025_CRAC_CoreferenceInFrenchNovels_poster.pdf">Poster</a>
  </div>

  <div class="ab-card">
    <span class="ab-year">2025</span>
    <h3>GLaRef@CRAC2025: Should We Transform Coreference Resolution into a Text Generation Task?</h3>
    <p class="ab-authors">Olga Seminck, <strong>Antoine Bourgois</strong>, Yoann Dupont, Mathieu Dehouck, Marine Delaborde</p>
    <p class="ab-venue">Proceedings of the Eighth Workshop on Computational Models of Reference, Anaphora and Coreference (CRAC 2025), EMNLP 2025, Suzhou, China.</p>
    <a class="ab-btn" href="articles/2025_CRAC_SharedTask.pdf">PDF</a>
    <a class="ab-btn" href="articles/EMNLP_CRAC_2025_with-UWB.pdf">Presentation</a>
    <a class="ab-btn" href="articles/2025_CRAC_SharedTask_Slides.pdf">Slides</a>
  </div>

  <h2>Talks</h2>
  <div class="ab-card">
    <span class="ab-year">2025</span>
    <h3>BookNLP-fr : Chaîne d'analyse computationnelle des œuvres de fiction française</h3>
    <p class="ab-venue">Séminaire « Interprétations artificielles », CSLF et MSH Mondes, 20 mars 2025.</p>
  </div>

  <h2>Contact</h2>
  <p>antoine [dot] bourgois [at] protonmail [dot] com</p>

  <div class="ab-footer">Lattice, Montrouge, France</div>

</div>
