---
title: Existence and uniqueness of TF-lifts
tags: fact
toc: true
season: winter
---
## Existence
Given a [[Cohen ring]] $(A,k)$, a $p$-basis $\bar \beta \subseteq k$ and a choice of representatives $s: \bar \beta \to A$, there exists a Teichmüller-Frobenius lift of type $(s,\bar \beta)$.
## Proof of existence
Let $e: A \to W[k^{\mathrm{perf}}]$ be the embedding obtained via the [[Teichmüller's embedding process]]. Let $\phi = \mathrm{Frob} \circ e$, where $\mathrm{Frob}$ is the unique [[Lift of the Frobenius]] to the [[Witt vectors]].
Then $\phi$ is a [[Teichmüller-Frobenius lift]] of type $(s,\bar\beta)$. The only tricky part is the fact that $\phi(A) \subseteq A$: this follows from [[Mac Lane's identity theorem]], since $\phi(s(\bar\beta)) \subseteq A$. $\square$

## Uniqueness
Given a [[Cohen ring]] $(A,k)$, a $p$-basis $\bar \beta \subseteq k$ and a choice of representatives $s: \bar \beta \to A$, there is a unique Teichmüller-Frobenius lift of type $(s,\bar \beta)$.
## Proof of existence
Suppose $\phi$ is the lift obtained from the embedding, and let $\phi'$ be any other lift. Note that then, $\phi(s(b)) = \phi'(s(b))$ for every $b \in \bar\beta$. Now, working modulo $p^n$ we consider the induced morphisms $\phi_n,\phi_n': A/p^{n+1} \to A/p^{n+1}$. In particular, for every $a \in A$, we have that the class $[a]_n \in A/p^{n+1}$ can be represented as $[a]_n = \sum_{i=0}^{n} S_n(a_{i,n}) p^i$ for some $a_{i,n} \in k$, and we get
$$ \phi_n([a]_n) = \sum_{i=0}^{n} \phi_n(S_n(a_{i,n})) p^i.$$
Hence it is enough to show that, for any $a \in k$, $i$ and $n$, \[\phi_n(S_n(a)) = \phi_n'(S_n(a)).\]
Since $S_n(a) = \sum_{I} s_n(\lambda^I_{\bar\beta}(a)^{p^n}) s(\beta)^I$, where $s_n: k^{p^n} \to A/p^{n+1}$ are the unique $p^n$-representatives. Then,
$$\phi_n(S_n(a)) = \sum_I \phi_n(s_n(\lambda^I_{\bar\beta}(a)^{p^n})) \phi_n(s(\beta)^I) = \sum_I \phi_n(s_n(\lambda^I_{\bar\beta}(a)^{p^n})) \phi_n'(s(\beta)^I), $$
but now, taking the residues,
$$ \overline{\phi_n(s_n(\lambda^I_{\bar\beta}(a)^{p^n})} = \lambda^I_{\bar\beta}(a)^{p^{n+1}} = \overline{\phi_n'(s_n(\lambda^I_{\bar\beta}(a)^{p^n})},$$
meaning both $\phi_n(s_n(\lambda^I_{\bar\beta}(a)^{p^n})$ and $\phi_n'(s_n(\lambda^I_{\bar\beta}(a)^{p^n})$ are representatives of $\lambda^I_{\bar\beta}(a)^{p^{n+1}}$; however, there is only one such representative, namely $s_n( \lambda^I_{\bar\beta}(a)^{p^{n+1}})$, and hence they coincide. Back to our original setting, we now have for any $a \in A$,
$$ \phi(a) = \lim_{\longleftarrow} \phi_n([a]_n) = \lim_{\longleftarrow} \phi_n'([a]_n) = \phi'(a).$$