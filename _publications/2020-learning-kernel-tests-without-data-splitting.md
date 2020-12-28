---
layout: "paper"
title: "Learning Kernel Tests Without Data Splitting"
type: conference
venue: neurips
year: "2020"
authors:
  - jonas_kuebler
  - wittawat_jitkrittum
  - bernhard_schoelkopf
  - krikamol_muandet
link: "https://papers.nips.cc/paper/2020/file/44f683a84163b3523afe57c2e008bc8c-Paper.pdf"
bibtex: "test"
poster: "test"
slide: "test"
code: "test"
video: "test"
abstract: "Modern large-scale kernel-based tests such as maximum mean discrepancy (MMD) and kernelized Stein discrepancy (KSD) optimize kernel hyperparameters on a held-out sample via data splitting to obtain the most powerful test statistics. While data splitting results in a tractable null distribution, it suffers from a reduction in test power due to smaller test sample size. Inspired by the selective inference framework, we propose an approach that enables learning the hyperparameters and testing on the full sample without data splitting. Our approach can correctly calibrate the test in the presence of such dependency, and yield a test threshold in closed form. At the same significance level, our approach’s test power is empirically larger than that of the data-splitting approach, regardless of its split proportion."
---
