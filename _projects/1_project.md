---
layout: page
title: RNA structure and modifications
description: RNA structure, RNA modifications, and developmental regulation.
img: assets/img/rna-structure-bulge-c2b.png
importance: 1
category: work
_styles: |
  .post {
    position: relative;
    overflow: hidden;
    border-radius: 8px;
    padding: 2rem;
    isolation: isolate;
  }

  .post::before {
    content: "";
    position: absolute;
    inset: 0;
    z-index: -2;
    background-image:
      url("/assets/img/rna-structure-bulge-c2b.png"),
      url("/assets/img/rna-structure-bulge-c2b.png"),
      url("/assets/img/rna-structure-bulge-c2b.png");
    background-position: center 10%, left 70%, right 82%;
    background-repeat: no-repeat;
    background-size: min(900px, 95vw), min(520px, 55vw), min(560px, 60vw);
    opacity: 0.16;
    transform: scale(1.12);
    animation: rna-project-zoom 1400ms ease-out forwards;
  }

  .post::after {
    content: "";
    position: absolute;
    inset: 0;
    z-index: -1;
    background: var(--global-bg-color);
    opacity: 0.72;
  }

  .post-header,
  .post article {
    position: relative;
    border-radius: 8px;
    background: color-mix(in srgb, var(--global-bg-color) 82%, transparent);
    box-shadow: 0 12px 32px rgba(0, 0, 0, 0.08);
    opacity: 0;
    transform: translateY(10px);
    animation: rna-content-in 700ms ease-out 220ms forwards;
  }

  .post-header {
    margin-bottom: 1rem;
    padding: 1.25rem 1.5rem;
  }

  .post article {
    padding: 1.5rem;
  }

  @keyframes rna-project-zoom {
    from {
      opacity: 0.05;
      transform: scale(1.22);
    }
    to {
      opacity: 0.16;
      transform: scale(1.04);
    }
  }

  @keyframes rna-content-in {
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  @media (max-width: 576px) {
    .post {
      padding: 1rem;
    }

    .post-header,
    .post article {
      padding: 1rem;
    }
  }
---

RNA molecules do far more than carry genetic information. They fold into dynamic structures that control splicing, translation, RNA stability, localization, catalysis, viral replication, gene regulation, and interactions with proteins, metabolites, and other nucleic acids. Determining RNA structure is therefore essential for understanding how sequence encodes function, how RNA conformations change across developmental or disease states, and how RNA can be targeted therapeutically.

Current RNA structure determination uses a combination of high-resolution structural biology, chemical probing, sequencing-based readouts, and computational modeling. X-ray crystallography can provide atomic-resolution structures, but it often requires stable, homogeneous RNAs that crystallize well. Nuclear magnetic resonance spectroscopy is powerful for resolving RNA conformations and dynamics in solution, especially for smaller RNAs, but becomes challenging as molecular size and spectral complexity increase. Cryo-electron microscopy has become increasingly important for large RNAs and RNA-protein complexes because it avoids crystallization and can capture macromolecular assemblies closer to native states, although smaller and flexible RNAs remain difficult to resolve.

Chemical probing methods such as SHAPE, DMS, icSHAPE, and related mutational profiling approaches provide nucleotide-level information about RNA flexibility, base pairing, and structure in vitro, in cells, or across transcriptomes. These methods are valuable because they scale to many RNAs and can capture context-dependent structure, but they usually provide indirect constraints rather than complete atomic models. Their interpretation depends on probe chemistry, sequencing depth, reverse transcription behavior, RNA abundance, and computational assumptions.

A major limitation across all approaches is that RNA is not a single static object. Many RNAs occupy ensembles of conformations that shift with ions, temperature, proteins, metabolites, modifications, and cellular state. High-resolution methods can miss rare or transient conformations, while transcriptome-wide probing can lose long-range contacts and three-dimensional detail. Computational prediction has improved, but RNA tertiary structure remains difficult because flexible backbones, noncanonical base pairs, pseudoknots, modifications, and ligand- or protein-dependent folding are hard to model from sequence alone.

This project focuses on integrating experimental and computational strategies to better understand RNA structure, RNA modifications, dynamics, and function in biologically relevant developmental contexts.

## Related publications

Publications related to this current research direction will be added as they become available. See the full [publications list](/publications/).
