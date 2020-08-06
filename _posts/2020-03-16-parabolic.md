---
layout: post
title:  "Moduli of parabolic subgroups"
date:   2020-03-16
categories: representation-theory
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
\newcommand{\Q}{\mathrm{Q}}$$

In this post, I'd like to talk about the moduli of parabolic subgroups of a
connected split semisimple algebraic group. What I'm writing here will appear in
the paper that I'm writing which I discussed
[here](/algebraic-geometry/2020/02/29/random.html).  Recall that if $$G$$ is a
reductive algebraic group over a field $$k$$, then the set of Borels in $$G$$ is
in bijection with $$(G/B)(k)$$, where $$B$$ is a fixed Borel in $$G$$ and
$$G/B$$ is the associated flag variety. The flag variety, which we'll denote
$$\cB$$ admits an action of $$G$$, and if $$T$$ is a maximal torus in $$G$$,
then the fixed points $$\cB^T$$ classifies Borels in $$G$$ containing $$T$$.

Here's the motivating question: fix a maximal torus $$T\subseteq G$$. Is there a
moduli stack classifying conjugacy classes of parabolic subgroups of $$G$$ which
contain $$T$$? The answer turns out to be yes, and it's actually a special case
of the construction $$\AA_\G/\GG_\G$$ described in [this
post](/algebraic-topology/2020/02/08/poset.html).

Let's work out the question in the universally simple example: $$G = \SL_2$$,
and $$T$$ is the usual diagonal subgroup in $$\SL_2$$. Then there are only three
conjugacy classes of parabolic subgroups containing $$T$$: the Borel $$B^+$$ of
upper triangular matrices, the Borel $$B^-$$ of lower triangular matrices, and
the entirety of $$\SL_2$$. There's a partial ordering on these parabolic
subgroups, given by inclusion: $$B^+\subseteq \SL_2 \supseteq B^-$$. (You could
sit down and try to explicitly work out what happens for $$\SL_3$$: you'd find
that there are $$13$$ conjugacy classes of parabolic subgroups in $$\SL_3$$. I
would not recommend doing this calculation.)

How do we understand parabolic subgroups? Let's first recall a result which sort
of reduces us to combinatorics. Fix a Borel subgroup $$B\subseteq G$$. Let
$$\XX^\bullet$$ (resp. $$\XX_\bullet$$) denote the lattice of weights (resp.
coweights), and let $$\XX^{\bullet,+}$$ (resp. $$\XX_\bullet^+$$) denote the
lattice of positive weights (resp. dominant coweights) determined by $$B$$. Let
$$\Delta$$ denote a set of simple roots, i.e., a base for the root system. Then
conjugacy classes of parabolic subgroups containing $$B$$ are in bijection with
subsets of $$\Delta$$. We can actually characterize the subsets of $$\Delta$$ in
terms of a certain partially ordered abelian group.


Equip $$\XX_\bullet^+$$ with the Bruhat ordering, so $$\mu_2\leq \mu_1$$ if
$$\mu_1 - \mu_2$$ is a sum of dominant coroots. Then, a simple combinatorial
exercise shows that faces of the monoid $$\XX_\bullet^+$$ are in bijection with
subsets of $$\Delta$$ (where "face" means the notion discussed in the [previous
post](/algebraic-geometry/2020/03/14/faces.html)). This is great: the main
result of the previous post shows that if $$\G$$ denotes the group completion of
$$\XX_\bullet^+$$, then the underlying space of $$\AA_\G/\GG_\G$$ is
homeomorphic (and in particular admits a bijection) to the set of faces of
$$\XX_\bullet^+$$.

In summary, if $$G$$ is a connected split semisimple group and $$B$$ is a chosen
Borel in $$G$$, then the underlying space of $$\AA_\G/\GG_\G$$ when $$\G$$ is
the group completion of $$\XX_\bullet^+$$ is in bijection with the set of
parabolic subgroups of $$G$$ containing the chosen Borel.

Aha! Now we can see what's going in the $$\SL_2$$ example. For each of the
Borels $$B^+$$ and $$B^-$$, there are only two parabolics in $$\SL_2$$
containing that Borel: the Borel itself, and the entirety of $$\SL_2$$. These
correspond to the closed point and the generic point of $$\AA^1/\GG_m$$. What,
then, corresponds to the moduli stack $$\cP$$ of parabolics containing a fixed
maximal torus $$T$$ (and not necessarily a chosen Borel)? In the case of
$$\SL_2$$, the moduli of parabolics containing $$T$$ should be obtained by
gluing two copies of $$\AA^1/\GG_m$$. Let's think about what's going on at the
level of underlying spaces. 

