---
layout: "paper"
title: "AutoML Two-Sample Test"
type: conference
venue: neurips
year: "2022"
authors:
  - jonas_kuebler
  - vincent_stimper
  - simon_buchholz
  - krikamol_muandet
  - bernhard_schoelkopf
link: "https://arxiv.org/abs/2206.08843"
bibtex: ""
poster: "assets/pdf/posters/kuebler-aistats-2022-poster.pdf"
slide: "assets/pdf/slides/"
code: "https://github.com/jmkuebler/auto-tst"
video: "https://slideslive.com/38991136/automl-twosample-test"
abstract: "Two-sample tests are important in statistics and machine learning, both as tools for scientific discovery as well as to detect distribution shifts. This led to the development of many sophisticated test procedures going beyond the standard supervised learning frameworks, whose usage can require specialized knowledge about two-sample testing. We use a simple test that takes the mean discrepancy of a witness function as the test statistic and prove that minimizing a squared loss leads to a witness with optimal testing power. This allows us to leverage recent advancements in AutoML. Without any user input about the problems at hand, and using the same method for all our experiments, our AutoML two-sample test achieves competitive performance on a diverse distribution shift benchmark as well as on challenging two-sample testing problems.
We provide an implementation of the AutoML two-sample test in the Python package autotst."
---
