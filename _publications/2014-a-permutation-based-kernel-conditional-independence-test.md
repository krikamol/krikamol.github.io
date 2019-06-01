---
layout: "paper"
title: "A Permutation-based Kernel Conditional Independence Test"
type: conference
venue: uai
year: "2014"
authors:
  - gary_doran
  - krikamol_muandet
  - kun_zhang
  - bernhard_schoelkopf
abstract: "Determining conditional independence (CI) relationships between random variables is a challenging but important task for problems such as
Bayesian network learning and causal discovery.
We propose a new kernel CI test that uses a single, learned permutation to convert the CI test
problem into an easier two-sample test problem.
The learned permutation leaves the joint distribution unchanged if and only if the null hypothesis of CI holds. Then, a kernel two-sample test,
which has been studied extensively in prior work,
can be applied to a permuted and an unpermuted
sample to test for CI. We demonstrate that the
test (1) easily allows the incorporation of prior
knowledge during the permutation step, (2) has
power competitive with state-of-the-art kernel CI
tests, and (3) accurately estimates the null distribution of the test statistic, even as the dimensionality of the conditioning variable grows."
---
