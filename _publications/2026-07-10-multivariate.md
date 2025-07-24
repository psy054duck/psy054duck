---
title: "Verifying Recursions and Array Manipulating Programs in a Uniform Way by Solving Multivariate Recurrences"
collection: # conferences
category: conferences
permalink: /publication/2026-07-10-multivariate
authors: '<b>Chenglin Wang</b>'
# date: 2025-08-10
venue: 'Under review, submitted to POPL'
slidesurl: # 'http://academicpages.github.io/files/slides1.pdf'
paperurl: # 'http://academicpages.github.io/files/paper1.pdf'
citation: # 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
## Abstract

Both recursions and arrays are convenient tools for programmers to express complex algorithms.
However, they also pose challenges for program verification.
Like loops, recursions introduce unbounded execution paths,
which makes it difficult to reason about the correctness of programs.
Arrays with unbounded size are usually processed in a loop,
which introduces not only unbounded execution paths but also unbounded number of elements.
Addressing either of these challenges significantly impacts the verification of real-world programs.

The past years has seen significant advances in multi-path loop summarization
by treating them as conditional univariate recurrences.
Closed-form solutions to these recurrences are precise summaries to those loops.
However, these techniques are not directly applicable to recursions and array manipulating loops,
because recursions may have multiple input parameters and loops manipulating arrays correspond to multivariate recurrences.
In this paper, we present a novel approach to convert multivariate recurrences into univariate ones,
and then invoke existing recurrence solvers designed for univariate recurrences to solve them.
Closed-form solutions to these univariate recurrences are then translated back to obtain solutions to original multivariate recurrences.
The key insight is that although there may be multiple recursive calls in a recursive case,
there is a pivot call such that all other non-pivot calls in the same recursive case are computed as intermediate results during the computation of the pivot call.
This allows us to convert the original multivariate recurrence into a vectorized nearly tail recursion
by caching and returning these intermediate results,
which can be transformed into vectorized tail recursion and finally into univariate recurrences.

To show the effectiveness in program verification, we implemented a prototype verifier and compared it with other state-of-the-art verifiers.
We conducted experiments on a set of benchmarks from SV-COMP 2025,
and the results show that our tool is effective in proving recursions and programs that manipulate arrays,
and successfully verifies programs that all other tools fail to handle.