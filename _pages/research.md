---
layout: page
title: Research
permalink: /research/
description: Fluid mechanics, nonlinear waves, and dispersive dynamics.
nav: true
nav_order: 1
_styles: |
  .research-overview .research-lead {
    max-width: 78ch;
    margin: 0 0 1.8rem;
    font-size: 1.025rem;
    line-height: 1.8;
  }
  .research-overview .research-theme {
    display: grid;
    grid-template-columns: minmax(12rem, 0.95fr) minmax(0, 2fr);
    gap: 2rem;
    padding: 1.5rem 0;
    border-top: 1px solid var(--global-divider-color);
  }
  .research-overview .research-theme h2 {
    margin: 0;
    font-size: 1.2rem;
    font-weight: 600;
    line-height: 1.45;
    letter-spacing: -0.01em;
  }
  .research-overview .research-theme p {
    margin: 0;
    line-height: 1.8;
  }
  .research-overview .research-cite {
    white-space: nowrap;
    font-size: 0.88em;
    font-weight: 500;
  }
  .research-overview .research-note {
    margin: 0.5rem 0 0;
    font-size: 0.875rem;
    line-height: 1.6;
  }
  @media (max-width: 700px) {
    .research-overview .research-theme {
      grid-template-columns: minmax(0, 1fr);
      gap: 0.65rem;
      padding: 1.3rem 0;
    }
    .research-overview .research-theme h2 {
      font-size: 1.15rem;
    }
  }
---

<div class="research-overview">
  <p class="research-lead">
    My research concerns <strong>singularity formation and long-time dynamics in fluid and dispersive equations</strong>.
    I study how transport, nonlinear focusing, resonance, and radiation shape the evolution of solutions and select singular or coherent structures that persist under perturbations.
  </p>

  <section class="research-theme" aria-labelledby="boundary-layer-separation-and-turbulence">
    <h2 id="boundary-layer-separation-and-turbulence">Boundary layer separation and turbulence</h2>
    <p>
      Boundary-layer separation and the generation of fine scales are important mechanisms in fluid motion.
      My interests include unsteady separation, the amplification and transport of vorticity, and their connections with turbulent motion and the interaction between viscous and inviscid flow.
    </p>
  </section>

  <section class="research-theme" aria-labelledby="vorticity-dynamics-and-fluid-stability">
    <h2 id="vorticity-dynamics-and-fluid-stability">Vorticity dynamics and fluid stability</h2>
    <p>
      Transport, stretching, and dissipation govern the evolution of vorticity and the stability of fluid structures.
      My work on vorticity models connects nonlinear structure and energy balance with fluid stability
      <a class="research-cite" href="{{ '/publications/#lei2020clm' | relative_url }}" title="Lei, Liu and Ren: On the Constantin–Lax–Majda model with convection">[LLR20]</a>.
      Related work on hypoviscous elastodynamics concerns finite-energy weak solutions in coupled fluid systems
      <a class="research-cite" href="{{ '/publications/#chen2022elastodynamics' | relative_url }}" title="Chen and Liu: Weak solutions of the three-dimensional hypoviscous elastodynamics with finite kinetic energy">[CL22]</a>.
    </p>
  </section>

  <section class="research-theme" aria-labelledby="compressible-focusing-and-collapse">
    <h2 id="compressible-focusing-and-collapse">Compressible focusing and collapse</h2>
    <p>
      Compression and attractive forces can concentrate mass and produce large velocity gradients in compressible flow.
      I am interested in the mechanisms that select collapse profiles and rates, the competition between pressure and focusing, and the stability of these regimes under perturbations.
    </p>
  </section>

  <section class="research-theme" aria-labelledby="self-similar-blow-up-in-nonlinear-waves">
    <h2 id="self-similar-blow-up-in-nonlinear-waves">Self-similar blow-up in nonlinear waves</h2>
    <p>
      Nonlinear focusing can lead to finite-time blow-up, with self-similar or generalized self-similar profiles describing the emerging scales.
      My work examines generalized self-similar blow-up in wave equations with derivative nonlinearities
      <a class="research-cite" href="{{ '/publications/#ghoul2025spatial' | relative_url }}" title="Ghoul, Liu and Masmoudi: Blow-up of the one-dimensional wave equation with quadratic spatial derivative nonlinearity">[GLM25]</a>
      <a class="research-cite" href="{{ '/publications/#liu2025time' | relative_url }}" title="Liu and Raees: Stable self-similar blow-up in nonlinear wave equations with quadratic time-derivative nonlinearities">[LR25]</a>,
      and the role of symmetry in nonlinear stability
      <a class="research-cite" href="{{ '/publications/#liu2026superconformal' | relative_url }}" title="Liu: A note on the stability of self-similar blow-up solutions for superconformal semilinear wave equations">[Liu26]</a>.
    </p>
  </section>

  <section class="research-theme" aria-labelledby="resonance-radiation-and-energy-transfer">
    <h2 id="resonance-radiation-and-energy-transfer">Resonance, radiation, and energy transfer</h2>
    <p>
      Nonlinear resonance allows localized coherent modes to exchange energy with radiation, producing damping and metastable behavior.
      My work on Hamiltonian Klein–Gordon equations examines these interactions and their long-time dynamics
      <a class="research-cite" href="{{ '/publications/#lei2026weak' | relative_url }}" title="Lei, Liu and Yang: Energy transfer, weak resonance, and Fermi’s golden rule in Hamiltonian nonlinear Klein–Gordon equations">[LLY26a]</a>
      <a class="research-cite" href="{{ '/publications/#lei2026resonances' | relative_url }}" title="Lei, Liu and Yang: Resonances, energy transfer and radiation in Hamiltonian nonlinear wave equations with multiple internal modes">[LLY26b]</a>.
      Related work on wave scattering describes how nonlinear solutions approach freely propagating waves
      <a class="research-cite" href="{{ '/publications/#he2020scattering' | relative_url }}" title="He, Liu and Wang: Scattering for the quasilinear wave equations with null conditions in two dimensions">[HLW20]</a>.
    </p>
  </section>

  <p class="research-note">Reference labels link to the full entries on the <a href="{{ '/publications/' | relative_url }}">Publications</a> page.</p>
</div>
