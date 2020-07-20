---
layout: page
title: Scientific interests
order: 2
---

Statistical mechanics in random combinatorial optimization; phase transitions; scaling and universality.


<!-- I am interested in ...
The Euclidean Random Assignment Problem and, more broadly, typical properties of large random structures.
{: .text-justify}
-->

### Current projects

#### - Euclidean Random Assignment Problem (2017-)

Works in preparation:

- Random assignment problems on \\( 2d \\) manifolds
 with *D. Benedetto, E. Caglioti, S. Caracciolo, G. Sicuro and A. Sportiello*.


- Field theoretic approach to the Euclidean random assignment problem
with *S. Caracciolo, G. Sicuro and A. Sportiello*.

- The Euclidean random assignment problem at non-integer Hausdorff dimension \\( d_H \in (1,2) \\)
 with *A. Sportiello*.

- Anomalous scaling of the optimal cost in the one-dimensional Euclidean random assignment problem: some rigorous results
 with *A. Sportiello*.

 Further details on the ERAP (and other random combinatorial optimization problems) can be found [at this ResearchGate project page](https://www.researchgate.net/project/Bipartite-matching-relationship-between-random-and-Euclidean-graphs).
 {: .text-justify}

<!--
#### Some motivations

Formally, an ERAP is a linear sum assignment problem[^9] in which the assignment of \\( n \\) objects (the blue points, say) to another set of \\( n \\) objects (the red points, say) minimises a global energy function \\( \mathcal{H}(\pi) \\) which is linear in the contribution of each edge. This choice, coupled with the convexity of the search space, makes the problem simple, and a solution can be found in polynomial time under rather mild conditions[^1]. A configuration of minimal energy can be specified by a permutation \\(\pi^\* \\), which is called the optimal assignment or ground state. In an ERAP, blue and red points are families of i.i.d. random variables drawn from a given probability measure \\( \mu \\) supported on a metric space \\( \mathcal{M} \\) of Hausdorff dimension \\( d_H \\). \\( c_{ij} \\), the \\( ij \\)-th entry of the cost matrix, is a scale invariant function of the \\(d\\)-dimensional Euclidean distance between blue \\(i\\) and red \\(j\\), such as \\( c(x) = \|x \|^p \\) with \\( p \in \mathbb{R} \\). These aspects qualify the ERAP as a prototypical and genuinely finite-dimensional example of a critical (due to having the same number of points of each color), frustrated (due to the Euclidean correlations) and disordered system, in which analytical predictions can be tested by simple numerical explorations (an example of solution to an ERAP at \\(d=2\\) on the unit square is given in the following figure).
{: .text-justify}

<!--
For example, the energy function \\( \mathcal{H}\\) of an ERAP, with the above choice of cost function \\(c\\) depending on \\(p\\), corresponds to the \\(p\\)-Wasserstein distance (to the power \\(p\\)) between the two empirical measures associated to blue and red points. Monge-Kantorovich duality in the continuum, which corresponds to linear programming duality in a discrete setting[^8], corresponds to the physical fact that the ground state energy (which is a sum of non-local terms) can be written as a sum of local quantities, sometimes termed _prices_ or _cavity fields_:
{: .text-justify}

\\[ c_{i\pi^\*(i)}=u_i+v_{\pi^\*(i)} \qquad \forall i=1,\ldots,n \\]

-->
<!--
<div class="tf2d" markdown="block">

![I'm rendering a big image... please wait: depending on the speed of your connection this may take a while.]({{ site.url }}/assets/size50002d.png){:width="100%"}

</div>

<p class="message"><i class="fa fa-info-circle fa-fw" aria-hidden="true"></i>Instance of an ERAP in the unit square with the uniform measure. Here, the n=5000 blue and red points are not shown for clarity, and p=1, so that arrows connecting optimally matched points do not cross. Each arrow has been assigned a color to emphasize its contribution to the ground state energy (colorbar). This image can be downloaded <a href="assets/size50002d.png" target="_blank">here</a>. </p>
{: .text-justify}
<br/>

The ERAP is also intimately related to a well-known problem in the calculus of variations, the so-called Monge-Kantorovich problem in optimal transport. Some aspects of this correspondence can be at least traced back to the work of Leonid Kantorovich, recipient of the Nobel Prize in Economics in 1975 for his work on the optimal allocation of resources and one of the ``founding fathers'' of optimal transport[^8]. Moreover, like any assignment problem, the ERAP can also be interpreted in terms of the optimal strategy in a certain zero-sum, two player non-cooperative game[^15]. It is interesting to notice that within this context results based on physical arguments [^5][^11][^12] have been proven rigorously much later[^6][^13][^14], and often raised new and challenging questions.
{: .text-justify}

We have started a program of investigations of the ERAP combining analytical and numerical methods (see the [publications](/publications) page for some relevant references).
Further details on the ERAP and other stochastic combinatorial optimisation problems may be found at this [ResearchGate project page](https://www.researchgate.net/project/Bipartite-matching-relationship-between-random-and-Euclidean-graphs).
{: .text-justify}


**(Essential) references**

[^1]:
    Kuhn, H. W. (1955), _The Hungarian method for the assignment problem_. Naval Research Logistics, 2: 83–97. [doi:10.1002/nav.3800020109](http://onlinelibrary.wiley.com/doi/10.1002/nav.3800020109/abstract){:target="_blank"}

[^2]:
    McCann, R. J. (1999). _Exact solutions to the transportation problem on the line_. Proceedings of the Royal Society of London. Series A: Mathematical, Physical and Engineering Sciences, 455(1984), 1341–1380. [doi:10.1098/rspa.1999.0364](https://doi.org/10.1098/rspa.1999.0364){:target="_blank"}

[^3]:
    Orland, H., & Zee, A. (2002). _RNA folding and large N matrix theory_. Nuclear Physics B, 620(3), 456–476. [doi:10.1016/S0550-3213(01)00522-3](https://doi.org/10.1016/S0550-3213(01)00522-3){:target="_blank"}

[^4]:
    Shah, D., Giaccone, P., & Prabhakar, B. (2001). _An efficient randomized algorithm for input-queued switch scheduling_. Proceedings - Symposium on the High Performance Interconnects, Hot Interconnects.
  [doi:10.1109/HIS.2001.946686](https://doi.org/10.1109/HIS.2001.946686){:target="_blank"}

[^5]:
    Mézard, M., & Parisi, G. (1985), _Replicas and optimization_. Journal de Physique Lettres, 46(17), 771–778. [doi:10.1051/jphyslet:019850046017077100](http://jphyslet.journaldephysique.org/en/articles/jphyslet/abs/1985/17/jphyslet_1985__46_17_771_0/jphyslet_1985__46_17_771_0.html){:target="_blank"}

[^6]:
    Aldous, D. J. (2001). _The ζ(2) limit in the random assignment problem_. Random Structures and Algorithms. [doi:10.1051/10.1002/rsa.1015](https://doi.org/10.1002/rsa.1015){:target="_blank"}


[^7]:
    Talagrand, M. (2004). _Spin Glasses: A Challenge for Mathematicians – Cavity and Mean Field Models_. Springer, 2003.
    [Publisher website](https://www.springer.com/gp/book/9783540003564){:target="_blank"}

[^8]:
    Villani, C. (2009). _Optimal transport, old and new_ (Springer). [doi:10.1007/978-3-540-71050-9](https://doi.org/10.1007/978-3-540-71050-9){:target="_blank"}

[^9]:
    Burkard, R. E., & Çela, E. (1999). _Linear Assignment Problems and Extensions_. In Handbook of Combinatorial Optimization (pp. 75–149). [doi:10.1007/978-1-4757-3023-4_2](https://doi.org/10.1007/978-1-4757-3023-4_2){:target="_blank"}

[^10]:
    Mezard, M., Parisi, G., & Virasoro, M. (1986). _Spin Glass Theory and Beyond_ (World Scientific). [doi:10.1142/0271](https://doi.org/10.1142/0271){:target="_blank"}

[^11]:
    Parisi, G. (1998). _A Conjecture on random bipartite matching_. ArXiv. Retrieved from [ArXiv/cond-mat/9801176](http://arxiv.org/abs/cond-mat/9801176){:target="_blank"}

[^12]:
    Caracciolo, S., Lucibello, C., Parisi, G., & Sicuro, G. (2014). _Scaling hypothesis for the Euclidean bipartite matching problem_. Physical Review E, 90(1), 012118.[doi:10.1103/PhysRevE.90.012118](https://doi.org/10.1103/PhysRevE.90.012118){:target="_blank"}

[^13]:
    Linusson, S., & Wästlund, J. (2003). _A proof of Parisi’s conjecture on the random assignment problem_. Probab. Theory Relat. Fields, 62(10831001), 1–7. [doi:10.1007/s00440-003-0308-9](https://doi.org/10.1007/s00440-003-0308-9){:target="_blank"}

[^14]:
    Ambrosio, L., Stra, F., & Trevisan, D. (2019). _A PDE approach to a 2-dimensional matching problem_. Probability Theory and Related Fields. [doi:10.1007/s00440-018-0837-x](https://doi.org/10.1007/s00440-018-0837-x)

[^15]:
    von Neumann, J. (1953). _1. A Certain Zero-sum Two-person Game Equivalent to the Optimal Assignment Problem_. In H. W. Kuhn & A. W. Tucker (Eds.), Contributions to the Theory of Games (AM-28), Volume II (pp. 5–12). [doi:10.1515/9781400881970-002](https://doi.org/10.1515/9781400881970-002)

-->