The stack $$\cP$$ is glued together from two copies of $$\AA^1/\GG_m$$. The
gluing is nontrivial: on the level of underlying spaces, $$\AA^1/\GG_m$$ is
$$\cf(\Z_{\geq 0})$$, and the underlying space of $$\cP$$ is obtained by gluing
two copies of $$\cf(\Z_{\geq 0})$$ along $$\cf(\Z)$$, where the gluing is
determined by the diagram

$$\XX_\bullet(B^+)^+ = \Z_{\geq 0} \xrightarrow{n\mapsto n} \Z =
\XX_\bullet(B^\pm)^{+,\mathrm{gp}} \xleftarrow{n\mapsto -n} \Z_{\geq 0} =
\XX_\bullet(B^-)^+.$$

In other words, the underlying space of $$\cP$$ is the underlying space of
$$\PP^1/\GG_m$$ --- it contains three points, two of which are closed, and the
third of which is a generic point. These points correspond to the two Borel
subgroups of $$\SL_2$$, and the entirety of $$\SL_2$$ itself (there are no other
parabolic subgroups). In fact, when $$G = \SL_2$$, the stack $$\cP$$ to be
defined below is $$\PP^1/\GG_m$$ itself.

For a general connected split semisimple group $$G$$, a construction of the
"parabolic stack" $$\cP$$ was provided by
[Procesi](http://www1.mat.uniroma1.it/people/procesi/toric-varietyWeyl.pdf) and
[Dolgachev-Lunts](https://www.sciencedirect.com/science/article/pii/S0021869384712518).
We begin by recalling a general procedure for gluing the stacks
$$\AA_\G/\GG_\G$$ in a certain special case. Let $$(\Sigma, N)$$ be a fan.  For
each cone $$\sigma\in \Sigma$$, let $$S_\sigma$$ denote the monoid
$$\{\lambda\in N^\vee \text{ such that } \lambda|_\sigma \geq 0\}$$. There is an
associated spectral affine scheme $$\AA_{S_\sigma} = \spec \S[S_\sigma]$$ and an
associated group scheme $$\GG_{S_\sigma} = \spec \S[S_\sigma^\gp]$$ acting on
$$\AA_{S_\sigma}$$. If $$\sigma, \tau\in \Sigma$$ are cones such that $$\tau$$
is a face of $$\sigma$$, then $$S_\tau$$ is obtained by localizing $$S_\sigma$$
at the face $$\{\lambda\in S_\sigma \text{ such that } \lambda|_\tau = 0\}$$. It
follows that there is an open immersion $$\AA_{S_\tau} \to \AA_{S_\sigma}$$
which is equivariant for the action of $$\GG_{S_\tau}$$. Just as in with
classical toric varieties, the data of the inclusions of cones in the fan
$$(\Sigma, N)$$ specify the data necessary to glue the resulting stacks
$$\AA_{S_\sigma}/\GG_{S_\sigma}$$ to form a stack $$\AA_\Sigma/\GG_\Sigma$$.

Similarly, we may associate the space $$\cf(S_\sigma)$$ to each cone $$\sigma\in
\Sigma$$, and the data of the inclusions of cones in the fan $$(\Sigma, N)$$
specify the data necessary to glue the spaces $$\cf(S_\sigma)$$ to form a space
$$\cf(\Sigma)$$.  These constructions are functorial in the fan $$(\Sigma, N)$$:
if $$(\Sigma, N)\to (\Sigma', N')$$ is a morphism of fans, then there is an
induced morphism $$\AA_{\Sigma'}/\GG_{\Sigma'}\to \AA_\Sigma/\GG_\Sigma$$ of
stacks and an induced morphism $$\cf(\Sigma')\to \cf(\Sigma)$$ of spaces.
Moreover, the theorem in [this post](/algebraic-geometry/2020/03/14/faces.html)
implies that the underlying space of the stack $$\AA_\Sigma/\GG_\Sigma$$ is
homeomorphic to $$\cf(\Sigma)$$.

Here's the variation on Procesi's and Dolgachev-Lunts' construction. Let
$$(V,R)$$ be a root system, and let $$\Q(R) = \Z\{R\}$$ denote the root lattice
of $$R$$. Let $$(\Sigma(R), \Q(R))$$ denote the fan where $$\Sigma(R)$$ consists
of the Weyl chambers of the dual root system $$R^\vee$$ and their faces. Define
$$\cP_{(V, R)}$$ to be the stack associated to the fan $$(\Sigma(R), \Q(R))$$
via the above construction. If $$(\XX^\bullet_\RR, \Phi)$$ is the root system
associated to a connected split reductive group $$G$$ and a maximal torus
$$T\subseteq G$$, then let $$\cP_G$$ denote the stack $$\cP_{(\XX^\bullet_\RR,
\Phi)}$$. When it is clear, we simply write $$\cP$$ to denote $$\cP_G$$. 

Note that since the Weyl group $$W(R)$$ of a root system $$(V, R)$$ acts on
$$R$$, there is an action of $$W(R)$$ on $$\cP_{(V,R)}$$. In particular, if
$$W$$ denotes the Weyl group associated to a connected split reductive group
$$G$$ and a maximal torus $$T$$, then there is an action of $$W$$ on $$\cP$$.

For instance, if $$G$$ is a connected split semisimple group, $$T$$ is a maximal
torus, and $$B$$ is a Borel of $$G$$ containing $$B$$, then the toric variety
$$X(R)$$ associated to the root system of $$G$$ via Procesi's and
Dolgachev-Lunts' construction admits an action of $$\GG_\G$$ (where, as usual,
$$\G = \XX_\bullet^{+,\gp}$$); the underlying stack of $$\cP$$ is the stacky
quotient $$X(R)/\GG_\G$$.

Observe that the underlying space of $$\cP$$ is homeomorphic to $$\cf(\Sigma)$$.
The space $$\cf(\Sigma)$$ is obtained by gluing $$\cf(S_\sigma)$$ for each face
$$\sigma$$ of a Weyl chamber, where $$S_\sigma$$ is defined as in the above
construction. If $$\sigma$$ is a Weyl chamber of the root system $$(V, R) =
(\XX^\bullet_\RR, \Phi)$$ corresponding to a Borel subgroup $$B\subseteq G$$
containing $$T$$, then a face of $$\sigma$$ corresponds to a conjugacy class of
parabolic subgroups of $$G$$ containing $$B$$. More precisely, for each Weyl
chamber $$\sigma$$, there is a morphism $$\AA_\G/\GG_\G\to \cP$$; the underlying
space of $$\AA_\G/\GG_\G$$ is homeomorphic to $$\cf(S_\sigma)$$, and hence by
the above discussion, points of $$\cf(S_\sigma)$$ are conjugacy classes of
parabolic subgroups of $$G$$ which contain the Borel corresponding to the Weyl
chamber $$\sigma$$.  A common face of two Weyl chambers corresponds to a
parabolic subgroup containing the Borel subgroups associated to the Weyl
chambers. It is in this sense that when $$G$$ is a connected split semisimple
group, points of $$\cP$$ correspond to conjugacy classes of parabolic subgroups
of $$G$$ which contain the maximal torus $$T$$.

Let's end with the following. Let $$\cP$$ denote the stack associated to a
connected split semisimple group $$G$$ and a choice of maximal torus. Let $$W$$
denote the Weyl group, and let $$(\XX^\bullet_\RR, \Phi)$$ denote the associated
root system. Then, the number of points in the underlying space $$|\cP|$$ of the
stack is given by the number of elements in the Coxeter complex of type
$$(\XX^\bullet_\RR, \Phi)$$. For instance, if $$G = \SL_{n+1}$$, then the number
of points in $$\cP_{\SL_{n+1}}$$ is given by the $$n$$th Fubini number:

$$|\cP_{\SL_{n+1}}| = \sum_{i=0}^n \sum_{j=0}^i (-1)^{i-j} \binom{i}{j} j^n.$$

For instance, $$|\cP_{\SL_2}| = 3$$, $$|\cP_{\SL_3}| = 13$$, and $$|\cP_{\SL_4}|
= 75$$. That's how we got the count at the beginning of the post.
