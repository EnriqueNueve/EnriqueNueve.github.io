---
title: "Trading off Consistency and Dimensionality of Convex Surrogates for Multiclass Classification"
collection: publications
date: 2024-09-25
venue: 'NeurIPS 2024'
paperurl: 'https://openreview.net/pdf?id=xCIbVuXwPM'
author_list: Enrique Nueve, Bo Waggoner, Dhamma Kimpara, Jessie Finocchiaro
---

Abstract: In multiclass classification over $$n$$ outcomes, the outcomes must be embedded into the reals with dimension at least $$n−1$$ in order to design a consistent surrogate loss that leads to the "correct" classification, regardless of the data distribution. For large $$n$$, such as in information retrieval and structured prediction tasks, optimizing a surrogate in $$n−1$$ dimensions is often intractable. We investigate ways to trade off surrogate loss dimension, the number of problem instances, and restricting the region of consistency in the simplex for multiclass classification. Following past work, we examine an intuitive embedding procedure that maps outcomes into the vertices of convex polytopes in a low-dimensional surrogate space. We show that full-dimensional subsets of the simplex exist around each point mass distribution for which consistency holds, but also, with less than $$n−1$$ dimensions, there exist distributions for which a phenomenon called hallucination occurs, which is when the optimal report under the surrogate loss is an outcome with zero probability. Looking towards application, we derive a result to check if consistency holds under a given polytope embedding and low-noise assumption, providing insight into when to use a particular embedding. We provide examples of embedding $$n=2^d$$ outcomes into the d-dimensional unit cube and $$n=d!$$ outcomes into the d-dimensional permutahedron under low-noise assumptions. Finally, we demonstrate that with multiple problem instances, we can learn the mode with $$\frac{n}{2}$$ dimensions over the whole simplex

