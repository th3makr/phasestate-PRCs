---
prc: 1
title: PRC Purpose and Guidelines
author: th3makr
status: Living
type: Meta
created: 2026-02-21
---

# PRC-1: Purpose and Guidelines

## What is a PRC?
PRC stands for Phase Request for Comment. A PRC is a design document providing information to the Phase State community, proposing a new mathematical formula for telemetry, or standardising a baseline thermodynamic schema for a specific industry.

The PRC process is the primary mechanism for collecting community input on digital thermodynamics and documenting the mathematical decisions that govern the Phase State Protocol.

## The Tracks
There are three primary tracks for submitting a PRC. **Note: We do not accept PRCs that dictate specific visual styling, CSS, or UI component designs.** The protocol is strictly concerned with the physics; visual execution is relative to the observer's brand.

### 1. Telemetry Algorithms (The Sensors)
Proposals that refine or introduce new mathematical algorithms for calculating the core sensory inputs (Gravity, Friction, Load, Velocity, Volatility, Force).
* *Example:* "PRC-07: Proposing a new time-decay formula to more accurately calculate User Volatility ($V_o$) on touchscreen devices over a 500ms rolling window."

### 2. Spacetime Schemas (The Baselines)
Proposals that establish the standard baseline JSON schemas (Base Pressure and Base Temperature) for specific digital environments, creating industry-wide defaults.
* *Example:* "PRC-404: Establishing a Base Temperature ($T$) of 0 for Tier-1 Medical Dashboards to prevent high-entropy UI thrashing during high-stress scenarios."

### 3. Protocol Integration (The API Spec)
Proposals that standardise naming conventions and architectural patterns for how existing UI kits (Tailwind, Material, Radix) map their design tokens to Phase States.
* *Example:* "PRC-12: Standardising the design-token nomenclature for phase-shifting borders in strict CSS environments."

## The Workflow
To ensure high-quality standards, the PRC lifecycle is split into two phases:

**Phase 1: Ideation (Low Friction)**
Before drafting a formal document, authors **must** open a thread in the GitHub **Discussions** tab. This allows the community to debate the mathematical or logical merits of the proposal without the friction of Git version control.

**Phase 2: Formal Submission (High Friction)**
Once consensus is reached in Discussions, the proposal moves to formal documentation:
1. **Draft:** The author forks the repository and submits a formatted Markdown file via Pull Request (PR).
2. **Review:** The core team and community review the mathematical proofs and logic within the PR.
3. **Last Call:** A 14-day window is set for final objections.
4. **Final:** The PR is merged. The standard is officially ratified and added to the Phase State Protocol. Future updates to the `th3makr` engine will support this standard.

## Document Structure
Every formal PRC must contain the following elements:
* **Preamble:** Metadata containing the PRC number, title, author, and status.
* **Abstract:** A short (~200 word) description of the technical issue being addressed.
* **Motivation:** Why is the current standard insufficient? 
* **Specification:** The exact mathematical formulas (LaTeX formatting preferred), algorithms, or JSON schemas being proposed.
* **Backwards Compatibility:** An explanation of how this change impacts existing `th3makr` implementations.
