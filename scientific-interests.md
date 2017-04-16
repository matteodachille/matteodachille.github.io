---
layout: page
title: Scientific interests
order: 2
---

<!--- TOC
{:toc}-->

Mathematical aspects of statistical mechanics, disordered systems, critical phenomena and universality, with both analytical and numerical methods. The following are the specific topic I have so far contributed to.
{: .text-justify}

### Stochastic assignment problems


The _assignment problem_ is the search of a permutation \\( \pi^* \in \mathcal{S}_n \\), the symmetric group on $$n$$ symbols, that minimizes a cost or energy
{: .text-justify}

$$ E(\pi^*;w) := \min_{ \pi \in \mathcal{S}_n } E(\pi;w) = \min_{ \pi \in \mathcal{S}_n } \sum_{i=1}^n w_{i\pi(i)}
$$

where \\( w_{ij} \\) is the cost of assigning the $$i$$-th object of a certain class to the $$j$$-th one of another one. $$ E(\pi^*;w)$$ is called the _optimal cost_ or _the ground state energy_, depending on the context. Thus the problem is completely specified by a $$n\times n$$ matrix $$w$$, called ''cost matrix''. For example, you run a business and you know that employee $$i$$ can finish task $$j$$ in $$w_{ij}$$ seconds, and you would like to minimize the total employees time of execution for the whole set of $$n$$ tasks under the constraint that each employee does only one task. 
{: .text-justify}

This problem was solved by **H.W.Kuhn** in 1955[^1] with the introduction of the "Hungarian method", an algorithm that solves this problem in polynomial time complexity $$O(n^4)$$[^2]. But what happens if $$w$$ is a **random matrix**?
{: .text-justify}


Depending on the way this random matrix is built, this stochastic problem takes different names:
{: .text-justify}

- **Random Assignment Problem** (RAP) if the entries are independent and identically distributed random variables with density $$\rho$$;
- **Euclidean Bipartite Matching Problem** (EBMP), if $$w_{ij}=d^p(b_i,w_j)$$, where $$\lbrace b_i \rbrace_{i=1}^n$$ ("the blacks") and $$\lbrace w_i \rbrace_{i=1}^n$$ ("the whites") are two families of i.i.d.r.v. uniformly distributed in the unit hypercube in $$D$$ dimensions (or in the $$D$$-torus), and $$d$$ is the Euclidean distance. 
	
In these problems, where physically only typical information is known on the nature of interactions, there is lack of the most common symmetries, that are restored only on average. They also display **frustration**, in the sense that it is in general not possible to locally satisfy energy minimization. Both previous features are typically found in the statistical physics of **spin glasses**. 	
{: .text-justify}


In a seminal paper on the subject[^3], **M.Mézard** and **G.Parisi** introduced a canonical ensemble formulation for the RAP. Using the _replica method_, they showed that, in determining the asymptotics of the zero-temperature quenched free energy (i.e. the _typical optimal cost_) as $$n \to \infty$$, the only relevant property is a **universal exponent** $$r$$ characterizing the small-argument behavior of $$\rho$$: $$\rho(w_{ij})\sim w_{ij}^r$$ as $$w_{ij} \to 0$$.
{: .text-justify}


The EBMP is in many respect more difficult than the RAP due to the geometry of the underlying space; solutions may have very different qualitative behavior depending on $$D$$ and $$p$$. Remarkably, it has rich connections with different areas of mathematics, for example with the Monge-Kantorovich problem and with cycle properties of random permutations (especially in $$D=1$$).
{: .text-justify}

Since the problem at fixed instance is solved in polynomial time, current technologies allow a Monte Carlo approach to sizes up to $$n=10^4$$ on a personal computer, so that analytical predictions can be significantly tested against numerical simulations.
{: .text-justify}

The research on these problems started in [my M.Sc. thesis](downloads/masterthesis.pdf){:target="_blank"}. You can find relevant publications by [clicking here](/publications).
{: .text-justify}

<div class="tf2d" markdown="block">
![I'm rendering a big .svg image...please wait: this may take a while.](assets/size50002d.png){:width="100%"}

</div>

<p class="message"><i class="fa fa-info-circle fa-fw" aria-hidden="true"></i>The solution of an instance of the EBMP in D=2 on the unit square. Each link contributes to the total cost with its Euclidean length, which determines its color as shown in the key (image also accessible <a href="/assets/size50002d.png" target="_blank">here</a>). </p>
{: .text-justify}

**Footnotes**

[^1]:
	Kuhn, H. W. (1955), _The Hungarian method for the assignment problem_. Naval Research Logistics, 2: 83–97. [doi:10.1002/nav.3800020109](http://onlinelibrary.wiley.com/doi/10.1002/nav.3800020109/abstract){:target="_blank"}

[^2]:
	It seems the solution to this precise problem was known to Jacobi, who found it in a completely different setting in its work "_[On the study of the order of a system of differential equations with arbitrary coefficients](http://gdz.sub.uni-goettingen.de/dms/load/img/?PPN=GDZPPN002152592&IDDOC=266552){:target="_blank"}_"
	
[^3]:
	Mézard, M., & Parisi, G. (1985), _Replicas and optimization_. Journal de Physique Lettres, 46(17), 771–778. [doi:10.1051/jphyslet:019850046017077100](http://jphyslet.journaldephysique.org/en/articles/jphyslet/abs/1985/17/jphyslet_1985__46_17_771_0/jphyslet_1985__46_17_771_0.html){:target="_blank"}