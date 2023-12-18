---
layout: page
title: Euclidean Random Assignment Problems
show: hyde
---


<br/>

<img style="max-width:350px;float:right;margin: 15px 15px 15px 15px;padding: 10px;" src="../assets/config-n500.png">
{: style="text-align: justify" }
 <ins>In brief</ins>: given \\( 2n \\) points, \\(n\\) “reds” and \\(n\\) “blues” in a Euclidean space, solving the associated **Euclidean Assignment Problem** consists in finding the bijection between red and blue points that minimizes a functional of the distances of the point positions (an example instance at \\(n=500\\) on the unit square is depicted in figure). In the simplest stochastic version of this problem, the points are a [binomial process](https://en.wikipedia.org/wiki/Binomial_process), and some interest has developed over the years on the typical properties of the solution in the limit \\( n \to \infty \\) depending on the dimension of the ambient space and choice of cost function. The main motivations come by an analogy of this problem with a low-dimensional disordered-system and by recent results on the Monge–Kantorovich optimal transport problem.
{: style="text-align: justify" }



<ins>Works in preparation</ins>:

1. "Anomalous scaling of the optimal cost in the one-dimensional Euclidean random assignment problem: some rigorous results'',
 with A. Sportiello (2019-)

2. "The Euclidean random assignment problem at non-integer Hausdorff dimension \\( d_H \in (1,2) \\)'',
 with A. Sportiello (2020-)


<ins>Keywords</ins>: random assignment problem, statistical field theory, disordered systems in finite dimension, Monge-Kantorovich transportation problem



If you are interested in numerical simulations, you may want to have a look at [ERAP2d.py](https://github.com/matteodachille/ERAPs2d){:target="_blank"}, a Python module for easy numerical simulations of ERAPs.
