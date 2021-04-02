---
layout: post
title:  "Exact expected cost in the one-dimensional ERAP for a generic translation-invariant cost function"
date:   2021-03-18 22:31:47
categories: Problems
tags: ERAP HypergeometricFunctions
---

During a recent talk of mine at the ALEA Days 2021 (see [here]() and [here]() for slides), Nathanaël Enriquez asked in which generality one can hope to obtain exact formulas for the expected ground state energy in the 1d ERAP in the convex regime for \\(n\\), \\(\sim U[0,1]\\) blue and red points. Here, _exact_ means valid at any fixed \\(n\\)), and _nice_ means that can be written without the explicit use of hypergeometric functions. This question started a discussion involving also Andrea Sportiello. A general argument in this direction can be made based on a connection with generalized Selberg integrals discovered by Caracciolo et al. [here](). There, the authors have shown that the \\(k\\)-th edge contributes to the total energy through the possibly intimidating expression (see [here](), eq. 2.4)
\\[
M_{p,k,n}= \frac{\Gamma^2(n+1)\Gamma(k+\frac{p}{2})\Gamma(n-k+1+\frac{p}{2})\Gamma(1+p)}{\Gamma(k)\Gamma(n-k+1)\Gamma(n+1+\frac{p}{2})\Gamma(n+1+p)\Gamma(1+\frac{p}{2})}
\\]

This result allowed the authors to show that, for the usual choice of cost function \\(D^p\\) with \\(p\geq 1\\),
\\[
E(n) = \frac{\Gamma \left(1+\frac{p}{2}\right)}{p+1} n \frac{\Gamma(n+1)}{\Gamma \left(n+1+\frac{p}{2}\right)},
\\]
where \\(\Gamma \\) is Euler's function.

The questions is thus whether one can cook up a cost function admitting a series representation which plays nicely with the moments, so that a sufficiently simple expression for \\(E(n)\\) can be obtained via resummation.

A natural choice is



As of today

- \\(f(r) =\cosh{r}\\)
- \\(f(r) =J_0(r)\\) (Bessel function of order 0)
