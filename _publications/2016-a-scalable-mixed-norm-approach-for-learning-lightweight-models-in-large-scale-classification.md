---
layout: "paper"
title: "TerseSVM : A Scalable Approach for Learning Compact Models in Large-scale Classification"
type: conference
venue: sdm
year: "2016"
authors:
  - krikamol_muandet
abstract: "For large-scale multi-class classification problems, consisting of tens of thousand target categories, recent works have emphasized the need to store billions of parameters. For instance, the classical l2-norm regularization employed by a state-of-the-art method results in the model size of 17GB for a training set whose size is only 129MB. To the contrary, by using a mixed-norm regularization approach, we show that around 99.5% of the stored parameters is dispensable noise. Using this strategy, we can extract the information relevant for classification, which is constituted in remaining 0.5% of the parameters, and hence demonstrate drastic reduction in model sizes. Furthermore, the proposed method leads to improvement in generalization performance compared to state-of-the-art methods, especially for under-represented categories. Lastly, our method enjoys easy parallelization, and scales well to tens of thousand target categories."
---
