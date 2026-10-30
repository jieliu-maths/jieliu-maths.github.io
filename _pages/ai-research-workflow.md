---
layout: page
title: AI4Math
permalink: /ai-research-workflow/
description: My explorations in AI-assisted mathematical research, from inspectable workflows to faithful manuscript revision.
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
  .workflow-showcase .wf-experiment { margin: 1.3rem 0 0; padding: 1rem 1.1rem; border: 1px solid var(--global-divider-color); border-radius: 6px; }
  .workflow-showcase .wf-experiment > summary { cursor: pointer; color: var(--wf-accent); font-size: .9rem; font-weight: 600; }
  .workflow-showcase .wf-experiment[open] > summary { margin-bottom: 1.2rem; }
---

<div class="workflow-showcase">
  <section class="wf-hero" aria-labelledby="workflow-heading">
    <p class="wf-eyebrow">Research direction · Work in progress</p>
    <h2 id="workflow-heading">Exploring AI-assisted<br>mathematical research.</h2>
    <p class="wf-lead">I am exploring how AI can support mathematical research while keeping assumptions, evidence, proof obligations, and author decisions explicit. The research-workflow and manuscript-editing tools below are early components of this developing direction.</p>
    <div class="wf-links">
      <a class="wf-primary" href="#workflow-demo">Research workflows ↓</a>
      <a href="#manuscript-editor">Manuscript review &amp; revision ↓</a>
    </div>
    <p class="wf-meta">Ongoing exploration · Analysis and PDE as initial settings</p>
  </section>

  <section class="wf-section" aria-label="Questions guiding this exploration">
    <div class="wf-principles">
      <div>
        <h3><span class="wf-number">01</span>Keep the question precise.</h3>
        <p>How can AI-assisted work retain the exact theorem target, assumptions, proof dependencies, and unresolved gaps across research sessions?</p>
      </div>
      <div>
        <h3><span class="wf-number">02</span>Keep evidence in scope.</h3>
        <p>How can a proof, a finite check, a numerical observation, and an external input remain clearly distinguished as an argument develops?</p>
      </div>
      <div>
        <h3><span class="wf-number">03</span>Keep the author in control.</h3>
        <p>How can review and revision improve an argument's clarity while preserving its mathematical meaning and explicit human decisions?</p>
      </div>
    </div>
  </section>

  <section class="wf-section" id="workflow-demo" aria-labelledby="demo-heading">
    <p class="wf-eyebrow">Exploration 01 · Research process</p>
    <h2 id="demo-heading">Inspectable research workflows</h2>
    <p class="wf-intro">AI Research Workflow is an early prototype for this direction. It records theorem targets, dependencies, evidence, independent review, and author-approved decisions. The teaching example follows a familiar identity through construction, critique, repair, and a decision.</p>
    <p class="wf-scope"><a href="https://github.com/jieliu-maths/AI-Research-Workflow">Workflow source &amp; notes ↗</a> · <a href="https://github.com/jieliu-maths/AI-Research-Workflow/blob/main/README.zh-CN.md" lang="zh-CN">中文说明 ↗</a></p>
    <details class="wf-experiment" id="workflow-example">
      <summary>Explore the research-workflow demonstration</summary>
      <iframe class="wf-demo" id="ai4math-demo" src="{{ '/assets/demos/ai4math-workflow.html' | relative_url }}" title="Interactive AI4Math workflow teaching example, with English and Chinese controls" width="930" height="720" loading="lazy"></iframe>
      <p class="wf-caption">A scripted illustration with local exact computation. It makes no model calls or uploads and changes no research record. <a href="{{ '/assets/demos/ai4math-workflow.html' | relative_url }}">Open the demonstration ↗</a></p>
    </details>
    <details class="wf-experiment">
      <summary>Try the offline workflow example</summary>
      <p class="wf-scope">Python 3.10 or later is enough for the bundled local example; no API key or model download is needed.</p>
      <pre><code>git clone https://github.com/jieliu-maths/AI-Research-Workflow.git
