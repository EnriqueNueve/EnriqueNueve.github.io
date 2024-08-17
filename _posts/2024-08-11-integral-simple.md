---
title: "Integral of Simple Functions"
date: 2024-08-11
permalink: /posts/2024/08/IntegralofSimpleFunctions/
tags:
  - Real Analysis
---

This is week three of re-writing a proof from Axler's book Measure, Integration & Real Analysis by Sheldon Axler. The proof covered here demonstrates the closed form for integral of simple function. 


**Def. ($$\mathcal{S}$$-Partion)**: 
Suppose $$\mathcal{S}$$ is a $$\sigma$$-algebra on a set $$X$$.
An $$\mathcal{S}$$-partion of $$X$$ is a finite collection $$A_1,\dots ,A_m$$ of disjoint sets in $$\mathcal{S}$$ such that $$A_1 \cup\dots \cup A_m =X$$.

**Def. (Lower Lebesgue Sum)**: 
$$\mathcal{L}(f,P)=\sum_{j=1}^{m}\mu (A_j )\inf_{A_j}f$$

**Def. (Integral of a Nonnegative Function)**: 
$$ \int f d\mu = \sup \{ \mathcal{L}(f,P) : \; P \; \text{is a partion of } X \}=\sup_{A_j\in P} \sum_{j=1}^{m}\mu (A_j )\inf_{A_j} f$$

**Lemma 1**: Suppose $$(X,\mathcal{S},\mu )$$ is a measure space and 
$$D,E\in\mathcal{S}$$ are such that 
$$D\subseteq E$$.
Then $$\mu (E\setminus D)=\mu (E)-\mu (D)$$ provided that $$\mu (D)<\infty $$.

**Integral of a Characteristic Function**: Suppose $$(X,\mathcal{S},\mu )$$ is a measure space and $$E\in \mathcal{S}$$.
Then $$\int \chi_{E} d\mu =\mu (E)$$.

**Proof**: 
$$(\int \chi_{E}d\mu \geq \mu (E)): $$ 
say $$P$$ is a partion of $$X$$  with $$E$$ and its compliment 
$$E^{c}=X\setminus E$$.
Then 
$$\mathcal{L}(\chi_{E},\{ E,E^{c} \})=\mu (E)\cdot 1+\mu (E^c)\cdot 0 =\mu (E) $$.
Yet, whose to say $$P=\{ E,E^c \}$$ is the $$\sup_{P}\mathcal{L}(\chi_{E},P)$$ hence, 
$$(\int \chi_{E}d\mu \geq = \mathcal{L}(\chi_{E},\{E,E^c\}) = \mu (E))~. $$


$$(\int \chi_{E}d\mu \leq \mu (E)): $$ say $$P = \{ A_1,\dots ,A_m  \} $$ partions $$X$$.
Note, 
$$\mu (A_j)\inf_{A_j}\chi_{E} = \mu (A_j)\cdot 1$$ if 
$$A_j\subset E$$ by Def. $$\chi_{E}$$ and $$\mu (A_j)\cdot 0$$ otherwise.
Thus, 
<br>

$$\begin{equation}
\begin{split}
  \mathcal{L}(\chi_{E},P) & = \sum_{\{ j:A_j\subset E \}}\mu (A_j) &  \\
              & = \mu (\cup_{\{ j:A_j\subset E\}}A_j) & \quad  \text{Def. measure as}\; A_j \; \text{is disjoint} \\
              & \leq \mu (E) & \text{Lemma 1}, \cup_{\{ j:A_j\subset E \}} A_j \subseteq E 
\end{split} 
\end{equation}
$$
and therefore 
$$\int \chi_{E}d\mu \leq \mu (E) $$. $$\square$$

