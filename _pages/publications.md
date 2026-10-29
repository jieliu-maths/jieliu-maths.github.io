---
layout: page
title: Publications
permalink: /publications/
description: Published articles and public preprints.
nav: true
nav_order: 2
_styles: |
  .publication-records .publication-section + .publication-section { margin-top: 2.5rem; }
  .publication-records .publication-section > h2 { margin: 0; font-size: 1.25rem; font-weight: 600; line-height: 1.4; }
  .publication-records .publications {
    display: grid;
    grid-template-columns: 4.5rem minmax(0, 1fr);
    column-gap: 1.75rem;
    row-gap: 1.75rem;
    margin-top: 1.25rem;
  }
  .publication-records .publications h2.bibliography {
    grid-column: 1;
    margin: 0;
    padding: 1.1rem 0 0;
    border-top: 1px solid var(--global-divider-color);
    color: var(--global-text-color);
    font-size: 1.05rem;
    font-weight: 600;
    line-height: 1.5;
    text-align: left;
  }
  .publication-records .publications ol.bibliography {
    grid-column: 2;
    min-width: 0;
    margin: 0;
    padding: 1.1rem 0 0;
    border-top: 1px solid var(--global-divider-color);
  }
  .publication-records .publications ol.bibliography > li { margin: 0; padding: 0; }
  .publication-records .publications ol.bibliography > li + li { margin-top: 1.4rem; padding-top: 1.4rem; border-top: 1px solid var(--global-divider-color); }
  .publication-records .publications .row { margin-left: 0; margin-right: 0; }
  .publication-records .publications .row > [id] { flex: 0 0 100%; max-width: 100%; min-width: 0; padding: 0; scroll-margin-top: 5rem; }
  .publication-records .publications ol.bibliography .title { font-size: 1.025rem; font-weight: 500; line-height: 1.55; }
  .publication-records .publications ol.bibliography .author { margin-top: 0.25rem; font-size: 0.94rem; line-height: 1.6; }
  .publication-records .publications ol.bibliography .periodical { font-size: 0.92rem; line-height: 1.65; }
  .publication-records .publications ol.bibliography .links { display: flex; flex-wrap: wrap; gap: 0.4rem; margin-top: 0.65rem; }
  .publication-records .publications ol.bibliography .links a.btn { margin: 0; padding: 0.2rem 0.65rem; border: 1px solid var(--global-divider-color); border-radius: 4px; font-size: 0.75rem; line-height: 1.5; }
  .publication-records .publications ol.bibliography .links a.btn:hover { border-color: var(--global-theme-color); }
  @media (max-width: 700px) {
    .publication-records .publications { grid-template-columns: minmax(0, 1fr); row-gap: 0.75rem; }
    .publication-records .publications ol.bibliography { grid-column: 1; padding-top: 0; border-top: 0; }
    .publication-records .publications h2.bibliography { margin-top: 0.5rem; }
  }
---

<div class="publication-records">
  <section class="publication-section" aria-labelledby="published-articles">
    <h2 id="published-articles">Published articles</h2>
    <div class="publications">
      {% bibliography --query @article %}
    </div>
  </section>
  <section class="publication-section" aria-labelledby="preprints">
    <h2 id="preprints">Preprints</h2>
    <div class="publications">
      {% bibliography --query @unpublished %}
    </div>
  </section>
</div>
