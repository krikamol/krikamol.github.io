---
layout: "paper"
title: "Gated Domain Units for Multi-source Domain Generalization"
type: preprint
venue: arxiv
year: "2023"
authors:
  - simon_foell
  - alina_dubatovka
  - eugen_ernst
  - martin_maritsch
  - patrik_okanovic
  - gudrun_thaeter
  - joachim_buhmann
  - felix_wortmann
  - krikamol_muandet
link: ""
bibtex: ""
poster: ""
slide: ""
code: ""
video: ""
abstract: "Distribution shift (DS) is a common problem that deteriorates the performance of learning machines. To tackle this problem, we postulate that real-world distributions are composed of elementary distributions that remain invariant across different domains, which we call an invariant elementary distribution (I.E.D.) assumption. We show that the I.E.D. assumption on the distribution space implies an invariant structure in the solution space that enables knowledge transfer to unseen domains. To exploit this property in domain generalization (DG), we developed a modular neural network layer that consists of Gated Domain Units (GDUs). Each GDU learns an embedding of an individual elementary distribution that allows us to encode the domain similarities during the training. During inference, the GDUs compute similarities between an observation and each of the corresponding elementary distributions which are then used to form a weighted ensemble of learning machines. Our extensive evaluation on image, text, and graph data shows a consistent improvement in the performance on out-of-training target domains without domain information and any access to data from the target domains. This finding supports the practicality of the I.E.D. assumption as well as the technical instantiation in the form of GDUs."
---
