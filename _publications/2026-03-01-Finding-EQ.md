---
title: "An Efficient Method to Find Implied Equalities in Linear Real Arithmetic and Linear Integer Arithmetic"
collection: # conferences
category: conferences
permalink: /publication/2026-03-01-Finding-EQ
authors: 'Amir K. Goharshady, Pingjiang Li, <b>Chenglin Wang</b> (authors are ordered alphabetically)'
# date: 2025-08-10
venue: 'Under review'
slidesurl: # 'http://academicpages.github.io/files/slides1.pdf'
paperurl: # 'http://academicpages.github.io/files/paper1.pdf'
citation: # 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
## Abstract
Finding implied equalities plays an important role in formal verification.
SMT solvers based on Nelson-Oppen combination require their built-in theory solvers to be able to infer equalities between variables.
Finding equalities also provides a heuristic for fast quantifier elimination.
Many well-known quantifier elimination algorithms are computationally expensive and intractable in practice.
For instance, the Fourier-Motzkin algorithm exhibits doubly exponential complexity for linear real arithmetic (LRA), and Cooper’s method is triply exponential for linear integer arithmetic (LIA).
However, if the variable to be eliminated is involved in an implied equality, then it can be substituted away cheaply.
Previous works have shown that this problem can be solved in polynomial time by reducing it to linear programming problem.
However, we find that this approach is inefficient in practice.
In this work, we focus on the problem of efficiently detecting the set of equalities implied by a formula.
Specifically, we present a novel sound and complete algorithm for discovering \emph{all implied equalities} in LRA, running in \emph{polynomial time}.
By relaxing LIA formulas to LRA, our approach can also be soundly applied to integer variables.
Comparisons with other polynomial-time approaches on a wide range of benchmarks demonstrate that our method is significantly more efficient.
More concretely, the experimental results demonstrate that our algorithm is able to synthesize implied equalities in a wide variety of real-world inputs taken from SMT-COMP, including 65.42\% of the LRA benchmarks and 19.26\% of the LIA benchmarks.
We also compare our method with previous known algorithms and show that our method runs faster than other polynomial time algorithms.
Thus, it provides a highly effective heuristic that helps avoid expensive quantifier and variable elimination methods in a significant percentage of real-world scenarios.