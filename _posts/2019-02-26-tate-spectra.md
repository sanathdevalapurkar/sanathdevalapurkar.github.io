---
layout: post
title:  "Tate spectra"
date:   2019-02-26
categories: algebraic-topology
---

<script type="text/javascript" async=""
src="https://www.google-analytics.com/analytics.js"></script>
<script async=""
src="https://www.googletagmanager.com/gtag/js?id=UA-109004213-1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());

        gtag('config', 'UA-109004213-1');
</script>
<script type="text/javascript"
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>

$$\newcommand{\KO}{\mathrm{KO}} \newcommand{\TMF}{\mathrm{TMF}}
\newcommand{\KU}{\mathrm{KU}} \newcommand{\Mfg}{M_\mathrm{fg}}
\newcommand{\spec}{\mathrm{Spec}\ } \newcommand{\dX}{\mathcal{X}}
\newcommand{\co}{\mathcal{O}} \newcommand{\Z}{\mathbf{Z}}
\newcommand{\top}{\mathrm{top}} \newcommand{\E}{\mathbf{E}}
\newcommand{\GG}{\mathbf{G}} \newcommand{\DD}{\mathbf{D}}
\newcommand{\Mell}{M_\mathrm{ell}} \newcommand{\ce}{\mathcal{E}}
\newcommand{\H}{\mathrm{H}} \newcommand{\dR}{\mathrm{dR}}
\newcommand{\cf}{\mathcal{F}} \newcommand{\FF}{\mathbf{F}}
\newcommand{\spf}{\mathrm{Spf}\ } \newcommand{\cA}{\mathcal{A}}
\newcommand{\Mcub}{M_\mathrm{cub}} \newcommand{\Mqd}{M_\mathrm{qd}}
\newcommand{\Aut}{\mathrm{Aut}} \newcommand{\tmf}{\mathrm{tmf}}
\newcommand{\Tmf}{\mathrm{Tmf}} \newcommand{\Map}{\mathrm{Map}}
\newcommand{\Ext}{\mathrm{Ext}} \newcommand{\End}{\mathrm{End}}
\newcommand{\cg}{\mathcal{G}} \newcommand{\Hom}{\mathrm{Hom}}
\newcommand{BP}[1]{\mathrm{BP}\langle #1\rangle} \newcommand{\QQ}{\mathbf{Q}}
\newcommand{\PP}{\mathbf{P}} \newcommand{\Gal}{\mathrm{Gal}}
\newcommand{\proj}{\mathrm{Proj}\ } \newcommand{\Ltwo}{L_{K(2)}}
\newcommand{\Eoo}{\mathbf{E}_\infty} \newcommand{\ol}[1]{\overline #1}
\newcommand{\pic}{\mathrm{Pic}} \newcommand{\d}{\mathrm{d}}
\newcommand{\F}{\mathrm{F}} \newcommand{\wt}[1]{\widetilde #1}
\newcommand{\AA}{\mathbf{A}} \newcommand{\PP}{\mathbf{P}}
\newcommand{\top}{\mathrm{top}} \newcommand{\der}{\mathrm{der}}
\newcommand{\M}{M} \newcommand{\colim}{\mathrm{colim}\ }
\newcommand{\GL}{\mathrm{GL}} \newcommand{\W}{\mathrm{W}}
\newcommand{\et}{\mathrm{et}} \newcommand{\im}{\mathrm{im}}
\newcommand{\tors}{\mathrm{tors}} \renewcommand{\div}{\mathrm{div}}
\newcommand{\Ln}{L_n}$$

Let $$\dX$$ be an even-periodic refinement of a Deligne-Mumford stack $$X$$
arising via [Lurie's theorem](/algebraic-geometry/2019/02/21/p-div-gps.html),
and assume that the map $$X\to \Mfg$$ is *affine*. Let $$\GG$$ denote the
associated [*oriented
spectral*](http://www.math.harvard.edu/~lurie/papers/Elliptic-II.pdf) (also see
[here](http://www.mit.edu/~sanathd/orientations.pdf)) $$p$$-divisible group
over $$\dX$$, with underlying $$p$$-divisible group $$G$$, say of height $$n$$
(so that $$\Gamma(\dX, \co_\dX)$$ is $$\Ln$$-local). A classical computation
shows that if $$\dX = \spf E$$, where $$E$$ is a height $$n$$ Morava
$$E$$-theory, then $$\pi_0(E^{B\Z/p^k_+}) = G[p^k]$$.

This is not true, however, if $$\dX = \spf L_{n-1} E$$. Indeed, in this case,
if $$A = \Z/p$$, then $$\spec \pi_0((L_{n-1} E)^{B\Z/p_+})$$ is the
$$p$$-torsion in the formal group $$G_{L_{n-1} E} = \spec \pi_0((L_{n-1}
E)^{\mathbf{C}P^\infty_+})$$ associated to $$L_{n-1} E$$. The height $$n-1$$
formal group $$H_{L_{n-1} E}$$ is actually the formal component of the
$$p$$-divisible group $$G_{L_{n-1} E} = \spec \pi_0
L_{n-1}(E^{B\Z/p^\infty_+})$$ of height $$n$$; this is defined via the
canonical map $$L_{n-1}(E^{B\Z/p^\infty_+}) \to (L_{n-1} E)^{B\Z/p^\infty_+}$$.
Note that $$\GG_{L_{n-1} E}$$ is precisely the restriction of $$\GG_E$$ to the
locus $$\spec \pi_0 L_{n-1} E \subseteq \spec \pi_0 E$$.

In general, if $$\dX$$ is as above, let $$A = \Gamma(\dX, \co_\dX)$$. Then
there is a map $$\Gamma(\GG[p^k], \co_{\GG[p^k]}) \to A^{B\Z/p^k_+}$$. Let
$$\{e\}$$ denote the origin of $$G[p^k]$$, defined coordinate-independently as
follows: there is a quotient map $$\Z/p^k \to \ast$$, and this induces a closed
immersion $$\{e\} \hookrightarrow G[p^k]$$. Let $$\GG[p^k]\setminus \{e\}$$
denote the canonical even-periodic refinement of the associated open subscheme
(really, substack) of $$\GG[p^k]$$. There is an analogous construction one can
do for $$A^{B\Z/p^k_+}$$: let $$\rho$$ denote the $$1$$-dimensional complex
($$2$$-dimensional real) representation of $$\Z/p^k$$ given by the inclusion of
the $$p^k$$th roots of unity. Then the inclusion $$0\hookrightarrow \rho$$
defines a map $$e_\rho:S^0 \to S^\rho$$, which in turn defines a map
$$e_\rho^N:A^{h\Z/p^k} = A^{B\Z/p^k_+} \to (\Sigma^{N\rho} A)^{h\Z/p^k}$$. We
then have the following lemma, whose proof we shall postpone.

**Lemma:** For some $$N\gg 0$$, there is an *equivariant* identification
$$\Sigma^{N\rho} A \simeq \Sigma^{2N} A$$ of $$A$$-modules.

The $$\Eoo$$-ring $$A$$ necessarily has some even period (which can be proved
by arguing exactly as in our proof of the above lemma (to be given below); some
power of the periodicity generator in $$\H^0(X;\pi_2 \co_\dX)$$ identifying
$$\Sigma^2 \co_\dX \simeq \co_\dX$$ survives the descent spectral sequence), so
we can then choose $$N$$ large enough such that $$\Sigma^{2N} A \simeq A$$; in
this case, $$e_\rho^N$$ defines a map $$A^{h\Z/p^k} \to A^{h\Z/p^k}$$. Let
$$A^{h\Z/p^k}[e_\rho^{-1}]$$ denote the colimit; then, it is known that
$$A^{h\Z/p^k}[e_\rho^{-1}]$$ is equivalent to the Tate construction
$$A^{t\Z/p^k}$$. The discussion above implies that the map $$\Gamma(\GG[p^k],
\co_{\GG[p^k]}) \to A^{B\Z/p^k_+}$$ restricts to a map
$$\Gamma(\GG[p^k]\setminus\{e\}, \co_{\GG[p^k]\setminus\{e\}}) \to
A^{t\Z/p^k}$$.

We then have the following blueshift phenomenon; see also Theorem 3.4
[here](http://www.ms.uky.edu/~njst237/papers/sixauthors.pdf) for the local case
of Lubin-Tate theory with $$\Z/p^k$$ replaced by a general finite abelian
$$p$$-group and the Tate construction replaced by the geometric fixed points
construction:

**Theorem:** The maximum height of the formal component of the $$p$$-divisible
group over every geometric point of $$G[p^k]\setminus\{e\}$$ is at most
$$n-1$$; in other words, the canonical map $$G[p^k]\setminus\{e\}\to \Mfg^{\leq
n}$$ factors through $$\Mfg^{\leq n-1} \to \Mfg^{\leq n}$$.

This implies that $$\Gamma(\GG[p^k]\setminus\{e\},
\co_{\GG[p^k]\setminus\{e\}})$$ is $$L_{n-1}$$-local; because of the ring map
$$\Gamma(\GG[p^k]\setminus\{e\}, \co_{\GG[p^k]\setminus\{e\}}) \to
A^{t\Z/p^k}$$, we conclude that $$A^{t\Z/p^k}$$ is also $$L_{n-1}$$-local.

Here's the proof of the theorem. For every field $$L$$, we know that
$$G[p^k](L) \cong (\Z/p^k)^{n-t}$$, where $$t$$ is the height of the formal
component of $$G_L$$. It follows that the maximum height of the formal
component of the $$p$$-divisible group over every geometric point of
$$G[p^k]\setminus\{e\}$$ is the largest integer $$t\geq 0$$ for which there is
a *nontrivial* homomorphism $$f:\Z/p^k \to (\Z/p^k)^{n-t} \cong G[p^k](L)$$.
(One could see this as the statement that an $$R$$-point of $$G[p^k]$$ is the
data of a $$p$$-divisible group over $$R$$ isomorphic to the pullback of $$G$$
to $$R$$, along with a $$p^k$$-torsion point, possibly zero.  Removing the
identity of $$G[p^k]$$ precisely excludes this degeneracy.) Clearly $$n-1$$ is
the largest such integer, so we win.

What can we do with our understanding of $$\GG[p^k]\setminus\{e\}$$? Above, we
constructed a map $$\Gamma(\GG[p]\setminus\{e\}, \co_{\GG[p]\setminus\{e\}})
\to A^{tC_p}$$. The target may be thought of as a natural target of cohomology
operations. Namely, we have a map $$\pi_0 A \to A^0(B\Sigma_p) \to
A^0(B\Sigma_p)/I$$, where $$I$$ is the transfer ideal; this map is the total
power operation. Now, $$A^0(B\Sigma_p) \simeq \pi_0 A^{h\Sigma_p}$$, and there
is a natural map to $$A^{hC_p}$$, which in turn maps to $$A^{tC_p}$$. The map
t; this map is the total power operation. Now, $$A^0(B\Sigma_p) \simeq \pi_0
A^{h\Sigma_p}$$, and there is a natural map to $$A^{hC_p}$$, which in turn maps
to $$A^{tC_p}$$. The map to $$\pi_0 A^{tC_p}$$ factors through the quotient
$$A^0(B\Sigma_p)/I$$, because, in a sense, $$A^{tC_p}$$ is the homotopical
version of this quotient. The upshot is that we obtain a map $$\pi_0 A \to
A^0(B\Sigma_p)/I \to \pi_0 A^{tC_p}$$.

There is also a map of $$\Eoo$$-ring spectra $$A\to A^{tC_p}$$; this is called
the *Tate-valued Frobenius*. This map is discussed in great detail in [this
paper](https://arxiv.org/pdf/1707.01799.pdf). The above discussion then
suggests that there is a map $$A\to \Gamma(\GG[p]\setminus\{e\},
\co_{\GG[p]\setminus\{e\}})$$ of $$\Eoo$$-rings factoring the Tate-valued
Frobenius. Since $$A = \Gamma(\dX)$$, it is most natural to expect that this
comes from a morphism $$\GG[p] \setminus \{e\} \to \dX$$. I haven't yet gotten
around to precisely defining this map, but it is supposed to be analogous to
the morphism $$X\times_{M_p(n)} M_p(n)_{\Gamma_1(p)} \to X$$ that is the
pullback of the morphism $$M_p(n)_{\Gamma_1(p)} \to M_p(n)$$ that sends
$$(G,P)$$ to $$G/\langle P \rangle$$. The desired map $$\GG[p] \setminus \{e\}
\to \dX$$ is a bit mysterious: it's definitely *not* going to be a spectral
lift of the map $$X\times_{M_p(n)} M_p(n)_{\Gamma_1(p)} \to X$$: the main
theorems of [this paper of
mine](http://www.mit.edu/~sanathd/roots-of-unity.pdf) forbid the source from
being lifted to the world of $$\Eoo$$-rings.

Instead, (I believe that) the derived stack $$\GG[p]$$ classifies a
*different*, but related, moduli problem. Recall that the classical stack
$$G[p]$$ classifies the following moduli problem: a map $$S \to G[p]$$ is the
data of a $$p$$-torsion point on the $$p$$-divisible group defined by the
pullback of $$G$$ to $$S$$ along the map $$S \to G[p] \to X$$. In the spectral
setting, a morphism $$S\to \GG[p]$$ (now from a derived scheme $$S$$) certainly
still defines a spectral $$p$$-divisible group $$\GG'$$ over $$S$$ via the
pullback of $$\GG$$ along the map $$S\to \GG[p] \to \dX$$, but what is the
appropriate notion of a $$p$$-torsion point on $$\GG'$$? Let us consider the
case when both $$S$$ and $$X = \spec A$$ are actually affine, so that $$\GG'$$
is an affine group scheme $$\spec B$$ over $$\spec A$$. Presumably the derived
stack $$\GG[p]$$ classifies a "$$p$$-torsion point" on $$\GG'$$. This would be
a map of constant group schemes $$\underline{\Z/p} \to \GG'$$. In particular,
we have a $$p$$-torsion element of the underlying $$p$$-divisible group $$G'$$
over the underlying scheme of $$S$$.

In general, if $$R$$ is an $$\Eoo$$-ring and $$x$$ is a strictly commutative
element of $$R$$, i.e., an element of $$\pi_0 R$$ such that the map
$$S^0\{t\}\to R$$ detecting $$x$$ factors through $$S[t] = \Sigma^\infty_+
\Z_{\geq 0}$$, we may take the quotient $$R/x$$, and this is an $$\Eoo$$-ring.
Indeed, since there is a fiber sequence $$S[t] \xrightarrow{t} S[t] \to S^0$$,
we get an equivalence $$R/x\simeq R\otimes_{S[t]} S^0$$. In particular, if
$$I$$ is a finitely generated ideal of $$\pi_0(R)$$ generated by strictly
commutative elements, then $$\spec(R/I)$$ is a closed subscheme of $$\spec R$$.
Weil divisors on Noetherian schemes whose associated ideal sheaves are
generated by strictly commutative elements therefore give closed subschemes of
$$\spec R$$ that deserve to be called Weil divisors of $$\spec R$$. In
particular, given a strict $$p$$-torsion point $$Q$$ on $$\GG'$$ defined by a
morphism $$\underline{\Z/p} \to \GG'$$, we can form the closed subscheme
$$\langle Q\rangle$$ of $$\GG'$$ as the Weil divisor in $$\GG'$$ defined as the
Weil divisor associated to the morphism $$\underline{\Z/p} \to G'$$ of ordinary
group schemes. Using this, one should be able to define the map
$$\GG[p]\setminus\{e\} \to \dX$$ as a map of moduli problems. I haven't had the
time to work this out precisely, but I think the story should work out
similarly to the classical theory.

---

We now prove the lemma we left unproved way back in the beginning of the post.
Let $$B$$ denote the global sections of some etale cover of $$\dX$$, so that
$$B$$ is even-periodic. Then it is classical that $$\Sigma^\rho B \simeq
\Sigma^2 B$$, so by descent, it suffices to construct a map $$\Sigma^{2N} A \to
\Sigma^{N\rho} A$$ of $$A$$-modules which is an equivalence after inducing up
to $$B$$. This is the same as an element of $$\pi_{(2-\rho)N} A$$ which maps to
the obvious class in $$\pi_{(2-\rho)N} B$$.

We know (because it is true after pulling back via every affine etale
morphism) that there is an equivalence of sheaves $$\Sigma^2 \co_\dX \simeq
\Sigma^\rho \co_\dX$$. This defines a section $$\wt{e}_\rho$$ of the homotopy
sheaf $$\pi_{2-\rho} \co_\dX$$. Using the Bousfield-Kan spectral sequence, one
can construct the following analogue of the descent spectral sequence for
$$RO$$-graded homotopy groups (where the action is trivial; the construction
becomes more complicated when a nontrivial action is involved):

$$E_2^{s,V} = \H^s(X; \pi_V \co_\dX) \Rightarrow \pi_{V-s} A,$$

where $$\pi_V \co_\dX$$ is the sheaf $$U\mapsto \pi_V(\co_\dX(U))$$ on
$$\mathrm{Aff}^\mathrm{et}_{/X}$$ and $$V\in \mathrm{RO}(\Z/p^k)$$. We have an
element $$\wt{e}_\rho\in E_2^{s,2-\rho}$$; we claim that there is some $$N\gg
0$$ for which $$\wt{e}_\rho^N$$ survives to the $$\Eoo$$-page of this spectral
sequence; then, $$\wt{e}_\rho^N$$ defines an element of $$\pi_{(2-\rho)N} A$$
that by construction maps to the obvious element of $$\pi_{(2-\rho)N} B$$, as
desired.

Suppose that $$E_2^{s,V}$$ is torsion for $$s\geq 1$$. Then
$$d_2(\wt{e}_\rho)$$ is $$k$$-torsion for some $$k$$, so by the Leibniz rule,
$$\wt{e}_\rho^k$$ survives to the $$E_3$$-page. Arguing similarly, we conclude
that for each $$r$$, some power of $$\wt{e}_\rho$$ survives to the
$$E_r$$-page. To conclude, it suffices to show that $$E_r^{s,V}$$ degenerates
at a finite page. This is true by thick subcategory arguments: by tameness of
the map $$X\to \Mfg$$, the stack $$X\times_{\Mfg} \spec \pi_0 E$$ (which has an
even-periodic refinement to $$\dX \times_{\spec S} \spec E$$) is tame, and
hence has finite cohomological dimension. Therefore, the spectral sequence for
$$\dX \times_{\spec S} \spec E$$ already degenerates a finite page. By the
Hopkins-Ravenel smash product theorem, $$A$$ is in the thick tensor ideal
generated by $$\Gamma(\dX \times_{\spec S} \spec E) = A\wedge E$$; therefore,
we conclude that the spectral sequence $$E_2^{s,V}$$ for $$A$$ degenerates at a
finite page.

It therefore remains to show that $$E_2^{s,V}$$ is torsion for $$s\geq 1$$.
The map $$X\to \Mfg$$ is affine, so the map $$X_\QQ \to (\Mfg)_\QQ = B\GG_m$$
is also affine. It follows that $$X_\QQ$$ is the quotient of an affine scheme
by $$\GG_m$$, which proves that $$X_\QQ$$ has no higher sheaf cohomology; in
particular, $$E_2^{s,V}$$ must be torsion for $$s\geq 1$$, and we win.
