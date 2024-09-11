---
title: "On Polynomial Expressions with C-Finite Recurrences in Loops with Nested Nondeterministic Branches"
collection: # conferences
category: conferences
permalink: /publication/2024-07-26-Polynomial
excerpt: 'Authors: <b>Chenglin Wang</b>; Fangzhen Lin'
date: 2024-07-26
venue: 'Computer Aided Verification (CAV)'
slidesurl: # 'http://academicpages.github.io/files/slides1.pdf'
paperurl: # 'http://academicpages.github.io/files/paper1.pdf'
citation: # 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
## Abstract

Loops are inductive constructs, which make them difficult to analyze and verify in general. One approach is to represent the inductive behaviors of the program variables in a loop by recurrences and try to solve them for closed-form solutions. These solutions can then be used to generate invariants or directly fed into an SMT-based verifier. One problem with this approach is that if a loop contains nondeterministic choices or complex operations such as non-linear assignments, then recurrences for program variables may not exist or may have no closed-form solutions. In such cases, an alternative is to generate recurrences for expressions, and there has been recent work along this line. In this paper, we further work in this direction and propose a template-based method for extracting polynomial expressions that satisfy some c-finite recurrences. While in general there are possibly infinitely many such polynomials for a given loop, we show that the desired polynomials form a finite union of vector spaces. We propose an algorithm for computing the bases of the vector spaces, and identify two cases where the bases can be computed efficiently. To demonstrate the usefulness of our results, we implemented a prototype system based on one of the special cases, and integrated it into an SMT-based verifier. Our experimental results show that the new verifier can now verify programs with non-linear properties.