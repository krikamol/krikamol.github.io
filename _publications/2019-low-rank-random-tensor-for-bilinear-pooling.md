---
layout: "paper"
title: "Low-rank Random Tensor for Bilinear Pooling"
type: preprint
venue: arxiv
year: 2019
authors:
  - yan_zhang
  - krikamol_muandet
  - qianli_ma
  - heiko_neumann
  - siyu_tang
abstract: "Bilinear pooling is capable of extracting high-order information
from data, which makes it suitable for fine-grained visual understanding and
information fusion. Despite their effectiveness in various applications, the
bilinear models with massive number of parameters can easily suffer from the
curse of dimensionality and intractable computation. In this paper, we propose
a novel bilinear model based on low-rank random tensors. The key idea is to
effectively combine low-rank tensor decomposition and random projection to reduce
the number of parameters while preserving the model representativeness. From the
theoretical perspective, we prove that our bilinear model with random tensors
can estimate feature maps to reproducing kernel Hilbert spaces (RKHSs) with
compositional kernels, grounding the high-dimensional feature fusion with theoretical
foundations. From the application perspective, our low-rank tensor operation is
lightweight, and can be integrated into standard neural network architectures to
enable high-order information fusion. We perform extensive experiments to show
that the use of our model leads to state-of-the-art performance on several
challenging fine-grained action parsing benchmarks."
---
