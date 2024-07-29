---
title: 'Heine-Borel Theorem'
date: 2024-07-27
permalink: /posts/2024/07/Heine-Borel/
tags:
  - Real Analysis
---

For fun and to improve my proof-writing, I am working through the book Measure, Integration & Real Analysis by Sheldon Axler. Each week (as of 7/27/24), I plan to write a blog post re-writing a proof from Axler's book.


**Open Cover**: Let $$A\subset \mathbb{R}$$. A collection $$\mathcal{C}$$ of open subsets of $$\mathbb{R}$$ is called an open cover of $$A$$ if $$A$$ is contained in the union of all the sets in $$\mathcal{C}$$.

**Heine-Borel Theorem**: every open cover $$\mathcal{C}$$ of a closed bounded subset $$F$$ of $$\mathbb{R}$$ has a finite subcover. 

**Proof**: To begin we consider the case $$F=[a,b]$$ such that $$a,b\in\mathbb{R}$$ and $$a<b$$. Let $$D=\{d\in [a,b] \mid [a,d]\; \text{has a finite subcover from }\mathcal{C}  \}$$. To prove there exists a finite subcover from $$\mathcal{C}$$ over $$F$$, we will show that $$b\in D$$. Outlining the proof, we first show that $$\sup D$$ exists and $$\sup D\in D$$. Hence, by the definition of $$D$$, a finite subcover over $$[a,\sup D]$$ exists. Finally, we show that $$\sup D = b$$, completing the proof.


$$(D\neq \emptyset )$$: Since $$\mathcal{C}$$ is an open cover on $$F$$, there exists an open set $$G\in\mathcal{C}$$ such that $$a\in G$$ and thus $$[a,a]\in D$$. Therefore $$D\neq \emptyset$$.
<br>


$$(\sup D\in [a,b] )$$: Let $$s=\sup D$$. Since $$D\subseteq [a,b]$$, a closed set, $$s\in [a,b]$$.
<br>

$$(b=\sup D \; \& \; b\in D )$$: By $$\mathcal{C}$$ being an open cover on $$F$$, there exists $$G'\in \mathcal{C}$$ such that $$s\in G'$$. By $$G'$$ being an open set, there exists a $$\delta >0$$ such that $$(s-\delta ,s+\delta )\subset G'$$. Since $$s\in D\subseteq [a,b]$$, there exists $$d'\in (s-\delta ,s)$$ and a finite open cover $$G_1\dots G_n$$ such that $$[a,d']\subseteq G_1\cup \dots \cup G_n$$. Observer for all $$d''\in [s,s+\delta)$$ it hold that $$[a,d'']\subseteq G'\cup G_1\cup \dots \cup G_n$$. Therefore, for any $$\hat{d}\in [s,s+\delta )\cap [a,b]$$ it holds that $$\hat{d}\in D$$. <br>
We claim that $$b=s$$. If $$b\neq s$$ then some element of $$[s,s+\delta )$$ would be greater than $$\sup D$$ forming a contradiction. Hence, $$b\in [b,b+\delta )\cap [a,b]$$ meaning $$b\in D$$.
<br>

We now cover the general case for a closed bounded subset $$F$$ of $$\mathbb{R}$$ with an open cover $$\mathcal{C}$$. Pick $$a',b'\in \mathbb{R}$$ such that $$F\subset [a',b']$$. Note $$\mathcal{C}\cup \{\mathbb{R}\setminus F \}$$ is an open cover of $$\mathbb{R}$$ ane hence $$[a',b']$$. By our first proven case, there exists $$G_1\dots G_n\in\mathcal{C}$$ such that $$[a',b']\subset G_1\cup\dots \cup G_n\cup (\mathbb{R}\setminus F)$$. Since $$F\subset [a',b']$$ and $$F\cap (\mathbb{R}\setminus F)=\emptyset$$, it implies that $$F\subset G_1\cup\dots \cup G_n$$. $$\square$$

