---
layout: post
title:  "How to prove the nilpotence theorem"
date:   2020-04-04
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
\newcommand{\spec}{\mathrm{Spec}} \newcommand{\dX}{\mathcal{X}}
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
\newcommand{\pic}{\mathrm{Pic}} \newcommand{\RP}{\mathbf{R}P}
\newcommand{\BO}{\mathrm{BO}} \newcommand{\cc}{\mathbf{C}}
\newcommand{\CP}{\mathbf{C}P} \newcommand{\wt}[1]{\widetilde #1}
\newcommand{\RR}{\mathbf{R}} \renewcommand{\S}{\mathbb{S}}
\newcommand{\Lone}{L_{K(1)}} \newcommand{\Ltwo}{L_{K(2)}}
\newcommand{\gl}{\mathrm{gl}} \newcommand{\Lk}{L_{K(n)}}
\newcommand{\ku}{\mathrm{ku}} \newcommand{\ko}{\mathrm{ko}}
\newcommand{\GL}{\mathrm{GL}} \newcommand{\Ln}{L_n} \newcommand{\Lt}{L_{K(t)}}
\newcommand{\W}{\mathrm{W}} \newcommand{\BU}{\mathrm{BU}}
\newcommand{\SU}{\mathrm{SU}} \newcommand{\MU}{\mathrm{MU}}
\newcommand{\ul}[1]{\underline #1} \newcommand{\Sq}{\mathrm{Sq}}
\newcommand{\Tr}{\mathrm{Tr}} \newcommand{\d}{\mathrm{d}}
\newcommand{\HP}{\mathbf{H}P} \newcommand{\cL}{\mathcal{L}}
\newcommand{\cs}{\mathrm{cs}} \newcommand{\cd}{\mathcal{D}}
\newcommand{\Bord}{\mathrm{Bord}} \newcommand{\SO}{\mathrm{SO}}
\newcommand{\cC}{\mathcal{C}} \newcommand{\Sp}{\mathrm{Sp}}
\newcommand{\Lkd}{L_{K(d)}} \newcommand{\Mod}{\mathrm{Mod}}
\newcommand{\cH}{\mathcal{H}} \newcommand{\ket}[1]{|#1 \rangle}
\newcommand{\Bun}{\mathrm{Bun}} \newcommand{\cM}{\mathcal{M}}
\newcommand{\MTH}{\mathrm{MT}H} \newcommand{\MSO}{\mathrm{MSO}}
\newcommand{\twsm}{\ \widetilde{\wedge} \ } \newcommand{\BSpin}{\mathrm{BSpin}}
\newcommand{\MSpin}{\mathrm{MSpin}} \newcommand{\BString}{\mathrm{BString}}
\newcommand{\MString}{\mathrm{MString}} \newcommand{\B}{\mathrm{B}}
\newcommand{\der}{\mathrm{der}} \newcommand{\Cat}{\mathrm{Cat}}
\newcommand{\QCoh}{\mathrm{QCoh}} \newcommand{\LMod}{\mathrm{LMod}}
\newcommand{\Rep}{\mathrm{Rep}} \newcommand{\HH}{\mathrm{HH}}
\newcommand{\ZZ}{\mathfrak{Z}} \newcommand{\fr}{\mathrm{fr}}
\newcommand{\BSO}{\mathrm{BSO}} \newcommand{\BSU}{\mathrm{BSU}}
\newcommand{\id}{\mathrm{id}} \newcommand{\Top}{\mathrm{Top}}
\newcommand{\cP}{\mathcal{P}} \newcommand{\U}{\mathrm{U}}
\newcommand{\Sym}{\mathrm{Sym}} \newcommand{\coker}{\mathrm{coker}}
\newcommand{\Vect}{\mathrm{Vect}} \newcommand{\Fun}{\mathrm{Fun}}
\newcommand{\cT}{\mathcal{T}} \newcommand{\cJ}{\mathcal{J}}
\newcommand{\Res}{\mathrm{Res}} \newcommand{\Ind}{\mathrm{Ind}}
\newcommand{\MO}{\mathrm{MO}} \newcommand{\MSO}{\mathrm{MSO}}
\newcommand{\colim}{\mathrm{colim}} \newcommand{\hocolim}{\mathrm{hocolim}}
\newcommand{\fin}{\mathrm{fin}} \newcommand{\Tot}{\mathrm{Tot}}
\newcommand{\im}{\mathrm{im}} \newcommand{\FT}{\mathrm{FT}}
\newcommand{\AA}{\mathbf{A}} \newcommand{\Frob}{\mathrm{Frob}}
\newcommand{\ex}{\mathrm{ex,pr}} \newcommand{\fil}{\mathrm{fil}}
\newcommand{\gr}{\mathrm{gr}} \newcommand{\un}{\mathrm{un}}
\newcommand{\Syn}{\mathrm{Syn}} \newcommand{\Cart}{\mathrm{Cart}}
\newcommand{\bo}{\mathrm{bo}} \newcommand{\mmod}{/\!\!/}
\newcommand{\bsp}{\mathrm{bsp}} \newcommand{\BPP}{\mathrm{BP}}
\newcommand{\CAlg}{\mathrm{CAlg}} \newcommand{\TCart}{\mathrm{TCart}}
\newcommand{\BW}{\mathrm{BW}} \newcommand{\Br}{\mathrm{Br}}
\newcommand{\Pic}{\mathrm{Pic}} \newcommand{\ext}{\mathrm{ext}}
\newcommand{\Cl}{\mathrm{Cl}} \newcommand{\disc}{\mathrm{disc}}
\newcommand{\dir}{D\!\!\!\!/} \newcommand{\bb}{\mathrm{bb}}
\newcommand{\Ran}{\mathrm{Ran}} \newcommand{\cu}{\mathcal{U}}
\newcommand{\Gr}{\mathrm{Gr}} \newcommand{\Alg}{\mathrm{Alg}}
\newcommand{\G}{\Gamma} \newcommand{\dY}{\mathcal{Y}}
\newcommand{\Line}{\mathrm{Line}} \newcommand{\MUP}{\mathrm{MUP}}
\newcommand{\Bl}{\mathrm{Bl}} \newcommand{\St}{\mathrm{St}}
\newcommand{\cB}{\mathcal{B}} \newcommand{\SL}{\mathrm{SL}}
\newcommand{\XX}{\mathrm{X}} \newcommand{\gp}{\mathrm{gp}}
\newcommand{\Q}{\mathrm{Q}} \newcommand{\cI}{\mathcal{I}}
\newcommand{\T}{\mathrm{T}} \newcommand{\D}{\mathrm{D}}
\newcommand{\Aff}{\mathrm{Aff}} \newcommand{\BGL}{\mathrm{BGL}}$$

In a bunch of posts a while back (see, e.g., [this
one](/algebraic-topology/2019/04/18/cmn.html)), we talked about a particular
element $$\sigma_{n-1}\in \pi_{|v_n|-1} X(p^n-1)$$ is in the $$\E_3$$-center
$$\ZZ_{n-1}$$ of $$X(p^n-1)$$. In this post, we will describe how this
conjecture simplifies the main part of the proof of the nilpotence theorem due
to [Devinatz-Hopkins-Smith](https://www.jstor.org/stable/1971440). I am
currently writing a paper (which is 99% done, I think) about the implications of
the centrality conjecture (and applications to the string orientation), and will
expand on the stuff in this post in a future paper. We will work at $$p=2$$ for
this post --- this is very important for the arguments to work as stated
(although, as you might expect, slight modifications work at odd primes)!

We need to show that if $$R$$ is a homotopy commutative ring, and $$x\in
\pi_d(R)$$ (with $$d>0$$) is in the kernel of the map $$h:\pi_\ast(R)\to
\BPP_\ast(R)$$, then $$x$$ is nilpotent. Since $$\BPP$$ is a filtered colimit of
the $$T(n)$$s, and the sphere is compact, the map $$h(x):S^d\to \BPP\wedge R$$
factors through some $$T(n) \wedge R$$. (Remember that $$T(n)$$ is a summand of
$$X(p^{n+1}-1)$$ --- so, we will abusively write $$\alpha\in \pi_\ast
X(p^{n+1}-1)$$ to also mean $$\alpha\in \pi_\ast T(n)$$ if $$\alpha$$ is nonzero
in $$T(n)$$.) To recall the strategy in Devinatz-Hopkins-Smith, we need to
introduce some notation.

Remember that these $$T(n)$$s can be constructed inductively: there is an element
$$\sigma_{n-1}\in \pi_{2p^n-3} T(n-1)$$, and the resulting map $$S^{2p^n-2} \to
\BGL_1(T(n-1))$$ factors through a map $$\mu: \Omega S^{2p^n-1} \to
\BGL_1(T(n-1))$$. The Thom spectrum $$(\Omega S^{2p^n-1})^\mu$$ is equivalent to
$$T(n)$$. The space $$\Omega S^{2p^n-1}$$ admits a filtration, given by the
James construction; define

$$G_k := \mathrm{Thom}(J_{p^k-1}(S^{2p^n-2}) \to \Omega S^{2p^n-1}
\xrightarrow{\sigma_n} \BGL_1(T(n-1))).$$

Therefore, $$G_0 = T(n-1)$$, and $$\colim G_k = T(n)$$; these $$G_k$$ are the
$$T(n-1)$$-module skeleta of $$T(n)$$.

The strategy of proof of the nilpotence theorem is the following. Let
$$h_n:\S\to T(n)$$ denote the Hurewicz map, so $$h_n(x) \in T(n)_\ast(R)$$ is
zero for some $$n\gg 0$$ by the preceding discussion. In other words, $$T(n)
\wedge R[1/x]$$ is zero. Then, it suffices to show:

* ("Step II" in DHS) If $$h_n(x) = 0$$, then there is some $$k\gg 0$$ such that
  $$G_k \wedge R[1/x] = 0$$.
* ("Step III" in DHS) If $$F$$ is a spectrum such that $$G_k \wedge F = 0$$,
  then $$G_{k-1} \wedge F = 0$$.

The first part ("Step II") essentially boils down to algebra (or the EHP
sequence, depending on how you choose to prove it), and the centrality
conjecture has nothing to do with it. The second part ("Step III"), however, is
the real meat of the nilpotence theorem, and that's where centrality comes in.

Let us sketch how this works. The key point is that $$G_k$$ is built from
$$G_{k-1}$$ via iterated cofibers of a particular self-map

$$\sigma_{n-1,p^{k-1}}: \Sigma^{p^{k-1}|v_n|-1} G_{k-1} \to G_{k-1}.$$

This map is multiplication by a particular element $$\sigma_{n-1, p^{k-1}}\in
\pi_{p^{k-1}|v_n|-1} X(p^n-1)$$, which is constructed from the element
$$\sigma_{n-1}\in \pi_{|v_n|-1} X(p^n-1)$$ in the same way that the
$$\alpha$$-family is constructed from $$\alpha_1$$ as explained in [this
post](/algebraic-topology/2020/02/12/alpha.html). (As I said, details will
appear in my paper.) The upshots of this construction are the following:

* the nilpotence theorem follows if we can show that all the $$\sigma_{n-1,
  p^{k}}$$ are nilpotent.
* there is a relation $$Q_1(\sigma_{n-1,p^{k-1}}) = \sigma_{n-1,p^{k}}$$.
* the centrality conjecture (i.e., that $$\sigma_{n-1}$$ lifts to the
  $$\E_3$$-center $$\ZZ_{n-1}$$) implies that $$\sigma_{n-1,p^{k-1}}$$ lifts to
$$\ZZ_{n-1}$$.

The second and third facts allow us to induct on $$k$$, because of the following
nice fact. If $$R$$ is any $$\E_3$$-ring, and $$x\in \pi_\ast(R)$$, then
$$Q_1(x)^2 = Q_2(x^2)$$. Therefore, in the $$\E_3$$-center $$\ZZ_{n-1}$$, we
have the following relation for any integer $$N$$:

$$N\sigma_{n-1,p^k}^2 = Q_2(N\sigma_{n-1,p^{k-1}}^2).$$

In other words, if $$\sigma_{n-1, p^{k-1}}^2$$ is killed by $$N$$, then so is
$$\sigma_{n-1, p^k}$$. We also know by the classical Hopkins-Mahowald
$$\H\FF_p$$-theorem that if an element in a ($$p$$-local) $$\E_2$$-ring is
killed by $$p$$, then it is nilpotent. So the nilpotency of the $$\sigma_{n-1,
p^k}$$s will follow by induction if we can just show that $$p$$ kills
$$\sigma_{n-1}^2$$. (This feels like cheating --- somehow, we're appealing to
the Hopkins-Mahowald $$\H\FF_p$$-theorem, which is a "height zero" phenomenon,
to this story for general heights $$n$$. More on this next time.)

There are lots of ways to show this. In fact, we claim that $$2$$ kills
$$\sigma_{n-1}^2$$. To see this, let's make the following general observation.

Let $$R$$ be an $$\E_{1}$$-ring, and let $$\alpha\in \pi_d R$$. Then $$\alpha$$
defines a map $$S^{d+1} \to \BGL_1(R)$$, and it is natural to ask when
$$\alpha$$ extends along $$S^{d+1} \to \Omega S^{d+2}$$, or at least along
$$S^{d+1} \to J_k(S^{d+1})$$ for some $$k$$. This is automatic if $$R$$ is an
$$\E_{2}$$-ring, but not necessarily so if $$R$$ is only an $$\E_{1}$$-ring.
Recall that there is a cofiber sequence

$$S^{(k+1)(d+1)-1} \to J_k(S^{d+1})\to J_{k+1}(S^{d+1}),$$

where the first map is the $$(k+1)$$-fold Whitehead product $$[\iota_{d+1},
[\cdots, [\iota_{d+1}, \iota_{d+1}]], \cdots]$$. In particular, the map
$$S^{d+1} \to \BGL_1(R)$$ extends along the map $$S^{d+1} \to J_k(S^{d+1})$$ if
and only if there are compatible nullhomotopies of the $$n$$-fold Whitehead
products $$[\alpha, [\cdots, [\alpha, \alpha]], \cdots] \in \pi_\ast \BGL_1(R)$$
for $$n\leq k$$. These amount to properties of Toda brackets in the homotopy of
$$R$$. We note, for instance, that the Whitehead bracket $$[\alpha, \alpha]\in
\pi_{2d+1} \BGL_1(R) \cong \pi_{2d} R$$ is the element $$2\alpha^2$$; therefore,
the map $$S^{d+1}\to \BGL_1(R)$$ extends to $$J_2(S^{d+1})$$ if and only if
$$2\alpha^2 = 0$$.

So, $$2\sigma_{n-1}^2 = 0$$ follows from the known fact that $$\sigma_{n-1}:
S^{|v_n|} \to \BGL_1(X(p^n-1))$$ extends not just to $$J_2(S^{|v_n|})$$, but all
the way to $$\Omega S^{|v_n|+1}$$. Depending on your style, this is how we
[*defined*](/algebraic-topology/2019/04/01/mrs.html) $$\sigma_{n-1}$$. That
finishes the proof that all the $$\sigma_{n-1, p^{k}}$$ are nilpotent, and hence
("Step III" of) the nilpotence theorem.