cd AI-Research-Workflow
./workflow self-check
python3 examples/ai4math/verify.py \
  --output-dir /tmp/ai4math-demo</code></pre>
    </details>
  </section>

  <section class="wf-section" id="manuscript-editor" aria-labelledby="manuscript-heading">
    <p class="wf-eyebrow">Exploration 02 · Mathematical writing</p>
    <h2 id="manuscript-heading">Reviewing and revising mathematical manuscripts</h2>
    <p class="wf-intro">Within the same AI4Math exploration, Math Paper Editor examines how AI can assist with scoped mathematical review and faithful LaTeX revision. It separates mathematical concerns from language edits and makes the actual source changes inspectable.</p>
    <p class="wf-scope">The current prototype supports read-only review, conservative editing, deeper proof inspection, and authorized restructuring of existing arguments. Its demonstration shows what “edit only the Introduction” allows, including a valid zero-change outcome.</p>
    <p class="wf-scope"><a href="https://github.com/jieliu-maths/math-paper-editor">Editor source &amp; notes ↗</a> · <a href="https://github.com/jieliu-maths/math-paper-editor/blob/main/README.zh-CN.md" lang="zh-CN">中文说明 ↗</a></p>
    <details class="wf-experiment" id="editor-demo">
      <summary>Explore manuscript review and revision</summary>
      <iframe class="wf-demo" id="paper-editor-demo" src="{{ '/assets/demos/math-paper-editor.html' | relative_url }}" title="Interactive Math Paper Editor usage example with source comparison, diff, and English/Chinese controls" width="930" height="850" loading="lazy"></iframe>
      <p class="wf-caption">Preset examples using synthetic manuscripts, including a deliberately false claim. No model calls, uploads, or changes to a real paper. <a href="{{ '/assets/demos/math-paper-editor.html' | relative_url }}">Open the demonstration ↗</a></p>
    </details>
  </section>

  <section class="wf-section wf-last" aria-labelledby="scope-heading">
    <h2 id="scope-heading">Current scope and open questions</h2>
    <p class="wf-scope">These are early tools and teaching examples within my AI4Math exploration. Their consistency checks and model-assisted reviews do not certify mathematical truth, and broader gains in research productivity or proof-review accuracy have not been established. The editor's initial 10-case comparison met the same criteria with and without the skill.</p>
    <p class="wf-scope"><a href="https://github.com/jieliu-maths/AI-Research-Workflow/blob/main/docs/landscape-review.en.md">Related systems and design questions ↗</a> · <a href="https://github.com/jieliu-maths/math-paper-editor/blob/v0.1.0/evals/results/v0.1.0.md">Initial manuscript-editor evaluation ↗</a></p>
    <details class="wf-experiment">
      <summary>Implementation notes and the broader scientific setting</summary>
      <p class="wf-scope">The instructions and read-only review do not themselves need local Python. Bundled snapshots, guarded edits, validation, installation, and upgrades use Python 3.10+. The browser demonstrations use JavaScript; compiling a manuscript requires an available TeX compiler or host service.</p>
      <p class="wf-scope">An <a href="https://github.com/jieliu-maths/AI-Research-Workflow/tree/main/profiles/ai4s">experimental AI4S profile</a> also explores data provenance, controls, frozen evaluation, and reproducibility. The main emphasis here remains mathematical research.</p>
    </details>
  </section>
</div>

<script>
  (() => {
    const anchors = new Map([
      ["#workflow-demo", "workflow-example"],
      ["#manuscript-editor", "editor-demo"],
      ["#editor-demo", "editor-demo"],
    ]);
    const expandTarget = () => {
      const id = anchors.get(window.location.hash);
      if (id) document.getElementById(id).open = true;
    };
    window.addEventListener("hashchange", expandTarget);
    expandTarget();
    const frames = new Map([
      ["ai4math-demo-height", document.getElementById("ai4math-demo")],
      ["math-paper-editor-demo-height", document.getElementById("paper-editor-demo")],
    ]);
    window.addEventListener("message", (event) => {
      const frame = frames.get(event.data?.type);
      if (!frame || event.origin !== window.location.origin || event.source !== frame.contentWindow) return;
      const height = Number(event.data.height);
      if (Number.isFinite(height) && height >= 200 && height <= 4000) frame.style.height = (height + 2) + "px";
    });
  })();
</script>
