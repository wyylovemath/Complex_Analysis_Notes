# Complex Analysis Lecture Notes

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Status: In Progress](https://img.shields.io/badge/Status-Active-brightgreen.svg)]()
[![Topic: Mathematics](https://img.shields.io/badge/Topic-Complex%20Analysis-orange.svg)]()

> A structured and comprehensive set of lecture notes on **Complex Analysis**, covering foundational theorems, rigorous proofs, and key applications.

---

## ✍️ Author & Overview

* **Author:** Wang Yuyao
* **Subject:** Complex Analysis / Holomorphic Function Theory
* **Document Source:** [`Complex_Analysis.pdf`](./Complex_Analysis.pdf)

These notes provide a mathematically rigorous introduction to classical complex analysis, starting from contour integrals and foundational principles up to advanced approximation theorems.

---

## 📚 Table of Contents

- [Chapter 1: Cauchy's Theorem](#chapter-1-cauchys-theorem)
  - [1.1 Goursat's Theorem](#11-goursats-theorem)
  - [1.2 Cauchy's Theorem in Discs](#12-cauchys-theorem-in-discs)
  - [1.3 Cauchy's Integral Formula (CIF)](#13-cauchys-integral-formula-cif)
  - [1.4 Identity Theorem](#14-identity-theorem)
  - [1.5 Applications](#15-applications)
    - [1.5.1 Morera's Theorem](#151-moreras-theorem)
    - [1.5.2 Sequences of Holomorphic Functions](#152-sequences-of-holomorphic-functions)
    - [1.5.3 Holomorphic Functions Defined via Integrals](#153-holomorphic-functions-defined-via-integrals)
    - [1.5.4 Schwarz Reflection Principle](#154-schwarz-reflection-principle)
    - [1.5.5 Runge's Approximation Theorem](#155-runges-approximation-theorem)
- [✨ Key Highlights & Theorems](#-key-highlights--theorems)
- [🛠 Requirements & Compilation](#-requirements--compilation)
- [📄 License](#-license)

---

## 📖 Detailed Content Outline

### Chapter 1: Cauchy's Theorem

#### 1.1 Goursat's Theorem
* **Motivation:** Simplifying conditions on closed curves $\gamma$ via triangle partitioning.
* **Theorem:** Proof using triangle subdivision $T^{(0)} \supseteq T^{(1)} \supseteq \dots \supseteq T^{(n)}$, diameter shrink rates, and first-order expansions at the limit point $z_0 \in \Omega$.
* **Corollary:** Extension to rectangles $R \subset \Omega$.

#### 1.2 Cauchy's Theorem in Discs
* **Local Existence-of-Primitives Lemma:** Constructing $F(z) = \int_{\gamma_{0,z}} f(w)\,dw$ on open discs.
* **Toy Contours & Keyhole Contours:** Introduction of narrow-corridor contours $\Gamma_{\delta,\epsilon}$ for pole avoidance.
* **Cauchy's Theorem:** Vanishing contour integrals for closed curves in open discs.

#### 1.3 Cauchy's Integral Formula (CIF)
* **Core Formula:**
  $$f(z) = \frac{1}{2\pi i} \int_{C} \frac{f(\zeta)}{\zeta - z} \, d\zeta$$
* **Corollaries & Key Results:**
  1. **Higher Derivatives:** $f^{(n)}(z) = \frac{n!}{2\pi i} \int_{C} \frac{f(\zeta)}{(\zeta - z)^{n+1}} \, d\zeta$
  2. **Cauchy Inequalities:** Bounds on $|f^{(n)}(z_0)|$ via $R^n$.
  3. **Power Series Expansion:** Local analyticity of holomorphic functions.
  4. **Liouville's Theorem:** Bounded entire functions are constant.
  5. **Fundamental Theorem of Algebra:** Existence and factorization of roots in $\mathbb{C}$.

#### 1.4 Identity Theorem & Analytic Continuation
* Zeros of non-zero holomorphic functions are isolated.
* Uniqueness of analytic extensions over connected domains $\Omega$.

#### 1.5 Applications
* **1.5.1 Morera's Theorem:** Converse of Cauchy's Theorem via triangular path integrals.
* **1.5.2 Sequences of Holomorphic Functions:**
  * **Holomorphic Limit Theorem:** Uniform limits of holomorphic functions on compact subsets are holomorphic.
  * **Uniform Convergence of Derivatives:** $f_n' \to f'$ uniformly on compact sets.
* **1.5.3 Integrals with Parameters:** Holomorphicity of $f(z) = \int_{a}^{b} F(z,s)\,ds$.
* **1.5.4 Schwarz Reflection Principle:** Extending holomorphic functions across real boundary segments via symmetry ($f(\bar{z}) = \overline{f(z)}$).
* **1.5.5 Runge's Approximation Theorem:**
  * Integral representations on compact sets.
  * Rational function approximation and the **Pole Pushing Lemma**.
  * Uniform polynomial approximation when $K^c$ is connected.

---

## ✨ Key Highlights & Theorems Summary

| Theorem / Principle | Main Statement / Result |
| :--- | :--- |
| **Goursat's Theorem** | $\int_T f(z)\,dz = 0$ for any triangle $T \subset \Omega$ and $f \in \text{Hol}(\Omega)$. |
| **Cauchy's Integral Formula** | Expresses internal values $f(z)$ purely in terms of boundary values on $C$. |
| **Liouville's Theorem** | Every bounded entire function is constant. |
| **Morera's Theorem** | Continuous $f$ with zero integrals over all triangles is holomorphic. |
| **Schwarz Reflection** | Holomorphic functions real on $I_\Omega$ extend analytically across the real axis. |
| **Runge's Theorem** | Holomorphic functions can be uniformly approximated by polynomials if $K^c$ is connected. |

---

## 🛠 Building / Compiling the Notes

If you wish to recompile the LaTeX source file to generate the PDF:

```bash
# Compile using pdflatex or xelatex
xelatex Complex_Analysis.tex

# Re-run for table of contents and cross-references
xelatex Complex_Analysis.tex
