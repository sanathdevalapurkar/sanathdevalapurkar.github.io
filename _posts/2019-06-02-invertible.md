---
layout: post
title:  "Invertible TQFTs"
date:   2019-06-02
categories: physics
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
\newcommand{\pic}{\mathrm{Pic}} \newcommand{\RP}{\mathbf{R}P}
\newcommand{\BO}{\mathrm{BO}} \newcommand{\cc}{\mathbf{C}}
\newcommand{\CP}{\mathbf{C}P} \newcommand{\wt}[1]{\widetilde #1}
\newcommand{\RR}{\mathbf{R}} \renewcommand{\S}{\mathbb{S}}
\newcommand{\Lone}{L_{K(1)}} \newcommand{\Ltwo}{L_{K(2)}}
\newcommand{\gl}{\mathrm{gl}} \newcommand{\Lk}{L_{K(n)}}
\newcommand{\ku}{\mathrm{ku}} \newcommand{\ko}{\mathrm{ko}}
\newcommand{\GL}{\mathrm{GL}} \newcommand{\Ln}{L_n}
\newcommand{\Lt}{L_{K(t)}} \newcommand{\W}{\mathrm{W}}
\newcommand{\BU}{\mathrm{BU}} \newcommand{\SU}{\mathrm{SU}}
\newcommand{\MU}{\mathrm{MU}} \newcommand{\ul}[1]{\underline #1}
\newcommand{\Sq}{\mathrm{Sq}} \newcommand{\Tr}{\mathrm{Tr}}
\newcommand{\d}{\mathrm{d}} \newcommand{\HP}{\mathbf{H}P}
\newcommand{\cL}{\mathcal{L}} \newcommand{\cs}{\mathrm{cs}}
\newcommand{\cd}{\mathcal{D}} \newcommand{\Bord}{\mathrm{Bord}}
\newcommand{\SO}{\mathrm{SO}} \newcommand{\cC}{\mathcal{C}}
\newcommand{\Sp}{\mathrm{Sp}} \newcommand{\Lkd}{L_{K(d)}}
\newcommand{\Mod}{\mathrm{Mod}} \newcommand{\cH}{\mathcal{H}}
\newcommand{\ket}[1]{|#1 \rangle} \newcommand{\Bun}{\mathrm{Bun}}
\newcommand{\cM}{\mathcal{M}} \newcommand{\MTH}{\mathrm{MT}H}
\newcommand{\MSO}{\mathrm{MSO}}$$

Most of this post will be heuristic arguments; we will initially only consider
non-extended TQFTs (i.e., TQFTs in the sense of Atiyah), and then move on to
extended TQFTs. Consider a closed $$n$$-manifold $$M$$ (often $$n=3$$) with
finitely many $$0$$-cells $$\Delta^0$$. Consider a quantum system defined on
$$M$$: let $$\cH$$ denote the Hilbert space $$\bigotimes_{v\in \Delta^0} \cH_v$$
(we will often just consider a finite-dimensional space, and assume that
$$\cH_v$$ are all of the saame dimension), and let $$H$$ be the Hamiltonian of
the system. The Ising model, for instance, corresponds to the case when each
$$\cH_v$$ is $$2$$-dimensional (with basis $$\ket{\uparrow}$$ and
$$\ket{\downarrow}$$). In this case, one choice for the Hamiltonian $$H$$ is

$$H = -J\sum_{e\in \Delta^1, \ \partial e = i,j} \sigma^z_i \sigma^z_j -
h\sum_{v\in \Delta^0} \sigma^x_v,$$

where $$h$$ and $$J$$ are nonzero constants, and the $$\sigma$$s are the Pauli
matrices (generators of $$\mathfrak{su}_2$$). The first term is a spin-spin
interaction term, while the second corresponds to a magnetic field. Studying he
Ising model shows that there's a symmetry breaking when $$h$$ is turned on.

The ground state of this system is when all sites (vertices) have the same spin,
and the first excited state is when only one of the spins is different. Let us
suppose for simplicity that $$J=0$$; then, turning on one of the spins creates
an energy gap of $$2h$$ between the ground state and the first excited state.
Thanks to this property, the quantum system is said to be "gapped" (somewhat
more precisely, the lowest energy eigenvalue is an isolated point of the
spectrum of the Hamiltonian). Note that there is a unique ground state in this
system; we distinguish the case $$J=0$$ by saying that the system is in the
*trivial phase*. More generally, all sites are in the same state in the ground
state of the trivial phase.

It is interesting to consider an equivalence relation on Hamiltonians: two
Hamiltonians $$H$$ and $$H'$$ are in the same gapped phase if there is a smooth
deformation between $$H$$ and $$H'$$, i.e., there is a smooth path of gapped
Hamiltonians $$H(\lambda)$$ for $$\lambda\in [0,1]$$ with $$H(0) = H$$ and
$$H(1) = H'$$. Equivalently, if $$H_0$$ is a Hamiltonian acting on a state space
$$\cH_0$$ in the trivial phase, then $$H$$ acting on a state space $$\cH$$ is in
the same phase as $$H+H_0$$ acting on the state space $$\cH\otimes \cH_0$$. This
suggests the following definition: if $$H$$ is a gapped Hamiltonian acting on
the state space $$\cH$$, then $$H$$ is said to be in an invertible phase if
there is a Hamiltonian $$H'$$ with state space $$\cH'$$ for which $$H+H'$$
acting on $$\cH\otimes \cH'$$ is in the same phase as the trivial phase. If
$$H$$ is in an invertible phase, then it admits a
unique ground state, because $$H+H'$$ deforms to the trivial phase, which has a
unique ground state --- and, crucially, the deformation does not close the gap.
In particular, for a system in an invertible
phase, there is an energy gap, and the Hilbert space of ground states is
one-dimensional. I think that such a system is also said to be in an SPT
(symmetry-protected topological) phase.

A system in an invertible phase is short-range entangled. [One
definition](https://arxiv.org/pdf/1004.3835.pdf)of this latter term (the
original one) is that it is in the same gapped phase as an unentangled state
(the all-up or all-down states in the Ising model). With this definition, there
is a unique ground state, and in fact in [this
talk](http://online.kitp.ucsb.edu/online/topomat11/kitaev/), this is taken to be
the definition of a short-range entangled state. (A small $$J$$ or $$h$$ can
only affect the ground state of the Ising model locally.) I think that Freed and
Hopkins use this latter definition. I don't fully understand the physics behind
this stuff, but hopefully I will soon.

Let's now briefly shift gears; consider a system in a gapped phase. Often, the
infrared (low energy) limit (the "effective field theory") of such a system
gives rise to a TQFT. (Note that in natural units, since $$\hbar$$ has units of
$$\mathrm{mass}\times \mathrm{length}^2/\mathrm{time}$$ and $$c$$ has units of
$$\mathrm{length}/\mathrm{time}$$, the low energy limit is the same as the
long-distance limit.) There is a general heuristic that *the low-energy limit of
a gapped system is approximated by a TQFT*, i.e., that there is a TQFT $$Z$$
whose value $$Z(M)$$ on a closed $$(n-1)$$-manifold is $$\ker(H:\cH\to \cH)$$.
For instance, Chern-Simons theory is the effective field theory of a fractional
quantum Hall liquid.

Here is a heuristic argument for why the low-energy limit of a system should be
described by a TQFT. Let $$M$$ be a closed Riemannian $$n$$-manifold with metric
$$g$$, and let $$x\in M$$. Let $$\epsilon>0$$, and consider $$S_\epsilon(x)$$, a
sphere of radius $$\epsilon$$ around $$x$$. If $$Z$$ is a quantum field theory,
then $$Z(S_\epsilon(x))$$ is a state space of observables around $$x$$; the
space of point observables $$V_x$$ is the inverse limit of $$Z(S_\epsilon(x))$$
as $$\epsilon\to 0$$. If $$x_1,\cdots,x_n$$ are points in $$M$$, then
$$M\setminus \{x_1,\cdots,x_n\}$$ is a compact manifold which is a(n oriented,
if $$M$$ has an orientation) cobordism between $$\coprod S_\epsilon(x_i)$$ and
$$\emptyset$$; therefore, $$Z$$ defines a map $$V_{x_1}\otimes \cdots \otimes
V_{x_n} \to \cc$$. The value on operators is the $$n$$-point function $$\langle
\co_{x_1} \cdots \co_{x_n}\rangle$$. If $$Z$$ is a *topological* quantum field
theory, then $$Z(S_\epsilon(x))$$ is independent of $$\epsilon$$.

Now, it is a general fact that the energy-momentum tensor $$T_{\mu\nu}$$
satisfies the property 

$$\frac{\delta}{\delta g^{\mu\nu}(x)} \langle \co_{x_1} \cdots \co_{x_n}\rangle
= \langle \co_{x_1} \cdots \co_{x_n} T_{\mu\nu} (x)\rangle.$$

If $$T=0$$, then you end up with a topological field theory: the $$n$$-point
functions do not depend on the metric $$g$$ on $$M$$. One way to approximate
$$T=0$$ is to go to the low-energy limit.

Consider, for instance, the toric code/lattice gauge theory associated to a
finite group $$G$$ and a character $$\chi:G\to \cc^\times$$. This is a quantum
system defined on every closed manifold $$M$$ with a triangulation (defining a
CW-structure). Let $$M^{(n)}$$ denote the $$n$$-skeleton of $$M$$, and let
$$\Delta^k$$ be the set of $$k$$-cells of $$M$$. Define the space of fields
$$\Bun_G(M^{(1)}; M^{(0)})$$ to be the groupoid of $$G$$-bundles $$P$$ over
$$M^{(1)}$$ equipped with a section $$s$$ over $$M^{(0)}$$ (i.e., a
trivialization over the zero-skeleton of $$M$$). The space of states $$\cH$$ is
defined to be the (finite-dimensional) space $$\cc[\Bun_G(M^{(1)}; M^{(0)})]$$
of complex functions. For each $$v\in M^{(0)}$$, there is a map
$$\sigma_v:\Bun_G(M^{(1)}; M^{(0)})\to \Bun_G(M^{(1)}; M^{(0)})$$ defined as
follows: $$\sigma_v(P,s)$$ is defined to be the pair $$(P,s_v)$$, where $$s_v$$
is the same as the section $$s$$ on $$M^{(0)}\setminus \{v\}$$, and is
$$s(v)+1$$ on $$v$$. This defines a map $$\sigma_v^\ast:\cH\to \cH$$. The
Hamiltonian of the system is then defined as the sum $$J_1\sum_{v\in M^{(0)}}
H_v + J_2\sum_{f\in \Delta^2} H_f$$, where $$J_1$$ and $$J_2$$ are nonnegative
constants and

$$H_v \psi = \frac{1}{2} (\psi - \sigma_v^\ast \psi), \ H_f \psi = \frac{1 -
(-1)^{\mathrm{Hol}_P(f)}}{2} \psi,$$

where $$\mathrm{Hol}_P(f)$$ is the holonomy of $$P$$ around $$\partial f$$ with
respect to the character $$\chi:G\to \cc^\times$$: it is the evaluation of the
composite of the map $$\pi_1(M) \to G$$ (induced from the classifying map $$M\to
BG$$ of $$P$$) with $$\chi$$ on the $$1$$-cycle $$\partial f$$. (The classical
toric code corresponds to $$G = \Z/2$$ and $$\chi$$ being the canonical
inclusion $$\Z/2\subseteq \cc^\times$$).

What is the ground state of the toric code? If $$H_v\psi = 0$$, then $$\psi =
\sigma_v^\ast \psi$$; therefore, $$\psi:\Bun_G(M^{(1)}; M^{(0)}) \to \cc$$ does
not depend on the value of $$s$$ around $$v$$, i.e., $$\psi$$ is a function on
$$\Bun_G(M^{(1)})$$. If $$H_f\psi = 0$$, then $$\psi = (-1)^{\mathrm{Hol}_P(f)}
\psi$$, so $$\psi$$ must vanish on all bundles in $$\Bun_G(M^{(1)})$$ with
nontrivial holonomy around $$\partial f$$. So at least in the $$2$$-dimensional
case, the space of ground states of the toric model is a purely topological
invariant of $$M$$. As such, we expect there to be a topological field theory
whose value is this space of ground states.

Back to the [main plot](https://arxiv.org/pdf/1604.06527.pdf). If we're
interested in understanding the low energy limit of gapped systems in an
invertible phase, then we should try to understand topological quantum field
theories whose value on a closed $$(n-1)$$-dimensional manifold (spacelike
slice) is $$1$$-dimensional. (In order to get something physical, we need to add
more conditions, like unitarity; we'll get to that later.) Such TQFTs are known
as invertible; we'd like to understand these objects. Since the field theories
under consideration might have symmetry, we will define a generalized bordism
$$(\infty,n)$$-category $$\Bord^{(X,\xi)}_n$$ associated to a space $$X$$ with a
real bundle $$\xi$$ of dimension $$n$$ as follows: a $$k$$-morphism is a
$$k$$-dimensional manifold $$M$$ with corners with a map $$f:M\to X$$ equipped
with an isomorphism $$f^\ast \xi \cong \tau_M\oplus \epsilon^{n-k}$$.

We'll now consider extended TQFTs. If $$\cC$$ is a symmetric monoidal
$$(\infty,n)$$-category, then a TQFT $$Z:\Bord^{(X,\xi)}_n\to \cC$$ is said to
be invertible if $$Z$$ factors through the Picard space $$\pic(\cC)$$. The data
of a symmetric monoidal functor $$\Bord^{(X,\xi)}_n\to \pic(\cC)$$ is the same
as an infinite loop map $$|\Bord^{(X,\xi)}_n| \to \pic(\cC)$$, where $$|\cdot|$$
denotes geometric realization. In [this
paper](https://arxiv.org/pdf/1712.08029.pdf), Schommer-Pries shows that
$$|\Bord^{(X,\xi)}_n|$$ is the infinite loop space $$\Omega^{\infty-n}
X^{-\xi}$$, where $$X^{-\xi}$$ is the Thom spectrum of the virtual bundle
$$-\xi$$.

Great --- what about the target $$\pic(\cC)$$? Since finding target symmetric
monoidal $$(\infty,n)$$-categories is a hard task, we should try consider some
sort of "physical" universal target. What happens for low $$n$$? For the
degenerate case $$n=0$$, $$\cC$$ is just the vector space $$\cc$$ (just assign a
number to a point). For $$n=1$$, $$\cC$$ is $$\mathrm{Vect}_\cc$$; for $$n=2$$,
$$\cC$$ is the category of $$\cc$$-algebras, bimodules, and bimodule
homomorphisms (as we discussed [last time](/physics/2019/06/01/tqft.html)).
Let's denote the universal "physical" target $$(\infty,n)$$-category by
$$\cC_n$$; then, in each of these cases, the automorphism
$$(\infty,n-1)$$-category of the unit object is $$\cC_{n-1}$$. In other words,
$$\cC_{n-1}$$ is "$$\Omega \cC_n$$". This is literally true at the level of
Picard spaces: $$\pic(\cC_{n-1}) = \Omega \pic(\cC_n)$$. As such,
$$\{\pic(\cC_n)\}$$ forms an $$\Omega$$-spectrum, which we will just denote by
$$\pic(\cC)$$. (Note that this isn't the Picard space (it's not even a space!)
of any $$\cC$$.)

What are the homotopy groups of this spectrum? Since $$\pi_k \pic(\cC)$$ is the
homotopy of the zeroth space, which is $$\pic(\cC_0) = \pic(\cc) = \cc^\times$$,
we find that if we impose the discrete topology on $$\cc^\times$$, then $$\pi_k
\pic(\cC) = 0$$ for $$k>0$$, and is $$\cc^\times$$ for $$k=0$$. This is good: we
know that an invertible field theory is an infinite loop map $$\Omega^{\infty-n}
X^{-\xi}\to \Omega^\infty \pic(\cC)$$, i.e., a map of spectra $$\Sigma^n
X^{-\xi} \to \pic(\cC)$$. If we demand that the partition function determines
the invertible TQFT (discussed below), then this infinite loop map should be
recoverable upon taking $$\pi_0$$. Taking $$\pi_0$$ defines a map $$\pi_{-n}
X^{-\xi}\to \cc^\times$$. Since $$\cc^\times$$ is an injective abelian group,
there is an isomorphism $$[E, I_{\cc^\times}] \to [\pi_0 E, \pi_0
I_{\cc^\times}]$$, where $$I_{\cc^\times}$$ is the Brown-Comenetz dualizing
spectrum (they have the same $$p$$-completion for every prime $$p$$); therefore,
the map on $$\pi_0$$ lifts to a map $$\Sigma^n X^{-\xi} \to \Sigma^n
I_{\cc^\times}$$.  Consequently, we hypothesize that $$\pic(\cC) =
I_{\cc^\times}$$, i.e., that $$\pic(\cC_n) = \Omega^{\infty-n} I_{\cc^\times}$$,
and therefore that an (isomorphism class of an) invertible $$n$$-dimensional
TQFT with source $$\Bord^{(X,\xi)}_n$$ is a map of spectra $$X^{-\xi} \to
I_{\cc^\times}$$. Another way to say this is as follows: let $$\cM(X,\xi)$$
denote the moduli space of invertible $$n$$-dimensional TQFTs with source
$$\Bord^{(X,\xi)}_n$$; then $$\pi_0 \cM(X,\xi) = [X^{-\xi}, I_{\cc^\times}]$$.
Since we imposed the discrete topology on $$\cc^\times$$, these should really be
called *discrete* invertible TQFTs. There is a fiber sequence

$$H\cc\to I_{\cc^\times} \to \Sigma I_\Z.$$

Let $$Z_0,Z_1:X^{-\xi} \to I_{\cc^\times}$$ be invertible TQFTs; then $$Z_0$$
and $$Z_1$$ are said to be deformation equivalent if there is an element of
$$[X^{-\xi}, H\cc]$$ whose image in $$[X^{-\xi}, I_{\cc^\times}]$$ is the
difference $$Z_0-Z_1$$. In other words, a deformation of an invertible TQFT
$$\Sigma^n X^{-\xi} \to \Sigma^n I_{\cc^\times}$$ factors through $$\Sigma^n
H\cc$$, so $$\pi_0$$ of the moduli of deformation classes of discrete invertible
$$n$$-dimensional TQFTs is $$[\Sigma^n X^{-\xi}, \Sigma^{n+1}
I_{\Z}]_\mathrm{tor}$$, the torsion subgroup of $$[\Sigma^n X^{-\xi},
\Sigma^{n+1} I_{\Z}]$$ (the restriction stems from the fact that we're looking
at the image of $$[\Sigma^n X^{-\xi}, \Sigma^n I_{\cc^\times}]$$). Studying
deformation classes of invertible TQFTs is important because this corresponds to
understanding deformation classes (the equivalence relation on gapped phases we
discussed earlier) of invertible (SPT, really) phases. As such, Freed and
Hopkins hypothesize that a *continuous* invertible $$n$$-dimensional extended
TQFT (with symmetry $$(X,\xi)$$) is a map $$\Sigma^n X^{-\xi} \to \Sigma^{n+1}
I_{\Z}$$.

(I want to make an unexplained observation at this point. Let $$E$$ denote a
Morava $$E$$-theory of height $$n$$ with algebraically closed residue field;
then, the fiber of the map $$\gl_1(E) \to L_n \gl_1(E)$$ agrees with the
homotopy of $$\Sigma^n I_{\QQ_p/\Z_p}$$ in nonnegative degrees, and so the fiber
of the map $$\gl_1(E) \to L_n \gl_1(E)$$ agrees with the homotopy of
$$\Sigma^{n+1} I_{\Z_p}$$. Surely the appearance of $$\Sigma^{n+1} I_{\Z_p}$$ in
both of these places isn't a coincidence!)

In order to test these claims against the known calculations of deformation
classes of invertible phases, we need to make an appropriate choice of $$X$$ and
$$\xi$$. To impose some sort of geometric structure on our manifold, one often
lets $$X$$ be a classifying space $$BH_n$$ (where $$n$$ corresponds to the
dimension of the TQFT), and $$\xi$$ be the bundle induced by a group
homomorphism $$H_n \to \mathrm{O}(n)$$. One moreover requires that the image of
this homomorphism contain $$\mathrm{SO}(n)$$; the kernel $$K$$ of this
homomorphism is the group of internal symmetries. One can "stabilize" the map
$$H_n\to \mathrm{O}(n)$$: it can be shown that for every $$m\geq n$$, there are
compact Lie groups $$H_m$$ and maps $$H_m\to \mathrm{O}(m)$$ such that
$$H_{m-1}$$ is the pullback $$H_m\times_{\mathrm{O}(m)} \mathrm{O}(m-1)$$. Let
$$H$$ denote the colimit of the maps $$H_{m-1} \to H_m$$, and let $$\xi$$ denote
the map $$H\to \mathrm{O}$$.

Let $$\MTH_n$$ denote the associated Thom spectra $$\mathrm{B}H_n^{-\xi}$$, so
we obtain maps of spectra $$\Sigma^n \MTH_n\to \Sigma^{n+1} \MTH_{n+1}$$. Let
$$\MTH = \mathrm{B}H^{-\xi}$$ denote the colimit. An $$n$$-dimensional
invertible TQFT $$Z:\Sigma^n \MTH_n\to \Sigma^n I_{\cc^\times}$$ is said to be
stable if it factors through $$\MTH$$. There is a cofiber sequence
$$\Sigma^{\infty+n}_+ \mathrm{B}H_{n+1} \to \Sigma^n \MTH_n \to \Sigma^{n+1}
\MTH_{n+1}$$; this can be used to show that an $$n$$-dimensional invertible TQFT
is stable if and only if $$Z(S^n) = 1$$.

It turns out that stability is related to a naturally arising physical
condition, called "reflection positivity" (this is Wick-rotated unitarity; I'll
talk about in the next post). In Theorem 8.20 of their paper, Freed and Hopkins
show that the space of stable continuous $$n$$-dimensional TQFTs is the same as
the space of continuous reflection positive $$n$$-dimensional extended TQFTs. In
particular, after combining with the discussion above, we obtain the main
theorem of [this paper](https://arxiv.org/pdf/1604.06527.pdf): $$\pi_0$$ of the
moduli space $$\cM_u(\mathrm{B}H,\xi)$$ of deformation classes of reflection
positive extended invertible $$n$$-dimensional TQFTs with symmetry $$(H_n,\xi)$$
is $$[\MTH, \Sigma^{n+1} I_\Z]_\mathrm{tor}$$.

I'll conclude with the following. During the derivation of the identification
$$\pi_0 \cM_u(BH,\xi) = [\MTH, \Sigma^n I_{\cc^\times}]$$, we demanded that the
partition function determines the invertible TQFT. Can we make this explicit?
Namely, given an element $$Z$$ of $$[\MTH, \Sigma^n I_{\cc^\times}] = \Map(\pi_n
\MTH, \cc^\times)$$, can we explicitly construct a TQFT? Let us only attempt to
do this in the *non-extended* setting, in the case $$\MTH = \MSO$$. We know in
this case that $$\pi_{n-1} \MTH = \pi_{n-1} \MSO$$ is a finitely generated
abelian group, say $$\Z^r\oplus \bigoplus_{i=r+1}^{r+k} \Z/m_i \Z$$, where $$k$$
and $$m_i$$ are some finite integers. Choose generators $$M_1,\cdots,M_{r+k}$$
of these $$r+k$$ groups, so that an arbitrary $$n$$-dimensional "$$H$$-manifold"
$$M$$ is cobordant to some $$M_i$$; define $$Z(M)$$ to be the following quotient
of the free $$\cc$$-vector space $$V(M)$$ with basis given by the set
$$\Map_{\Bord_{[n-1,n]}}(M, M_i)$$. Let $$v_X$$ and $$v_Y$$ be two elements of
$$V(M)$$ corresponding to bordisms $$X,Y: M\to M_i$$; then, define a closed
manifold $$B$$ as follows: compose the bordism $$\emptyset \to -M\sqcup M$$ with
$$-X\sqcup Y: -M\sqcup M \to -M_i \sqcup M_i$$ with $$-M_i \sqcup M_i \to
\emptyset$$. Identify $$v_X$$ and $$v_Y$$ if $$v_X = Z(B) v_Y$$, where $$Z(B)$$
is the evaluation of $$Z:\pi_n \MTH \to \cc^\times$$ on $$B$$. It is not hard to
see that $$Z(M)$$ defined as above is in fact a one-dimensional $$\cc$$-vector
space. To define an unextended TQFT, we need to define a linear transformation
$$Z(M) \to Z(M')$$ associated to each bordism $$B:M' \to M$$. But this is easy
(it's why the above construction was chosen): we just send the vector in
$$Z(M)$$ corresponding to $$X$$ to the vector in $$Z(M')$$ corresponding to the
composite $$B\circ X'$$.
