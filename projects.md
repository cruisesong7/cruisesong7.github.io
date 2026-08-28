---
layout: page
title: Projects
permalink: /projects/
description: Selected projects by Congyan (Cruise) Song.
---

<style>
  .proj-icons { display: inline-block; margin-left: 8px; font-size: 1.05rem; }
  .proj-icons a { margin: 0 4px; color: #777; text-decoration: none; }
  .proj-icons a:hover { color: #0077cc; }
  @media (prefers-color-scheme: dark) {
    .proj-icons a { color: #8a8f98; }
    .proj-icons a:hover { color: #3eb7f0; }
  }
  .proj-topic { margin-top: 34px; margin-bottom: 12px; font-size: 1.3rem; border-bottom: 1px solid #e5e5e5; padding-bottom: 5px; }
  @media (prefers-color-scheme: dark) { .proj-topic { border-bottom-color: #2a2b35; } }
  .proj-title { margin-bottom: 4px; }
</style>

<h2 class="proj-topic">Formalization of Ramsey Theory</h2>

<h3 class="proj-title">formal_ramsey
  <span class="proj-icons">
    <a href="https://github.com/cruisesong7/formal_ramsey" title="GitHub repository" target="_blank" rel="noopener"><i class="fab fa-github"></i></a>
  </span>
</h3>

A Lean 4 formalization of finite Ramsey theory, proving exact values for several small
Ramsey numbers and related van der Waerden numbers. We also give Lean-verified SAT
encodings for Ramsey numbers and demonstrate the use of LRAT proofs in Lean. This is
the project behind our CICM 2024 paper, *"Formalizing Finite Ramsey Theory in Lean 4,"*
and we plan to submit it to mathlib as a reusable library for Ramsey-theoretic results.

<h3 class="proj-title">RamseyLemmas
  <span class="proj-icons">
    <a href="https://github.com/cruisesong7/RamseyLemmas" title="GitHub repository" target="_blank" rel="noopener"><i class="fab fa-github"></i></a>
    <a href="https://cruisesong7.github.io/RamseyLemmas/" title="Documentation" target="_blank" rel="noopener"><i class="fa-regular fa-file-lines"></i></a>
  </span>
</h3>

Formalizing results in Ramsey theory due to [Graver and Yackel](https://doi.org/10.1016/S0021-9800%2868%2980038-9),
which were used in the SAT certification of the Ramsey numbers R(3,8) and R(3,9) by
[Zhengyu Li](https://arxiv.org/abs/2502.06055).

<h2 class="proj-topic">Verifying Parsers</h2>

<h3 class="proj-title">cedar-spec
  <span class="proj-icons">
    <a href="https://github.com/cruisesong7/cedar-spec/tree/cruise-docs" title="GitHub repository" target="_blank" rel="noopener"><i class="fab fa-github"></i></a>
    <a href="https://cruisesong7.github.io/cedar-spec/" title="Documentation" target="_blank" rel="noopener"><i class="fa-regular fa-file-lines"></i></a>
  </span>
</h3>

Cedar is AWS's open-source authorization policy language and the engine behind Amazon
Verified Permissions. This project formally verifies Cedar's extension parsers — for
decimals, durations, datetimes, and IP addresses — with all correctness theorems
machine-checked in Lean 4. Part of my internship with the Amazon Automated Reasoning group.

<h3 class="proj-title">triptych
  <span class="proj-icons">
    <a href="https://github.com/cruisesong7/triptych" title="GitHub repository" target="_blank" rel="noopener"><i class="fab fa-github"></i></a>
    <a href="https://cruisesong7.github.io/triptych/" title="Documentation" target="_blank" rel="noopener"><i class="fa-regular fa-file-lines"></i></a>
  </span>
</h3>

A Lean 4 grammar-to-parser compiler for flat, non-recursive string formats. From a single
grammar definition, triptych produces three coordinated outputs — a human-readable
specification, a verified executable parser, and machine-checked correctness theorems —
relying only on standard Lean axioms.

<h2 class="proj-topic">Lean Tools</h2>

<h3 class="proj-title">LeanGraphMaker
  <span class="proj-icons">
    <a href="https://github.com/cruisesong7/LeanGraphMaker" title="GitHub repository" target="_blank" rel="noopener"><i class="fab fa-github"></i></a>
    <a href="https://conf.researchr.org/home/splash-issta-2026/hatra-2026" title="Documentation / paper" target="_blank" rel="noopener"><i class="fa-regular fa-file-lines"></i></a>
  </span>
</h3>

Widgets and tactics that let you generate, manipulate, and visualize graphs and
their substructures on a canvas embedded in the Lean 4 Infoview. Visual data is
sent back to the Lean workspace via RPC and parsed into formal terms. This is the
project behind our HATRA 2026 paper, *"Just Draw It."*

<h3 class="proj-title">Imandra-Lean
  <span class="proj-icons">
    <a href="https://github.com/cruisesong7/Imandra-Lean" title="GitHub repository" target="_blank" rel="noopener"><i class="fab fa-github"></i></a>
  </span>
</h3>

Work from my internship at Imandra: extending Imandra-Geo, a solver for nonlinear
real arithmetic, to generate proof certificates in Lean, plus custom
Lean tactics (via metaprogramming) that normalize nonlinear real arithmetic
expressions and translate Lean syntax into Imandra-Geo input.
