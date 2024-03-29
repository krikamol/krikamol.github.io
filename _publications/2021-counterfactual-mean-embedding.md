---
layout: "paper"
title: "Counterfactual Mean Embeddings"
type: journal
venue: jmlr
year: "2021"
authors:
  - krikamol_muandet
  - motonobu_kanagawa
  - sorawit_saengkyongam
  - sanparith_marukatat
link: "https://jmlr.org/papers/v22/20-185.html"
bibtex: ""
poster: ""
slide: ""
code: "https://github.com/sorawitj/counterfactual-mean-embedding"
video: ""
abstract: "Counterfactual inference has become a ubiquitous tool in online advertisement, recommendation systems, medical diagnosis, and econometrics. Accurate modelling of outcome distributions associated with different interventions---known as counterfactual distributions---is crucial for the success of these applications. In this work, we propose to model counterfactual distributions using a novel Hilbert space representation called counterfactual mean embedding (CME). The CME embeds the associated counterfactual distribution into a reproducing kernel Hilbert space (RKHS) endowed with a positive definite kernel, which allows us to perform causal inference over the entire landscape of the counterfactual distribution. Based on this representation, we propose a distributional treatment effect (DTE) which can quantify the causal effect over entire outcome distributions. Our approach is nonparametric as the CME can be estimated under the unconfoundedness assumption from observational data without requiring any parametric assumption about the underlying distributions. We also establish a rate of convergence of the proposed estimator which depends on the smoothness of the conditional mean and the Radon-Nikodym derivative of the underlying marginal distributions. Furthermore, our framework allows for more complex outcomes such as images, sequences, and graphs. Our experimental results on synthetic data and off-policy evaluation tasks demonstrate the advantages of the proposed estimator."
---
