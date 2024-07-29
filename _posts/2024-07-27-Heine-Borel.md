---
title: 'Heine-Borel Theorem'
date: 2024-07-27
permalink: /posts/2024/07/Heine-Borel/
tags:
  - Real Analysis
---

**Heine-Borel Theorem**: every open cover $$\mathcal{C}$$ of a closed bounded subset $$F$$ of $$\mathbb{R}$$ has a finite subcover. 

**Proof**: To begin we consider the case $$F=[a,b]$$ such that $$a,b\in\mathbb{R}$$ and $$a<b$$. Let $$D=\{d\in [a,b] \mid [a,d]\; \text{has a finite subcover from }\mathcal{C}  \}$$. To prove there exists a finite subcover from $$\mathcal{C}$$ over $$F$$, we will show that $$b\in D$$. Outlining the proof, we first show that $$\sup D$$ exists and $$\sup D\in D$$. Hence, by the definition of $$D$$, a finite subcover over $$[a,\sup D]\subseteq [a,b]$$ exists. Finally, we show that $$\sup D = b$$, completing the proof.


$$(D\neq \emptyset )$$:
<br>


$$(\sup D\in [a,b] )$$
<br>

$$(b=\sup D \; \& \; b\in D )$$
<br>

