---
layout: default
---

# Yunfeng Xiong (熊云丰）

I am currently working as the Boya Postdoctoral Fellow at School of Mathematical Sciences, Peking Univeristy. I got my Ph.D. degree of computational mathematics in June, 2020, at Peking University, China. My supervisor is Prof. Sihong Shao. The title of my thesis is _Many-body Wigner dynamics: Branching Random Walk and Particle Annihilation_.

Please [click here](./CV_PKU_Yunfeng_Xiong.pdf) to see my curriculum vitae.

# Research interests

My major research interest is the mathematical theory of particle methods, as well as their applications in solving high-dimensional PDEs arsing from the quantum physics and finances.  

The concept of particle method is closely related to the Monte Carlo methods. However, the usage of particle methods does not merely involve sampling process, but actually they are integrated applications of stochastic process, numerical mathematics, number theory, statistical learning, combinatorics, harmonic analysis and so on. 

![Connection](./assets/img/ch1_connection.pdf)

* * *

## Particle methods in quantum mechanics 

My graduate research concentrates on the particle method of the Wigner equation, a phase-space formulation of quantum dynamics initialized by Eugene Wigner. The fundamental obstacle is the **negative sign** in the probailistic model, which might be disliked by mathematicians majored in probability theory, but seems fundamental for physicists as the **negative probability** in quantum world intuitively manifests the Heisenberg's uncertainty principle.  

After fighting with the notorious negative sign problem for five years, I have tried to understand its origin and made the first attempt to solve the Wigner equation on the 12-D phase space, with both developments in particle generation and annihilation. But it still has a long way to go before touching the limit of the particle method. 

Currently, I am trying to extend the basic idea of the proposed particle method to solve high-dimensional PDEs in mathematical finance and to understand the complex interactions among multiple assets. 

* * *

### Particle generation: Connection between stochastic process and PDEs

Connection between stochastic processes and PDEs is an active topic in modern mathematics and provides powerful tools for both probability theory and analysis. The particle method borrows its essential idea but can be extended to a more general class of PDEs (beyond parabolic-type and elliptic-type) by introducing the negative particle sign.

The following animation is the Wigner dynamics of an electron interacting with a Gaussian barrier in the phase space.

![asm](./assets/img/asm.gif)

Under the particle formalism, the dynamics seems likes the stochastic reproduction and mitigation of two swarms. An interesting observation is that by taking expectation, the behaviours of particles obey some rules driven by the deterministic equation. So our main goal is to understand the profound connection behind it.

![branching](./assets/img/branching.gif)


* * *

### Particle annihilation: Probability theory and combinatorics 

Intuitively, the contribution of particles carrying opposite sign can be canceled out. This observation is pivital in suppressing the stochastic variances in long-time simulations. Such problem is closely related to the density estimation in statistical learning, which intends to postulate the underlying continuous density from the discrete point distribution. 

![wf_discrete](./assets/img/wf_sample.pdf)
![wf_discrete](./assets/img/wignerfunction.pdf)

Our strategy is to combine the **sequential clustering** of points (_combinatorial technique_) and **random matching** within each group (_probabilistic technique_). The sequential clustering can be performed by binary splitting of the Eucledian space and controlling the number-theoretic discrepancies. This can automatically monitor the concentration and sparsity of point distributions, and may work in high dimensional problem (numerical examples are provided up to 1080 dimension).


![wf_ded](./assets/img/wf_ded.pdf)


* * *

### Deterministic parallel solvers for high-dimensional Wigner equation 

A parallel line in my research is to design determistic solvers for the Wigner equation. The targets are as twofold. The first is to provide a highly accurate solution to the Wigner equation. The second is to give a thorough benchmark on the particle method.

In 2016, we made the first attempt to solve the Wigner equation in 4-D phase space using the semi-Lagrangian method and spectral method. After that, my collabators, Dr. Zhenzhu Chen and Prof. Sihong Shao have succeeded in simulating the complicated structure of [double-well interference](https://doi.org/10.1016/j.jcp.2019.06.047).   

At present, I am working on a project to surmount the numerical challenges in 6-D simulations with recent developments of parallel and distributed computing. 

* * *

## Ongoing project: Diffusive wave modeling 

I am going to inintialize a project on diffusive wave modeling with [Prof. Xu Guo](https://www.tjsl.sdu.edu.cn/info/1331/8187.htm) at School of Civil Engineering, Shandong University. The goal of this project is to understand the mathematical foundation of fractional wave equation in modeling the intermediate state of the heat diffusion and the wave propogation, to design effecient algorithms for multidimensional fractional wave equation, and to discuss related problems such as reverse-time mitigation, uncertainty qualification and parameter estimation. 


The background is the wave attentuation phenomenon in earth science. The mathematical problems involve PDE analysis, numerical PDEs, numerical algebra, statistical learning, Bayesian interference and uncertainty qualification (and maybe more).    

* * *

## Mottos

- “The full meaning of life, the collective meaning of all human desires, is fundamentally a mystery beyond our grasp.” —— **Eugene Wigner**

- “A basic idea behind the design of numerical schemes is that they can preserve the properties of the original problems as much as possible ... ”
—— **Kang Feng**


