---
title: Statistiscal properties of Random Dynamical Systems
separator: <!--s-->
verticalSeparator: <!--v-->
theme: ./themes/arno/arno-theme.css
revealOptions:
  transition: 'fade'
---

# Statistical properties of Random Dynamical Systems

### Alexander B

#### 16-01-2023 at 21:04

<!--s-->

# Outline

- Introduction
- Deterministic local dynamics
  - Definition of a random map
  - Toy Model
  - A Reformulation of the Model
  - Transfer operators and invariant measures
  - Helly's selection theorem

<!--v-->

## Introduction

### Consider

- $(X_n)_n$ $\mathbb{R}$-valued, square integrable i.i.d. R.V's
- Each with $\mathbf{E}[X_i] = \mu$ and $\mathbf{Var}[X_i] = v$

The strong law of large numbers tells us that

$$\frac{1}{n}X_n \xrightarrow[n\to\infty]{\quad a.s. \quad} E[X_n]$$

The CLT tells us $S_n^\star\\, \colon \\! = \frac{X_n-\mu}{\sqrt{v}} \xrightarrow[n\to\infty]{\quad d \quad} \mathcal{N}(0,1)$

<!--v-->

The aim of this paper is to discuss some statistical analogues for random dynamical systems. In contrast to deterministic dynamical systems, random dynamical systems permit the dynamical system to evolve in different ways according to certain probabilities. In particular, I will discuss a very specific model in subsection to analyse, with the goal of proving an analogue of the law of large numbers. This paper mostly follows [Kobre \& Young](https://doi.org/10.1007/s00220-007-0312-5).

<!--s-->

Let $\Sigma$ be a metric space equipped with its Borel measure,  
and let $\mathcal{F}$ be a finite family of continuous maps.  

We equip $\mathcal{F}$ with a probability measure denoted $P$.  
We call the pair $(\mathcal{F},P)$ a **random maps system**.  

For an infinite sequence $(f_i)_{i\in\mathbb{Z}^+}$ we define the composition  

$$f^{(n)}= f_{n-1}\circ\cdots f_{1}\circ f_0$$