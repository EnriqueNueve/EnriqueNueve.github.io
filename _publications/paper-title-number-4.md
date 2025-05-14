---
title: "Structured Prediction with Abstention via the Lovasz Hinge"
collection: publications
date: 2025-05-02
venue: 'In Review'
paperurl: 'https://arxiv.org/abs/2505.06446'
author_list: Jessie Finocchiaro, Rafael Frongillo, Enrique Nueve 
---

Abstract: The Lovász hinge is a convex loss function proposed for binary structured classification, in which k related binary predictions jointly evaluated by a submodular function. Despite its prevalence in image segmentation and related tasks, the consistency of the Lovász hinge has remained open. We show that the Lovász hinge is inconsistent with its desired target unless the set function used for evaluation is modular. Leveraging the embedding framework of Finocchiaro et al. (2024), we find the target loss for which the Lovász hinge is consistent. This target, which we call the structured abstain problem, is a variant of selective classification for structured prediction that allows one to abstain on any subset of the k binary predictions. We derive a family of link functions, each of which is simultaneously consistent for all polymatroids, a subset of submodular set functions. We then give sufficient conditions on the polymatroid for the structured abstain problem to be tightly embedded by the Lovász hinge, meaning no target prediction is redundant. We experimentally demonstrate the potential of the structured abstain problem for interpretability in structured classification tasks. Finally, for the multiclass setting, we show that one can combine the binary encoding construction of Ramaswamy et al. (2018) with our link construction to achieve an efficient consistent surrogate for a natural multiclass generalization of the structured abstain problem.