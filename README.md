# Photonic Processor Research — Field Engineering Gap Analysis

This project explores photonic processor research not just as a collection of isolated papers, but as an emerging field architecture.

Instead of asking only:

- Which topics have few papers?

it asks higher-level questions such as:

- Which subfields exist?
- How strongly are they connected?
- Which connections are underdeveloped?
- Where does the field still lack higher-order integration?
- Which emergent combinations have not fully formed yet?

The goal is to move from a normal topic analysis toward a Field Engineering perspective:

> Papers are not only individual contributions.  
> Together they form modules.  
> Modules together form a field.  
> And many important gaps do not lie in the parts themselves, but in the still-unformed higher field structure.

---

## Core Idea

This repository analyzes photonic processor research in four levels:

### Level 1 — Paper Collection
Research papers are collected from OpenAlex using several photonic / optical computing related search terms.

### Level 2 — Subfield Clustering
The papers are grouped into thematic subfields, such as:

- Hardware & Chip Design
- Optical Neural Networks
- Photonic Accelerators
- Quantum & Sensing
- Phase Change & Memory
- Matrix & Linear Algebra

### Level 3 — Field Architecture
These subfields are then treated as nodes of an emerging field architecture.

The analysis examines:

- semantic similarity
- citation / connection structure
- subfield size
- temporal development
- overall network structure

### Level 4 — Field Engineering Gaps
The final layer identifies underdeveloped connections between subfields.

This is not only a search for “small topics,” but for:

- structural gaps
- functional gaps
- emergent gaps
- missing bridges between modules
- areas where a higher-order field effect has not yet fully formed

---

## Why This Matters

Photonics is often discussed in terms of devices, accelerators, optical neural networks, or hardware performance.

But the more interesting question may be:

How does the field organize itself as a whole?

A field can contain many papers and many strong components, while still lacking:

- integration across modules
- memory-compute coupling
- sensing-compute bridges
- architecture-level coherence
- emergent system-level applications

This project tries to make these missing structures visible.

---

## Current Analysis Outputs

The current pipeline generates several outputs to analyze the field from different perspectives:

### 1. Gap Matrix
A matrix showing relative under- or over-connection between subfields.

Interpretation:

- positive values = weaker connection than expected → possible gap
- negative values = stronger connection than expected

### 2. Growth vs. Impact Plot
A momentum map comparing:

- subfield growth rate
- citation impact
- number of papers

This helps distinguish between:

- mature high-impact areas
- fast-growing emerging fields
- high-volume but weaker-impact areas
- small but influential subfields

### 3. Subfield Network
A network graph showing how strongly the different subfields are connected.

This helps reveal:

- central fields
- bridge fields
- isolated modules
- possible structural weak points

### 4. Publication Trends
A time-series view of subfield development from 2015–2025.

This helps identify:

- emerging waves
- stable infrastructure fields
- recent acceleration
- possible hype vs. consolidation dynamics

---

## Method Overview

The analysis currently follows this logic:

### Step 1 — Data Collection
Papers are pulled from OpenAlex using photonic-computing-related search terms.

### Step 2 — Relevance Filtering
A relevance score is applied to keep papers closer to the core field.

### Step 3 — Clustering
Papers are clustered into subfields.

### Step 4 — Architecture Construction
A subfield-level network is built from the clustered papers and their interrelations.

### Step 5 — Gap Scoring
For each subfield pair, the analysis compares:

- expected connection strength
- actual connection strength

The current gap score is:

```python
gap = (expected - actual) / expected
