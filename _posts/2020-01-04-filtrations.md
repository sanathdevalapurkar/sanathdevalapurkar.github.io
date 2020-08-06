---
layout: post
title:  "Filtrations"
date:   2020-01-04
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
\newcommand{\CAlg}{\mathrm{CAlg}} \newcommand{\TCart}{\mathrm{TCart}}$$

Our goal in this post is to redo some of the stuff in Section 3 of [this
paper](https://www.math.ias.edu/~lurie/papers/Waldhaus.pdf) from the
perspective of filtrations being equivalent to living over $$\AA^1/\GG_m$$.
This approach in the classical setting was pioneered by Simpson.

Let us first recall some major players. Let $$\Rep(\Z) = \Fun(\Z, \Sp)$$ be the
category of filtered spectra; here, our indexing will be *opposite* that of
Lurie’s, so that a filtered spectrum has maps $$X_i\to X_{i+1}$$.  We will also
often denote this by $$\Sp_\fil$$. Similarly, let $$\Rep(\Z^\mathrm{ds}) =
\Fun(\Z^\mathrm{ds}, \Sp)$$ be the category of graded spectra; we will often
denote this by $$\Sp_\gr$$. Also let $$\Rep^\fin(\Z) = \Sp_\fil^\omega$$ denote
the category of finite filtered spectra, i.e., filtered spectra $$\{X_n\}_{n\in
\Z}$$ where each $$X_n$$ is finite, such that $$X_n = 0$$ for $$n \ll 0$$, and
such that the map $$X_{n-1} \to X_n$$ is an equivalence for $$n\gg 0$$.

Then, if $$\cC$$ is an $$\infty$$-category, a local filtration on $$\cC$$
is the data of an action of $$\Z$$ on $$\cC$$, i.e., a monoidal functor $$\Z\to
\Fun(\cC, \cC)$$. Let $$\Cat^\fil_\infty$$ denote the $$\infty$$-category of
locally filtered presentable stable $$\infty$$-categories, with symmetric
monoidal structure such that $$\Sp_\fil$$ is the unit object. There is a
canonical symmetric monoidal functor $$\un:\Cat^\fil_\infty\to
\Cat_\infty^\ex$$ sending a locally filtered presentable stable
$$\infty$$-category to its underlying presentable stable $$\infty$$-category.
If $$\cC$$ is a locally filtered stable $$\infty$$-category and $$X\in \cC$$,
then we denote by $$X(n)$$ the object $$X$$ shifted to live in filtration
$$n$$.

We now introduce the stack $$\AA^1/\GG_m$$. Let $$\S[\tau]$$ denote the
$$\Eoo$$-ring $$\Sigma^\infty_+ \Z_{\geq 0}$$, where the $$\Eoo$$-ring structure
comes from the monoid structure of $$\Z_{\geq 0}$$. Let $$\AA^1 =
\spec(\S[\tau])$$, and let $$\GG_m = \spec \Sigma^\infty_+ \Z$$. There is a
natural action of $$\GG_m$$ on $$\AA^1$$. Let $$\AA^1/\GG_m$$ (resp. $$B\GG_m$$)
denote the geometric stack given by the geometric realization of the simplicial
object $$X_\bullet = (\AA^1)^{\times_{\GG_m} \bullet+1}$$ (resp. $$(\spec
\S)^{\times_{\GG_m} \bullet + 1}$$, where $$\GG_m$$ acts trivially on $$\spec
\S$$) in fpqc-sheaves on $$\CAlg$$. Let $$u$$ (resp. $$g$$) denote the canonical
morphism $$1:\spec \S\to \AA^1/\GG_m$$ (resp. $$0:B\GG_m\to \AA^1/\GG_m$$).

Then, a local filtration on a stable $$\infty$$-category $$\cC$$ is equivalent
to the data of a quasicoherent sheaf $$\cf_\cC$$ of stable $$\infty$$-categories
on $$\AA^1/\GG_m$$ along with an equivalence between the global sections of the
sheaf $$u^\ast \cf_\cC$$ on $$\spec \S$$ and $$\cC$$. More precisely:

**Theorem:** There is an equivalence $$\Cat^\fil_\infty \simeq
\QCoh_{\Cat^\ex_\infty}(\AA^1/\GG_m)$$. Moreover, under this equivalence, the
functor $$u^\ast: \QCoh_{\Cat^\ex_\infty}(\AA^1/\GG_m)\to
\QCoh_{\Cat^\ex_\infty}(\spec \S) \simeq \Cat^\ex_\infty$$ coincides with the
functor $$\un$$.

To show this, we need some lemmas.

**Lemma:** There is a symmetric monoidal equivalence
$$\QCoh_{\Cat^\ex_\infty}(\dX) \simeq \Mod_{\QCoh(\dX)}(\Cat^\ex_\infty)$$ for
any weakly perfect stack $$\dX$$ (see Definition 9.4.3.3 of
[SAG](http://www.math.harvard.edu/~lurie/papers/SAG-rootfile.pdf)).

To see this, we utilize Proposition 4.8.5.8 of
[HA](http://www.math.harvard.edu/~lurie/papers/HA.pdf). First note that
$$\Cat^\ex_\infty$$ admits geometric realizations of simplicial objects and the
tensor product preserves geometric realizations (since it is closed under
filtered colimits and the tensor product of presentable $$\infty$$-categories
preserves colimits separately in each variable). Clearly
$$\QCoh_{\Cat^\ex_\infty}(\dX)$$ is left-tensored over $$\Cat^\ex_\infty$$. We
now check each of the conditions of Proposition 4.8.5.8 of
[HA](http://www.math.harvard.edu/~lurie/papers/HA.pdf):

* $$\QCoh_{\Cat^\ex_\infty}(\dX)$$ admits geometric realizations of simplicial
  objects (since it admits filtered colimits).
* The action 

  $$\Cat^\ex_\infty \times \QCoh_{\Cat^\ex_\infty}(\dX)\to \QCoh_{\Cat^\ex_\infty}(\dX)$$

  preserves geometric realizations of simplicial objects, since it in fact
preserves filtered colimits.
* Since $$\dX$$ is weakly perfect, $$\QCoh(\dX)$$ is a dualizable object of
  $$\Cat^\ex_\infty$$. Therefore, the functor $$\Cat^\ex_\infty\to
\QCoh_{\Cat^\ex_\infty}(\dX)$$ sending $$\cC$$ to $$\cC\otimes \QCoh(\dX)$$
admits a right adjoint (given by tensoring with $$\QCoh(\dX)^\vee$$). 
* The functor $$G:\QCoh_{\Cat^\ex_\infty}(\dX)\to \Cat^\ex_\infty$$ given by
  tensoring with $$\QCoh(\dX)^\vee$$ preserves filtered colimits, and is
conservative. Similarly, item (6) of Proposition 4.8.5.8 of HA is direct.

The following is the main result of [this
paper](https://arxiv.org/abs/1907.13562v1).

**Lemma:** There is a symmetric monoidal equivalence $$\QCoh(\AA^1/\GG_m)
\simeq \Sp_\fil$$.

Finally, we prove the theorem. By Remark 3.1.12 of Lurie, there is an
equivalence $$\Cat^\fil_\infty \simeq \Mod_{\Rep^\fin(\Z)}(\Cat^\ex_\infty)$$.
Since $$\Cat^\ex_\infty$$ is the $$\infty$$-category of *presentable*
stable $$\infty$$-categories, any action of $$\Rep^\fin(\Z)$$ on $$\cC\in
\Cat^\ex_\infty$$ extends canonically to an action of $$\Rep(\Z) = \Sp_\fil$$.
In particular, $$\Cat^\fil_\infty \simeq \Mod_{\Sp_\fil}(\Cat^\ex_\infty)$$.
Since $$\AA^1/\GG_m$$ is weakly perfect (being the quotient of a perfect stack
by a flat affine group scheme), the first sentence of the theorem follows from
the two lemmas. The second sentence is immediate from the first.

Next, according to Section 3.2 of Lurie’s
[paper](https://www.math.ias.edu/~lurie/papers/Waldhaus.pdf), the associated
graded functor $$\Sp_\fil\to \Sp_\gr$$ factors as follows: there is an
$$\Eoo$$-algebra object $$\AA\in \Sp_\fil$$ which produces a symmetric monoidal
equivalence $$\Sp_\gr \simeq \Mod_\AA(\Sp_\fil)$$. Under this equivalence, the
functor $$-\otimes \AA:\Sp_\fil\to \Mod_\AA(\Sp_\fil)$$ is the associated
graded functor.

**Prop:** Under the equivalence of the second lemma, the quasicoherent sheaf
$$g_\ast\co_{B\GG_m}\in \QCoh(\AA^1/\GG_m)$$ may be identified with $$\AA$$ as
$$\Eoo$$-algebras.

To see this, let $$p:\AA^1\to \AA^1/\GG_m$$ denote the quotient map, and let
$$\cf_\AA\in \CAlg(\QCoh(\AA^1))$$ denote the $$\S[\tau]$$-module $$\S$$ (where
$$\tau$$ acts by zero). Then there is a canonical equivalence $$p_\ast \cf_\AA
\simeq g_\ast \co_{B\GG_m}$$ as $$\Eoo$$-algebras in $$\QCoh(\AA^1/\GG_m)$$.

We will abusively identify $$\AA\in \Sp_\fil$$ with its image in
$$\QCoh(\AA^1/\GG_m)$$. Then there is an $$\Eoo$$-map $$p_\ast \cf_\AA \to
\AA$$ given by an $$\Eoo$$-map $$\cf_\AA\to p^\ast \AA$$ in $$\QCoh(\AA^1)$$.
This map is an equivalence: indeed, there is a cofiber sequence
$$\co_{\AA^1}\to \co_{\AA^1}\to \cf_\AA$$ in $$\QCoh(\AA^1)$$, where the first
map given by $$\tau$$-multiplication. By Remark 3.2.8 of Lurie’s paper, there
is a similar cofiber sequence $$\S(-1)\to \S\to \AA$$ in $$\Sp_\fil$$; this
pulls back via $$p$$ to a cofiber sequence in $$\QCoh(\AA^1)$$. There is an
evident map of cofiber sequences in $$\QCoh(\AA^1)$$, and it induces an
equivalence $$\cf_\AA\to p^\ast \AA$$.

As a consequence:

**Corollary** Let $$\cC$$ be a presentable stable $$\infty$$-category, and let
$$\cC_\fil$$ (resp. $$\cC_\gr$$) denote the category $$\Fun(\Z, \cC)$$ (resp.
$$\Fun(\Z^\mathrm{ds}, \cC)$$). Then $$\cC_\fil$$ is a $$\Sp_\fil$$-module in
$$\Cat^\fil_\infty$$, and the associated graded functor $$\cC_\fil\to \cC_\gr$$
is given by tensoring with $$\AA$$.

Thanks to the proposition and its proof, we will abusively switch between the
notation $$\AA$$ and $$C\tau$$: colloquially speaking, one should think of
tensoring with $$C\tau$$ (i.e., killing $$\tau$$) as passing to the associated
graded. The following result is proved similarly:

**Proposition:** Let $$\cC$$ be a presentable stable $$\infty$$-category, and
let $$\cC_\fil$$ denote the category $$\Fun(\Z, \cC) = \cC\otimes \Sp_\fil$$.
The functor $$\cC_\fil\to \cC$$ sending a filtered object of $$\cC$$ to its
underlying object is given by tensoring with $$u_\ast \co_{\spec \S} \in
\QCoh(\AA^1/\GG_m) \simeq \Sp_\fil$$.

This result states that passing to the underlying non-filtered object is given
by ``inverting $$\tau$$''. Colloquially, the span

$$\cC\xleftarrow{\un = \tau^{-1}} \cC_\fil \xrightarrow{\gr = C\tau\otimes -}
\cC_\gr$$

is induced from the span
    
$$\spec \S \xrightarrow{u} \AA^1/\GG_m \xleftarrow{g} B\GG_m.$$

This philosophy can be made more precise: if $$X\in \cC_\fil$$, then $$\tau$$
induces a map $$X(-1)\to X$$. Then the first proposition asserts that there is
a symmetric monoidal equivalence $$\Mod_{C\tau}(\cC_\fil) \simeq \cC_\gr$$, and
the second proposition asserts that there is a symmetric monoidal equivalence
$$\cC_\fil(\tau^{-1}) \simeq \cC$$.

Here are some examples.

* Let $$\cC = \TCart_p$$ be the category of $$p$$-typical topological Cartier
modules (see [this paper](https://arxiv.org/abs/1809.01714)), i.e.,
$$S^1$$-spectra $$M$$ with an $$S^1$$-equivariant factorization
$$M_{hC_p}\xrightarrow{V} M \xrightarrow{F} M^{hC_p}$$ of the norm. The
Postnikov filtration on the underlying spectrum defines a $$t$$-structure on
$$\TCart_p$$ whose heart is the category of abelian groups equipped with
endomorphisms $$F$$ and $$V$$ such that $$FV = p$$. The process of tensoring
$$X\in \TCart_p$$ with $$\AA$$ amounts to sending $$X$$ to the generalized
Eilenberg-Maclane object $$\pi_\ast X$$. Note, however, that the $$S^1$$-action
on a $$p$$-typical topological Cartier module need not satisfy any
compatibility with the Postnikov filtration on its underlying nonequivariant
spectrum.
* Let $$E$$ be a homotopy commutative ring spectrum. The $$\infty$$-category
$$\Syn_E$$ of synthetic spectra is introduced in [this
paper](https://arxiv.org/abs/1803.01804). It is a presentable stable
$$\infty$$-category which is locally filtered via a natural $$t$$-structure.
There is an equivalence $$\Syn_E(\tau^{-1}) \simeq \Sp$$, and
$$\Mod_{C\tau}(\Syn_E)$$ is equivalent to Hovey's stable $$\infty$$-category of
$$E_\ast E$$-comodules if $$E$$ is Landweber exact.  Under the equivalence
between cellular $$\cc$$-motivic spectra and $$\Syn^\mathrm{even}_\MU$$ of
``even'' synthetic spectra, the map $$\tau^2: S^0(-2)\to S^0$$ corresponds to
the motivic map $$\tau:S^{0,-1}\to S^0$$.  Thanks to this example, the map
$$\tau$$ should be thought of as giving a theory of weights.

Related to this observation, we note that filtered compactly generated
symmetric monoidal stable $$\infty$$-categories admit slice filtrations. Recall
from Section 2 of [this paper](https://arxiv.org/abs/1012.3301) that if $$\cC$$
is a compactly generated symmetric monoidal stable $$\infty$$-category, then a
slice structure on $$\cC$$ is the data of a family

$$\cdots \subseteq \cC_{i+1} \subseteq \cC_i\subseteq \cdots \subseteq \cC_0\ni
\mathbf{1}$$

of full subcategories of $$\cC$$ such that:

* Each $$\cC_i$$ is closed under equivalences;
* $$\cC_i$$ is generated under colimits and extensions by a set $$K_i$$ of
compact objects;
* Each compact generator of $$\cC$$ is contained in some $$\cC_i$$.

The second statement allows one to characterize $$\cC_i$$ in terms of $$K_i$$:
for instance, if $$\cC = \Sp$$, one can let $$K_i = \{S^n | i\leq n\}$$ to
obtain a slice filtration. More generally: if $$\cC$$ is a filtered compactly
generated symmetric monoidal stable $$\infty$$-category, with a set
$$\{X_\alpha\}$$ of compact generators, let $$\cC_i\subseteq \cC$$ denote the
full subcategory generated under colimits and extensions by $$K_i =
\{X_\alpha(n) | i\leq n\}$$. Then $$\{\cC_i\}$$ forms a slice structure on
$$\cC$$. This deserves to be called the ``effective slice filtration'',
motivated by motivic homotopy theory. In general, it is not possible to define
an analogue of the very effective slice filtration.
