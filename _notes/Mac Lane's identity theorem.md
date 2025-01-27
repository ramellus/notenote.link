---
title: Mac Lane's identity theorem
tags: fact
toc: true
season: winter
---
## Statement
Suppose $(B,l)$ is a Cohen ring with two Cohen subrings $(A_1,k_1)$ and $(A_2,k_2)$. Fix a $p$-basis $\bar \beta \subseteq k_1$ with representatives $s: \bar \beta \to A_1$. If $k_1 \subseteq k_2$ and $s(\bar \beta) \subseteq A_2$, then $(A_1,k_1) \subseteq (A_2,k_2)$.

## Proof
We begin in characteristic $p^{m+1}$. Suppose $s_i: k_i^{p^m} \to A_i$ are the unique choices of $p^m$-representatives for $A_i$. Note that then, $A_1$ is generated by $s_1(k_1^{p^m}) \cup s(\bar \beta)$, and the latter is already in $A_2$, so we only need to check that $s_1(k_1^{p^m}) \subseteq A_2$. To do so, let $s_B: l^{p^m} \to B$ be the unique choice of $p^m$-representatives for $B$: then for any $\alpha \in k_i^{p^m} \subseteq l^{p^m}$, $s_B(\alpha)$ is the unique representative for $\alpha$; however, $s_i(\alpha)$ is also such a representative, hence $s_B(\alpha) = s_i(\alpha)$. In particular, $s_B$ extends both $s_1$ and $s_2$. In particular, all three must coincide on elements of $k_1^{p^m} \subseteq k_2^{p^m} \subseteq l^{p^m}$, so $s_2$ extends $s_1$ and thus $s_1(k_1^{p^m}) \subseteq s_2(k_1^{p^m}) \subseteq A_2$. Hence $A_1 \subseteq A_2$.
For the strict case, we have $A_1/(pA_1)^n \subseteq A_2/(pA_2)^n$ for any $n$, so by completeness $$A_1 = \lim_{\leftarrow} A_1/(pA_1)^n \subseteq \lim_{\leftarrow} A_2/(pA_2)^n = A_2.$$ $\square$
