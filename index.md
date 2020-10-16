## Welcome to MLDiag Page

An effective machine learing model diagnosing tool

### Introduction

Testing machine learning models is usually limited to some actions, mainly:

- algorithmic performances (metrics) of the model over a validation set (accuracy, precision, recall, etc.),
- computational performances of the model (speed, memory, etc.)
- examples where the model was most confidently incorrect

Decision made to promote a model into production is usually based on theses observations::

- is the current model offering an improvement over the existing version when evaluated on the same dataset.
- is the current model reaching the business required performance.

The model that fulfill this checklist is saved, along with hyperparamters and dataset that were used to validate the model, using MLFlow for instance. However, this traditional model checking lacks many important features:

- where the model does usually fail, and how to fix it?
- does the model generalize well on some variations over the evaluation set?
- how to track (and prevent) behavioral regressions for specific failure modes that had been previously addressed? Indeed, you might improve the overall evaluation metric but introduce a regression on a critical subset of data. Or you could unknowingly add a gender bias to the model through the inclusion of a new dataset during training.
- how can we define the best directions for model future improvement researcher usually look at a small set of incorrect predicted data to understand model failure. Such approach is biased since small samples are likely unrepresentative of the true error distribution. A more precise, reproducible, scalable, and testable procedure is required.

The checklist could be larger, but work is usually made manually.

MLDiag is a simple, yet effective framework, to handle model evaluation automatically. It provides at the end of the evaluation a comprehensive report on model robustness to adversarial attacks and simple tracks to improve its performances.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
