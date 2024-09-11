---
title: "Query Answering with Guarded Existential Rules under Stable Model Semantics"
collection: # conferences
category: conferences
permalink: /publication/2019-10-01-Query-Answering
excerpt: 'Authors: Hai Wan; Guohui Xiao; <b>Chenglin Wang</b>; Xianqiao Liu; Junhong Chen; Zhe Wang'
date: 2020-04-03
venue: 'Proceedings of the AAAI Conference on Artificial Intelligence (AAAI)'
slidesurl: # 'http://academicpages.github.io/files/slides1.pdf'
paperurl: # 'http://academicpages.github.io/files/paper1.pdf'
citation: # 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
## Abstract

In this paper, we study the problem of query answering with guarded existential rules (also called GNTGDs) under stable model semantics. Our goal is to use existing answer set programming (ASP) solvers. However, ASP solvers handle only finitely-ground logic programs while the program translated from GNTGDs by Skolemization is not in general. To address this challenge, we introduce two novel notions of (1) guarded instantiation forest to describe the instantiation of GNTGDs and (2) prime block to characterize the repeated infinitely-ground program translated from GNTGDs. Using these notions, we prove that the ground termination problem for GNTGDs is decidable. We also devise an algorithm for query answering with GNTGDs using ASP solvers. We have implemented our approach in a prototype system. The evaluation over a set of benchmarks shows encouraging results.