# Complex Analysis Notes

A rigorous, self-contained set of lecture notes on **Complex Analysis**, covering classical theory from Cauchy's Integral Theorem to Meromorphic Functions and the Argument Principle.

---

## 📖 Table of Contents

- [About the Notes](#-about-the-notes)
- [Summary of Topics](#-summary-of-topics)
  - [Chapter 1: Cauchy's Theorem](#chapter-1-cauchys-theorem)
  - [Chapter 2: Meromorphic Functions](#chapter-2-meromorphic-functions)
- [Key Theorems Covered](#-key-theorems-covered)
- [Author & Acknowledgments](#-author--acknowledgments)

---

## 💡 About the Notes

This repository contains comprehensive course/study notes on Complex Functions written by **Wang Yuyao**. The material is structured with formal mathematical definitions, rigorous proofs, geometric intuition, and key corollaries. 

The original PDF version is compiled with LaTeX, complete with illustrated diagrams (e.g., toy contours, keyhole paths) to assist in visualization.

---

## 📚 Summary of Topics

### Chapter 1: Cauchy's Theorem
- **Goursat's Theorem**: Proof via triangular subdivision and nested compact sets without assuming $f'$ is continuous.
- **Cauchy's Theorem in Discs & Toy Contours**: Primitive existence lemmas, keyhole contours, and general closed curve path integration.
- **Cauchy's Integral Formula (CIF)**:
  - Higher-order derivative formulas
  - Cauchy Inequalities
  - Power Series Expansion Theorem
  - Liouville's Theorem
  - Fundamental Theorem of Algebra
- **Identity Theorem & Analytic Continuation**: Properties of zeros, limit points, and extension across connected domains.
- **Applications & Extensions**:
  - **Morera's Theorem** (Converse of Cauchy's Theorem)
  - **Sequences of Holomorphic Functions** (Holomorphic Limit Theorem & Uniform Convergence of Derivatives)
  - **Holomorphic Functions defined by Integrals**
  - **Schwarz Reflection Principle** & Symmetry Principle
  - **Runge's Approximation Theorem** (Cauchy representation on compact sets, rational approximation, and pole pushing)

---

### Chapter 2: Meromorphic Functions
- **Zeros and Poles**: Local factorization theorem, orders of zeros/poles, principal part expansions, and residue calculation formulas.
- **Residue Formula**: Cauchy's Residue Theorem and its extensions over general toy contours.
- **Singularities**:
  - **Removable Singularities**: Riemann's Removable Singularity Theorem.
  - **Essential Singularities**: Casorati-Weierstrass Theorem (density of image near essential singularities).
- **Meromorphic Functions**: Properties in $\mathbb{C}$ and characterization in the extended complex plane $\hat{\mathbb{C}}$ (rational functions).
- **Argument Principle**:
  - Count of zeros and poles via logarithmic derivatives.
  - **Rouché's Theorem**
  - **Open Mapping Theorem**
  - **Maximum Modulus Principle** and boundary maximum corollaries.

---

## 🔑 Key Theorems Covered

| Theorem / Principle | Description / Core Idea |
| :--- | :--- |
| **Goursat's Theorem** | $\int_{T} f(z) dz = 0$ for triangles without assuming $C^1$ continuity of $f'$. |
| **Cauchy's Integral Formula** | $f(z) = \frac{1}{2\pi i} \int_{C} \frac{f(\zeta)}{\zeta - z} d\zeta$ |
| **Liouville's Theorem** | Every bounded entire function is constant. |
| **Morera's Theorem** | Continuous functions with zero triangular integrals are holomorphic. |
| **Schwarz Reflection Principle** | Extending holomorphic functions across real boundaries via complex conjugation. |
| **Runge's Theorem** | Uniform approximation of holomorphic functions by polynomials or rational functions. |
| **Casorati-Weierstrass** | Image of a deleted neighborhood of an essential singularity is dense in $\mathbb{C}$. |
| **Rouché's Theorem** | Comparison of zero counts for perturbed functions $\|f(z)\| > \|g(z)\|$. |

---

## 🛠 Usage & PDF Compilation

To view or compile the PDF directly from the source `.tex` files (if included):

```bash
# Using pdflatex or xelatex
xelatex Complex_Analysis.tex
