---
layout: page
title: Paper editor
permalink: /math-paper-editor/
description: Scoped review and traceable revision for mathematical manuscripts in LaTeX.
nav: true
nav_order: 6
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
  .workflow-showcase .wf-table { width: 100%; border-collapse: collapse; font-size: .87rem; margin: 1.2rem 0; }
  .workflow-showcase .wf-table th, .workflow-showcase .wf-table td { padding: .8rem .6rem; border-bottom: 1px solid var(--global-divider-color); text-align: left; vertical-align: top; }
  .workflow-showcase .wf-table th { font-weight: 600; }
---

<div class="workflow-showcase">
  <section class="wf-hero" aria-labelledby="editor-heading">
    <p class="wf-eyebrow">Open research tool · Mathematical manuscripts</p>
    <h2 id="editor-heading">Refine the writing.<br>Keep the mathematics.</h2>
    <p class="wf-lead">Math Paper Editor is a Codex skill for reviewing and revising LaTeX mathematical manuscripts. It keeps the requested scope, mathematical concerns, and actual source changes explicit.</p>
    <div class="wf-links">
      <a class="wf-primary" href="#editor-demo">Try the usage demo ↓</a>
      <a href="https://github.com/jieliu-maths/math-paper-editor">Source &amp; installation ↗</a>
      <a href="https://github.com/jieliu-maths/math-paper-editor/blob/main/README.zh-CN.md" lang="zh-CN">中文说明 ↗</a>
    </div>
    <p class="wf-meta">Version 0.1.0 · MIT licensed · Analysis and PDE first</p>
  </section>

  <section class="wf-section" aria-label="What the editor preserves">
    <div class="wf-principles">
      <div><h3><span class="wf-number">01</span>Choose the scope.</h3><p>Review without writing, edit a selected section, inspect a proof more deeply, or authorize restructuring of an existing argument.</p></div>
      <div><h3><span class="wf-number">02</span>Keep concerns explicit.</h3><p>A grammar correction cannot silently repair a theorem. Missing assumptions, proof gaps, and unverified references are reported separately.</p></div>
      <div><h3><span class="wf-number">03</span>Inspect the revision.</h3><p>Local snapshots and guarded replacements record the edit. Differences outside recorded operations remain visibly unattributed.</p></div>
    </div>
  </section>

  <section class="wf-section" id="editor-demo" aria-labelledby="editor-demo-heading">
    <p class="wf-eyebrow">An interactive usage example</p>
    <h2 id="editor-demo-heading">What does “edit the Introduction” allow?</h2>
    <p class="wf-intro">Explore four modes, inspect the original and current source, and view the exact difference. The rewrite tab uses a separate correct example. Switch to 中文 or copy an actual invocation inside the demonstration.</p>
    <iframe class="wf-demo" id="paper-editor-demo" src="{{ '/assets/demos/math-paper-editor.html' | relative_url }}" title="Interactive Math Paper Editor usage example with source comparison, diff, and English/Chinese controls" width="930" height="850" loading="lazy"></iframe>
    <p class="wf-caption">Preset teaching examples, including a deliberately false claim. This browser demonstration makes no model calls or uploads and changes no real manuscript. <a href="{{ '/assets/demos/math-paper-editor.html' | relative_url }}">Open the demo on its own ↗</a></p>
  </section>

  <section class="wf-section" aria-labelledby="python-heading">
    <p class="wf-eyebrow">Instructions and local tools</p>
    <h2 id="python-heading">Where does Python fit?</h2>
    <p class="wf-intro">The skill's core is a set of editing instructions. Python runs the bundled local tools for reliable records and upgrades; it is not the language in which an AI must think about mathematics.</p>
    <table class="wf-table">
      <thead><tr><th scope="col">Task</th><th scope="col">Local requirement</th></tr></thead>
      <tbody>
        <tr><td>Read the instructions or perform a read-only review</td><td>An AI host able to load the skill; local Python is not needed for the instructions themselves.</td></tr>
        <tr><td>Use the default tracked editing, installation, upgrade, or test tools</td><td>Python 3.10+, using the standard library. Snapshots, hashes, guarded edits, and diffs run locally.</td></tr>
        <tr><td>Use this web demonstration</td><td>A browser with JavaScript; no Python installation.</td></tr>
        <tr><td>Compile a LaTeX manuscript into a PDF</td><td>An available TeX compiler or host compilation service. Python alone does not compile LaTeX.</td></tr>
      </tbody>
    </table>
    <p class="wf-scope">The supplied v0.1.0 editing procedure uses the Python helper. If the required records cannot be created, the skill continues with read-only work and reports the limitation. Host/model data handling still follows the selected service's policies.</p>
  </section>

  <section class="wf-section wf-last" aria-labelledby="editor-evidence-heading">
    <h2 id="editor-evidence-heading">What has been checked?</h2>
    <p class="wf-scope">The first release passed 38 deterministic tool tests and four macOS/Linux CI combinations. An initial assistant-assessed evaluation ran 10 synthetic cases with the skill and 10 with an unaided baseline. Both met the case criteria; no mathematical accuracy improvement was demonstrated. The reports, observed sources, and limits are public.</p>
    <p class="wf-scope"><a href="https://github.com/jieliu-maths/math-paper-editor/blob/v0.1.0/evals/results/v0.1.0.md">Read the evaluation ↗</a> · <a href="https://github.com/jieliu-maths/math-paper-editor/releases/tag/v0.1.0">v0.1.0 release ↗</a></p>
    <p class="wf-scope">Use it independently or alongside <a href="{{ '/ai-research-workflow/' | relative_url }}">AI Research Workflow</a>. The workflow manages research evidence and approved state; the editor works on a selected manuscript. A fluent revision, a clean diff, or a successful build does not certify a proof.</p>
  </section>
</div>

<script>
  (() => {
    const frame = document.getElementById("paper-editor-demo");
    window.addEventListener("message", (event) => {
      if (event.origin !== window.location.origin || event.source !== frame.contentWindow || event.data?.type !== "math-paper-editor-demo-height") return;
      const height = Number(event.data.height);
      if (Number.isFinite(height) && height >= 200 && height <= 4000) frame.style.height = (height + 2) + "px";
    });
  })();
</script>
