---
layout: post
title:  "A simple lemma in trigonometry."
date:   2020-07-12 10:30:00 -0600
categories: Lemma
tags: Trigonometry Induction
---

Let \\(\theta_1, \theta_2,\ldots, \theta_k \\) be angles and \\(s_1,\ldots,s_k\\) boolean variables in \\(\lbrace 0,1\rbrace \\). Let \\(b_i = \theta_i + s_i \frac{\pi}{2} \\). Then
\\[ \sum_{s_1,\ldots,s_k \in \lbrace 0,1\rbrace^k} \left(\prod_{i=1}^k \cos b_i \right) \cos{\left(\sum_{i=1}^k b_i \right)} = 1. \\]

_Proof._

By induction. Let \\( L_k \\) be the expression in Lemma at \\( k \\). At \\(k=1\\)
\\[ L_1 = \sum_{s \in \lbrace 0,1\rbrace} \cos^2\left(\theta +s \frac{\pi}{2}\right) =\cos^2 \theta +\sin^2 \theta = 1.  \\]

Let us assume that Lemma holds at \\(k \\) and show that it holds at \\(k+1\\). Calling \\( \varphi_k = \sum_i^k b_i\\), we have
$$
\begin{align*}
L_{k+1} & = \sum_{s_1,\ldots,s_k \in \lbrace 0,1\rbrace^k} \left(\prod_{i=1}^{k} \cos b_i \right)\left[\cos{\theta_{k+1}}\cos{\left(\theta_{k+1}+\varphi_k\right)}-\sin{\theta_{k+1}}\cos{\left(\theta_{k+1}+\varphi_k+\frac{\pi}{2}\right)} \right] \\
& = \sum_{s_1,\ldots,s_k \in \lbrace 0,1\rbrace^k} \prod_{i=1}^{k} \cos b_i \left[\cos^2 \theta_{k+1}\cos{\varphi_k} + \sin^2 \theta_{k+1}\cos{\varphi_k}  \right] \\
& = \sum_{s_1,\ldots,s_k \in \lbrace 0,1\rbrace^k} \left(\prod_{i=1}^{k} \cos b_i\right) \cos \varphi_k = L_k. \qquad \blacksquare
\end{align*}
$$
