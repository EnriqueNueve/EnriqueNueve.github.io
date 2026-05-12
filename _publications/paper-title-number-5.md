---
title: "Adaptive Liquidity in Prediction Markets via Online Learning"
collection: publications
date: 2026-05-12
venue: 'In Review'
paperurl: 'https://arxiv.org/abs/2605.09599'
author_list: Enrique Nueve, Bao Nguyen, Rafael Frongillo, Bo Waggoner
---

Abstract: Prediction markets rely on liquidity to convert trades into informative prices, yet existing mechanisms fix liquidity ex ante. This restriction enforces a static trade-off between price responsiveness and worst-case loss despite inherently nonstationary trading conditions. We propose a fundamentally different approach that treats liquidity selection itself as an online learning problem. Our mechanism mixes a family of cost-function markets via learnable weights, yielding a single adaptive market that preserves no-arbitrage, bounded worst-case loss, expressiveness, and positive upside. We introduce a hybrid structural risk signal, a per-round objective that quantifies the trade-off between price impact and inventory risk, and show that standard online learning algorithms achieve switching-regret guarantees relative to the best sequence of liquidity regimes in hindsight. Simulations demonstrate that the mechanism adaptively shifts liquidity across regimes in response to both order flow and inventory dynamics. Our results establish a principled framework for adaptive liquidity, connecting prediction market design with online learning.