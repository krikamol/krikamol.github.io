---
layout: "paper"
title: "Proximal Causal Learning with Kernels: Two-Stage Estimation and Moment Restriction"
type: conference
venue: AISTATS
year: "2022"
authors:
  - jonas_kuebler
  - wittawat_jitkrittum
  - bernhard_schoelkopf
  - krikamol_muandet
link: ""
bibtex: ""
poster: ""
slide: ""
code: ""
video: ""
abstract: "The Maximum Mean Discrepancy (MMD) has been the state-of-the-art nonparametric test for tackling the two-sample problem. Its statistic is given by the difference in expectations of the witness function, a real-valued function defined as a weighted sum of kernel evaluations on a set of basis points. Typically the kernel is optimized on a training set, and hypothesis testing is performed on a separate test set to avoid overfitting (i.e., control type-I error). That is, the test set is used to simultaneously estimate the expectations and define the basis points, while the training set only serves to select the kernel and is discarded. In this work, we propose to use the training data to also define the weights and the basis points for better data efficiency. We show that 1) the new test is consistent and has a well-controlled type-I error; 2) the optimal witness function is given by a precision-weighted mean in the reproducing kernel Hilbert space associated with the kernel; and 3) the test power of the proposed test is comparable or exceeds that of the MMD and other modern tests, as verified empirically on challenging synthetic and real problems (e.g., Higgs data)."
---
