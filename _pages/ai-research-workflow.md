---
layout: page
title: AI4Math
permalink: /ai-research-workflow/
description: An open workflow for AI-assisted mathematics, with explicit evidence, independent review, and human decisions.
nav: true
nav_order: 5
_styles: |
  .workflow-showcase { --wf-accent: #79518c; }
  .workflow-showcase .wf-eyebrow { font-size: .69rem; font-weight: 600; letter-spacing: .17em; color: var(--wf-accent); text-transform: uppercase; margin: 0 0 .9rem; }
  .workflow-showcase .wf-hero { padding: .6rem 0 2.7rem; border-bottom: 1px solid var(--global-divider-color); }
  .workflow-showcase .wf-hero h2 { font-family: "Roboto Slab", Georgia, serif; font-size: clamp(2rem, 4.7vw, 3.15rem); font-weight: 400; letter-spacing: -.045em; line-height: 1.2; max-width: 20ch; margin: 0 0 1.35rem; }
  .workflow-showcase .wf-lead { max-width: 68ch; font-size: 1.07rem; line-height: 1.8; color: var(--global-text-color-light); margin-bottom: 1.35rem; }
  .workflow-showcase .wf-links { display: flex; flex-wrap: wrap; align-items: center; gap: 1rem 1.5rem; font-size: .9rem; }
  .workflow-showcase .wf-links .wf-primary { display: inline-block; background: var(--wf-accent); color: #fff; padding: .65rem 1rem; border-radius: 4px; text-decoration: none; }
  .workflow-showcase .wf-links a:focus-visible { outline: 3px solid #b598c6; outline-offset: 4px; }
  .workflow-showcase .wf-meta { font-size: .76rem; color: var(--global-text-color-light); margin: 1.3rem 0 0; }
  .workflow-showcase .wf-section { padding: 2.5rem 0; border-bottom: 1px solid var(--global-divider-color); }
  .workflow-showcase .wf-section h2 { font-size: 1.5rem; font-weight: 500; margin: 0 0 .9rem; }
  .workflow-showcase .wf-intro { max-width: 75ch; margin: 0 0 1.5rem; color: var(--global-text-color-light); }
  .workflow-showcase .wf-principles { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 2rem; }
  .workflow-showcase .wf-principles h3 { font-size: .98rem; font-weight: 600; margin: 0 0 .6rem; }
  .workflow-showcase .wf-principles p { font-size: .9rem; line-height: 1.8; margin: 0; }
  .workflow-showcase .wf-number { display: block; font-family: Georgia, serif; font-size: 1.5rem; margin-bottom: .9rem; color: var(--wf-accent); }
  .workflow-showcase .wf-demo { display: block; width: 100%; border: 1px solid var(--global-divider-color); border-radius: 8px; background: #fff; }
  .workflow-showcase .wf-caption { font-size: .78rem; color: var(--global-text-color-light); margin: .9rem 0 0; }
  .workflow-showcase .wf-start { display: grid; grid-template-columns: minmax(0, .9fr) minmax(0, 1.4fr); gap: 2rem; align-items: start; }
  .workflow-showcase .wf-start > * { min-width: 0; }
  .workflow-showcase pre { padding: 1.2rem; font-size: .77rem; line-height: 1.9; overflow-x: auto; margin: 0; background: color-mix(in srgb, var(--wf-accent) 5%, var(--global-bg-color)); border: 1px solid var(--global-divider-color); border-radius: 5px; }
  .workflow-showcase .wf-last { border-bottom: 0; padding-bottom: .5rem; }
  .workflow-showcase .wf-scope { font-size: .85rem; max-width: 78ch; color: var(--global-text-color-light); line-height: 1.8; }
  @media (max-width: 700px) {
    .workflow-showcase .wf-principles, .workflow-showcase .wf-start { grid-template-columns: minmax(0, 1fr); gap: 1.5rem; }
    .workflow-showcase .wf-hero { padding-top: 0; }
    .workflow-showcase .wf-section { padding: 2rem 0; }
    .workflow-showcase .wf-principles h3 { margin-bottom: .35rem; }
    .workflow-showcase .wf-number { display: inline-block; font-size: 1rem; margin: 0 .6rem 0 0; }
  }
---

<div class="workflow-showcase">
  <section class="wf-hero" aria-labelledby="workflow-heading">
    <p class="wf-eyebrow">Open research tool · AI4Math first</p>
    <h2 id="workflow-heading">Research with AI.<br>Keep the proof in view.</h2>
    <p class="wf-lead">AI Research Workflow keeps theorem targets, evidence, independent review, and unresolved gaps visible across research sessions. The researcher retains the decision to accept a result.</p>
    <div class="wf-links">
      <a class="wf-primary" href="#workflow-demo">Explore the workflow ↓</a>
      <a href="https://github.com/jieliu-maths/AI-Research-Workflow">Source &amp; documentation ↗</a>
      <a href="https://github.com/jieliu-maths/AI-Research-Workflow/blob/main/README.zh-CN.md" lang="zh-CN">中文说明 ↗</a>
    </div>
    <p class="wf-meta">Version 2.7.0 · MIT licensed · Local, inspectable research records</p>
  </section>

  <section class="wf-section" aria-label="Why keep a research workflow?">
    <div class="wf-principles">
      <div>
        <h3><span class="wf-number">01</span>Keep the question precise.</h3>
        <p>Separate the theorem target, its necessary lemmas, and the route being tested. Make assumptions and the stopping condition explicit.</p>
      </div>
      <div>
        <h3><span class="wf-number">02</span>Let evidence keep its scope.</h3>
        <p>Distinguish a proof, a finite check, a numerical observation, and an external result. Retain failed candidates and exactly what they exclude.</p>
      </div>
      <div>
        <h3><span class="wf-number">03</span>Review before accepting.</h3>
        <p>Use separate Director, Researcher, and Critic tasks. Independent review informs the decision; explicit owner approval changes the accepted record.</p>
      </div>
    </div>
  </section>

  <section class="wf-section" id="workflow-demo" aria-labelledby="demo-heading">
    <p class="wf-eyebrow">An interactive teaching example</p>
    <h2 id="demo-heading">What changes when a gap is found?</h2>
    <p class="wf-intro">Follow a familiar identity through construction, critique, repair, and an owner decision. The example shows why checking many cases does not by itself prove a theorem. Switch to 中文 inside the demonstration.</p>
    <iframe class="wf-demo" id="ai4math-demo" src="{{ '/assets/demos/ai4math-workflow.html' | relative_url }}" title="Interactive AI4Math workflow teaching example, with English and Chinese controls" width="930" height="720" loading="lazy"></iframe>
    <p class="wf-caption">Scripted illustration with a local exact computation. No model calls, uploads, or real project-state changes. <a href="{{ '/assets/demos/ai4math-workflow.html' | relative_url }}">Open the demonstration on its own ↗</a></p>
  </section>

  <section class="wf-section" aria-labelledby="start-heading">
    <div class="wf-start">
      <div>
        <p class="wf-eyebrow">Try it locally</p>
        <h2 id="start-heading">A small first step.</h2>
        <p>Start with an offline example. Python 3.10 or later is enough; the demo needs no API key or model download.</p>
        <p><a href="https://github.com/jieliu-maths/AI-Research-Workflow#quickstart">Installation &amp; project setup ↗</a></p>
      </div>
      <pre><code>git clone https://github.com/jieliu-maths/AI-Research-Workflow.git
cd AI-Research-Workflow
./workflow self-check
python3 examples/ai4math/verify.py \
  --output-dir /tmp/ai4math-demo</code></pre>
    </div>
  </section>

  <section class="wf-section wf-last" aria-labelledby="scope-heading">
    <h2 id="scope-heading">Scope and current limits</h2>
    <p class="wf-scope">The supported core is mathematical research. An <a href="https://github.com/jieliu-maths/AI-Research-Workflow/tree/main/profiles/ai4s">experimental AI4S profile</a> adds data provenance, controls, frozen evaluation, and reproducibility. The project does not include a foundation model, an automatic theorem prover, or a complete autonomous scientist. Workflow consistency checks do not certify mathematical truth, and comparative productivity gains have not yet been established.</p>
    <p class="wf-scope">For a selected manuscript, <a href="{{ '/math-paper-editor/' | relative_url }}">Math Paper Editor</a> adds scoped review and traceable revision. Its usage demonstration shows what a language edit may change.</p>
    <p class="wf-scope"><a href="https://github.com/jieliu-maths/AI-Research-Workflow/blob/main/docs/landscape-review.en.md">Related systems &amp; design comparison ↗</a> · <a href="https://github.com/jieliu-maths/AI-Research-Workflow/blob/main/ROADMAP.md">Development roadmap ↗</a></p>
  </section>
</div>

<script>
  (() => {
    const frame = document.getElementById("ai4math-demo");
    window.addEventListener("message", (event) => {
      if (event.origin !== window.location.origin || event.source !== frame.contentWindow || event.data?.type !== "ai4math-demo-height") return;
      const height = Number(event.data.height);
      if (Number.isFinite(height) && height >= 200 && height <= 4000) frame.style.height = `${height + 2}px`;
    });
  })();
</script>
