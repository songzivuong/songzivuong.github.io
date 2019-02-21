---
layout: post
title: "Read What Is Mathematics? by Courant"
categories: Mathematics Reading
tags: courant mathematics
math: true
---

[*What Is Mathematics? An Elementary Approach to Ideas and Methods*, 2nd Edition](https://www.amazon.com/dp/0195105192) (Richard Courant, Herbert Robbins and Ian Stewart. 1996).

{% include toc.html %}

## Chapter 1. The Natural Numbers

### The Mathematical Induction

Suppose there is an infinite sequence of statements $A_{1},A_{2},\dots$. The mathematical induction is a principle that can let us to examine whether all these statements are true or false. 

1. If $A_1$ is true;
2. If supposing $A_k$ is true can derive that $A_{k+1}$ is true.

Then we can conclude that for all $n$, $A_n$ is true.

Example: some formulas that can be proved by the mathematical induction:

- $1+2+\cdots+n=\frac{n(n+1)}{2}$
- $1+q+\cdots+q^n=\frac{1-q^{n+1}}{1-q}$
- $1^2+2^2+\cdots+n^2=\frac{n(n+1)(2n+1)}{6}$
- $1^3+2^3+\cdots+n^3=(\frac{n(n+1)}{2})^2$

The mathematical induction can only help us to *test and verify a hypothesis*, but it can not tell us how the hypothesis come out. Mathematical hypothesis needs other kinds of talent: **experiment**, **analogy**, and **constructive intuition**.

### An Important Inequality

For every number $p > -1$ and every positive integer $n$, we have

$$
(1+p)^n \geq 1+np
$$

Again, we can use the mathematical induction to verify this formula.

1. For $n=1$, the two sides are equal.
2. Suppose $(1+p)^n \geq 1+np$ is true, then

    $$
    (1+p)^{n+1}=(1+p)^{n}(1+p)
    $$

    Because $1+p>0$, then

    $$
    \begin{align}
    (1+p)^{n+1} &= (1+p)^{n}(1+p) \\
    &\geq (1+np)(1+p) \\
    &= 1+(n+1)p+np^2 \\
    &\geq 1+(n+1)p \\
    \end{align}
    $$

### The Binomial Theorem

For $n\geq1$,

$$
(a+b)^n=a^n+C_{1}^{n}a^{n-1}b+C_{2}^{n}a^{n-2}b^{2}+\cdots+C_{n-1}^{n}ab^{n-1}+b^n
$$

where $C_{i}^{n}=\frac{n!}{i!(n-i)!}$