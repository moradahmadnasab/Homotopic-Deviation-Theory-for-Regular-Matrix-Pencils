# Homotopic Deviation Theory for Regular Matrix Pencils

## Overview
This repository accompanies the research paper:

**"Homotopic Deviation Theory for Regular Matrix Pencils"**  
by Morad Ahmadnasab and Panayiotis J. Psarrakos, 2024.

We generalize the theory of homotopic deviation of square complex matrices to **regular matrix pencils**.  
The study focuses on the existence and analyticity of the resolvent of deviated matrix pencils,  
the limits of both the resolvent and the spectrum as the deviation parameter grows,  
and structural changes described via the Weierstrass canonical form.

---

## Abstract
We generalize the theory of homotopic deviation of square (complex) matrices to regular matrix pencils.  
To this end, we study the existence and the analyticity of the resolvent of the matrix pencils whose matrices are under homotopic deviation with the deviation parameter  
$t \in \mathbb{C}$.  

Moreover, we investigate and identify the limits of both the resolvent and the spectrum of the deviated matrix pencils, as $|t| \to \infty$.  
We also study the special cases where $t$ tends to the eigenvalues of the related matrix pairs.  
We use the notions and the results of the generalized homotopic deviation theory to analyze the Weierstrass structure of the deviated matrix pencils under two different assumptions.  

Numerical examples illustrate and support the theoretical results.

---

## Introduction
Consider a matrix pencil
\[
P(\lambda) = A - \lambda B,
\]
where $A, B \in \mathbb{C}^{n \times n}$.  
The spectrum is defined as
\[
\sigma(A,B) = \{\lambda \in \hat{\mathbb{C}} : \det(A - \lambda B) = 0\}.
\]

We perturb the pencil by introducing a deviation parameter $t$:
\[
P(\lambda,t) = (A+t\Delta A) - \lambda(B + t\Delta B).
\]

This repository provides numerical experiments and MATLAB codes to illustrate:
- Existence and analyticity of the resolvent $R(\lambda,t) = P(\lambda,t)^{-1}$,
- Behavior of $\sigma(P(\lambda,t))$ as $|t| \to \infty$,
- Relation between deviation parameter $t$ and eigenvalues $\lambda(t)$,
- Weierstrass structure under two assumptions:
  1. $\lambda$ varies as parameter,
  2. $t$ varies as parameter.

---

## Repository Contents
- `src/` : MATLAB scripts for assembling deviated pencils and computing resolvents/spectra.
- `examples/` : Numerical experiments from the paper.
- `figures/` : Plots reproduced from the paper.
- `docs/` : Drafts of the paper in LaTeX (if included).

---

## Numerical Experiments
The numerical experiments validate the theoretical results using MATLAB R2019a (9.6).  
The machine precision was $u=2^{-53} \approx 1.1 \times 10^{-16}$.  

Example experiments include:
- Resolvent norm vs. deviation parameter $t$,
- Spectrum trajectories as $t$ increases,
- Verification of analyticity disks,
- Structural changes in the Weierstrass form.

---

## Figures
The following figures illustrate results from the paper:

- **Figure 1**: Spectrum trajectories of deviated pencil.  
  ![Spectrum trajectories](figures/spectrum_trajectories.png)

- **Figure 2**: Resolvent norm vs. $|t|$.  
  ![Resolvent norm](figures/resolvent_norm.png)

- **Figure 3**: Weierstrass structure under varying $t$.  
  ![Weierstrass structure](figures/weierstrass_structure.png)

*(Please add the actual plots to `figures/` and update the filenames.)*

---

## Installation
Clone this repository:
```bash
git clone https://github.com/your-username/homotopic-deviation-pencils.git
cd homotopic-deviation-pencils
