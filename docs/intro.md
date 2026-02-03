# Background to WetChemSyn Ontology (WCSO)

## Why WCSO exists

Wet-chemical synthesis procedures are traditionally documented in free-text form (e.g., “Experimental” or “Methods” sections). This human-centered style has worked so far, but it often relies on implicit knowledge and uses subjective wording instead of explicit parameters. This makes procedures harder to interpret, reproduce, and compare, which is especially true for machines.

At the same time, **Materials Acceleration Platforms (MAPs)** and **Self‑Driving Labs (SDLs)** are increasingly used to autonomously design and execute experiments. In these settings, machines need **precise, explicit, machine-interpretable** descriptions of steps and process parameters. When workflows are created or executed by automation, *sharing* and *reusing* them across sites becomes a central requirement, not only a side effect.

Even when two labs run very similar experiments, they often use different:
- instrument and software stacks,
- workflow/orchestrator frameworks,
- naming conventions for the same operation and parameters.

In distributed SDL environments, this leads to heterogeneous terminology and ad‑hoc metadata practices (“vocabulary drift”), which reduces interoperability and complicates cross-experiment comparison and automated analysis. This motivates a standardized semantic layer that cleanly separates *meanings of textual descriptions* from *implementations on specific platforms*.


## WCSO in a nutshell

The **WeChemSyn Ontology (WCSO)** is a **lightweight, use‑case‑driven ontology** to represent wet‑chemical synthesis workflows (especially for nano and advanced materials) as **machine-actionable “recipes”** that can be shared, queried, and interpreted across heterogeneous SDL/MAP environments.


## Foundations: PMDco and BFO alignment

WCSO is grounded in the **PMD Core Ontology (PMDco)**, a mid-level ontology for materials science and engineering (MSE), which itself builds on the **Basic Formal Ontology (BFO)**. This foundation provides:
- a stable semantic backbone for representing materials, processes, and their context,
- and an interoperability strategy aligned with a broader ecosystem of BFO‑conformant ontologies and knowledge graphs. 

In practice, this means WCSO does not reinvent general modeling concepts; instead, it specializes them for wet‑chemical synthesis workflows in SDL/MAP contexts while remaining compatible with other semantic assets used in materials science.


## What you gain by using WCSO

> ### 1) Better reproducibility and clarity
> WCSO encourages describing syntheses with explicit steps and parameters, reducing ambiguity that can arise from narrative protocols and tacit assumptions.

> ### 2) Workflow sharing across labs and platforms
> By abstracting workflow meaning away from specific orchestrators and hardware/software backends, WCSO lowers the effort needed to transfer and reuse synthesis procedures across different SDL/MAP installations. 

> ### 3) FAIR and machine-actionable representations
> Ontology-based workflow descriptions support FAIR principles - especially interoperability and reuse as procedures become structured, machine-readable research objects rather than isolated text narratives. 

> ### 4) Queryable knowledge graphs for planning and analysis
> When synthesis workflows are exported as knowledge graphs aligned with WCSO, they can be queried to retrieve planning- and reuse-relevant information (e.g., required chemicals and amounts, key parameters, outputs). This enables systematic comparison across procedures and supports data-driven decision making.


## Scope

WCSO is intentionally designed as a **practical ontology for wet‑chemical synthesis workflows** in automation-centered contexts which is focused on representing recipes in a consistent way that can be executed (or at least interpreted) by machines and shared between laboratories. It is openly maintained and meant to be extendable by the community as synthesis knowledge bases and SDL/MAP needs evolve.

