---
layout: post
title:  "Calculus and chromatic theory"
date:   2019-07-02
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
\newcommand{BP}{\mathrm{BP}} \newcommand{\QQ}{\mathbf{Q}}
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
\newcommand{\Sym}{\mathrm{Sym}} \newcommand{\coker}{\mathrm{coker}}$$

I'm currently at [UChicago](http://math.uchicago.edu/~may/REU2019/), working
with Mark Behrens and Peter May. It's incredibly fun. I talked with Mark today
for almost three and a half(!) hours about some really interesting stuff, and
I'd like to better understand some of the story he told me about. That's what
I'll try to do in this post. I don't want to get bogged down in details for now,
since I'm still trying to understand this stuff, so I'll try to explain the big
picture.

Let's begin with the EHP spectral sequence. This uses the fiber sequence
$$\Omega^{n+2} S^{2n+1}\to \Omega^n S^n \xrightarrow{E} \Omega^{n+1} S^{n+1}$$
to obtain a filtration of $$\Omega^\infty \S$$, and hence define a spectral
sequence with $$E_1^{k,n} = \pi_{n+k} S^{2n-1}$$ converging to $$\pi_k \S$$,
where the $$d_1$$-differentials go $$d_1:E_1^{k,n} \to E_1^{k-1,n-1}$$.  Since
Serre tells us that $$S^{2n-1}$$ is rationally just $$K(\QQ,2n-1)$$, this
spectral sequence collapses at the $$E_2$$-page.

Serre's result suggests that we can maybe instead try to use the double
suspension; this gets us a fiber sequence $$W_n \to S^{2n-1} \xrightarrow{E^2}
\Omega^2 S^{2n+1}$$, where $$W_n$$ is the fiber of the double suspension.
According to Serre, $$E^2$$ is a rational homotopy equivalence, so $$(W_n)_\QQ =
\ast$$. Consequently, we get a filtration $$S^1\to \Omega^2 S^3\to \Omega^4
S^5\to \cdots \to QS^1$$, and hence a spectral sequence with $$E_1^{k,n} =
\pi_{k+2n} W_n$$ converging to $$\pi_k \S$$ (if I've got the indexing right).
Since the $$E_1$$-page vanishes rationally, we should try to invert $$v_1$$.

One can define the $$v_1$$-periodic homotopy of a spectrum $$X$$ in the usual
manner: find a type $$1$$ spectrum $$Y$$ with a $$v_1$$-self map (preferably of
minimal periodicity for calculational purposes), and then define $$v_1^{-1}
\pi_\ast(X;Y)$$ to be $$v_1^{-1} [Y,X]_\ast$$. One can, of course, also
construct this stably. Now, the bottom two cells of $$W_n$$ (i.e., the
$$pn+1$$-skeleton of $$W_n$$, although we'll only work at the prime two because
that's what Mahowald does) for $$n\geq 1$$ form a copy of the mod $$2$$ Moore
space. Mahowald
[proved](https://web.math.rochester.edu/people/faculty/doug/otherpapers/Mahowald-ImJ.pdf)
that if $$Y = \S/2\wedge \S/\eta$$ (which has a $$v_1^1$$-self map), then this
induces an isomorphism (up to shift)

$$v_1^{-1} \pi_\ast(W_n;Y) = [Y, \Phi_1 W_n]_\ast \cong v_1^{-1}
\pi_\ast^s(\S/2;Y) = [Y, \Lone \S/2]_\ast.$$

Consequently, we get a $$v_1$$-periodic version of our spectral sequence defined
using the double suspension; this new spectral sequence has $$E_1$$-page
$$E_1^{\ast,\ast} = v_1^{-1} \pi_\ast^s(\S/2;Y)$$. In the same paper linked to
above, Mahowald showed that the map $$\Omega^{2n} S^{2n+1} \to \Omega^\infty
\Sigma^{\infty+1} \RP^{2n}$$ (given by the stable projection $$\Omega^{2n}
S^{2n+1}_+ \to \Sigma \RP^{2n}_+$$ coming from the Snaith splitting) is a
$$v_1$$-periodic isomorphism (i.e., is an isomorphism after applying the
Bousfield-Kuhn functor $$\Phi_1$$). The filtration of $$\Sigma^{\infty+1}
\RP^{2n}$$ corresponding to the double suspension filtration is exactly the
filtration of $$\RP^\infty$$ coming from its even-dimensional skeleta.

Here's where things start to get wild. In [this
paper](https://eudml.org/doc/173303), Cohen constructs a map $$W_n \to
\Omega^{2p} W_{n+1}$$ which is degree one on the bottom cell, and induces an
isomorphism in $$v_1$$-periodic homotopy. Let $$G_{n+1}$$ denote the fiber of
this map; then, the $$8n+1$$-skeleton of $$G_{n+1}$$ (which is its
$$8$$-skeleton) is actually a copy of $$A_1$$, our spectrum from
[earlier](/algebraic-topology/2019/06/11/A1.html)! Then, in [this
paper](https://www.jstor.org/stable/2374985), Mahowald and Thompson show that
there is a certain type $$2$$ spectrum $$M$$ for which there is a
$$v_2$$-periodic isomorphism (up to shift)

$$v_2^{-1} \pi_\ast(G_{n+1};M) = [M, \Phi_2 G_{n+1}]_\ast \cong v_2^{-1}
\pi_\ast^s(A_1;M) = [M, L_{T(2)} A_1]_\ast.$$

At this point, you should be convinced that whatever's going on is not a
coincidence. We should expect, for instance, that we can inductively define
spaces $$F_m(S^{2n-1})$$ (with $$F_0(S^{2n-1}) = S^{2n-1}$$, $$F_1(S^{2n-1}) =
W_n$$, and $$F_2(S^{2n-1}) = G_{n+1}$$) such there is a map $$F_m(S^{2n-1}) \to
\Omega^{2m} F_m(S^{2n+1})$$ (whose fiber is $$F_{m+1}(S^{2n-1})$$) which is an
isomorphism in $$v_{n+1}$$-periodic homotopy, and whose bottom skeleton has
cohomology which is free over $$A(m)$$ (at least when $$p=2$$). Proving such a
result is the goal of [this
paper](https://pdfs.semanticscholar.org/7b6d/b29d723424fc72d494a19d6c952c77eb276c.pdf)
of Arone's. It's a *very* dense paper...

In order to figure out what's going on in that paper, we need to take a slight
detour into Goodwillie calculus. I gave a talk about general properties of
Goodwillie calculus at Juvitop a [long time
ago](http://www.mit.edu/~sanathd/goodwillie.pdf). We will let $$\Top_\ast$$
denote the category of pointed spaces, and let $$\id$$ denote the identity on
this category. Let $$P_n$$ denote the associated Taylor tower, so $$P_1 =
\Omega^\infty \Sigma^\infty$$. If $$D_n$$ denotes the $$n$$th graded piece (the
$$n$$th derivative), then $$D_n(X) = \Omega^\infty (\partial_n \wedge
\Sigma^\infty X^{\wedge n})_{h\Sigma_n}$$ for some naive $$\Sigma_n$$-spectrum
$$\partial_n$$. Arone and Mahowald explicitly identified this
$$\Sigma_n$$-spectrum: let $$K_n$$ denote the quotient $$|\cP_n|/\partial
|\cP_n|$$, where $$|\cP_n|$$ is the geometric realization of the poset of
partitions of $$\{1,\cdots,n\}$$ ordered by refining the partition, and
$$\partial |\cP_n|$$ denotes the subcomplex that does not contain the boring or
trivial partition as vertices. Then $$\partial_n$$ is the Spanier-Whitehead dual
of the suspension spectrum of $$K_n$$.

They use this to show that $$(\partial_n \wedge S^{n(2k-1)})_{h\Sigma_n}$$ is
rationally contractible. (Note, for instance, that since $$P_1 = \Omega^\infty
\Sigma^\infty$$, it follows that an odd dimensional sphere $$S^{2k-1}$$ is
rationally equivalent to $$QS^{2k-1}$$.) In fact, they prove $$p$$-local
statements too: the mod $$p$$ homology of $$(\partial_n \wedge
S^{n(2k-1)})_{h\Sigma_n}$$ vanishes unless $$n$$ is a power of $$p$$. In fact,
$$(\partial_{p^n} \wedge S^{p^n(2k-1)})_{h\Sigma_{p^n}}$$ is equivalent to
$$\Sigma^{2k-1-n} L(n)_{2k-1}$$, where $$L(n)_m$$ is defined as the stable
summand $$e_n(B\FF_p^n)^{m\rho_n}$$, where $$e_n$$ is the Steinberg idempotent
in $$\Z_{(p)}[\GL_n(\FF_p)]$$, $$\rho_n$$ is the reduced real regular
representation of $$\FF_p^n$$, and $$(B\FF_p^n)^{m\rho_n}$$ is the associated
Thom spectrum.

One can even calculate the mod $$p$$ cohomology of these spectra: they find that
$$(\partial_{p^n} \wedge S^{p^n(2k-1)})_{h\Sigma_{p^n}}$$ is free over
$$A(n-1)$$. The spectra $$L(n)_0$$ and $$L(n)_1$$ are classical objects, which
have been well-studied. Using Nakaoka's theorem (see, e.g.,
[here](http://www.math.harvard.edu/~lurie/ThursdayFall2017/Lecture13-Symmetric-power.pdf)),
one can get a concrete grasp on the cohomology of these spectra. (We'll work at
$$p=2$$ for simplicity (I'm not as comfortable with the mod $$p$$ Steenrod
algebra).)

To describe its cohomology, we need to recall the Dold-Thom theorem: if $$\Sym
:= \Sym(\S)$$ denotes the infinite symmetric power of the sphere spectrum, then
$$\Sym = \H\Z$$. Let $$\Sym^n$$ be the $$n$$th symmetric power of the sphere
spectrum; then $$L(n)_1$$ can be shown to be $$\Sigma^{-n}
\Sym^{p^n}/\Sym^{p^{n-1}}$$. The Dold-Thom theorem gives a map $$\H^\ast(\H\Z)
\to \H^\ast(\Sym^{p^n})$$, which exhibits $$\H^\ast(\Sym^{p^n})$$ as the
quotient of the cohomology of $$\H^\ast(\H\Z)$$ (which is spanned by admissible
monomials in the Steenrod algebra not ending in $$\Sq^1$$) by the ideal
generated by the admissible monomials of length $$\geq n$$. In the notes linked
to above, Hopkins denotes this by $$F_n^\Z$$. Nakaoka's theorem implies that
$$\H^\ast(L(n)_1)$$ is isomorphic to (a shift of) $$\coker(F_{n-1}^\Z
\xrightarrow{\Sq^1} F_{n+1})$$, where $$F_{n+1}$$ denotes the quotient of
$$\H^\ast(\H\FF_p)$$ by the ideal generated by the admissible monomials of
length $$\geq n$$. As a vector space, $$\H^\ast(L(n)_1)$$ is isomorphic to the
sub-vector space of $$A$$ spanned by admissible monomials of length exactly
$$n$$ which do not end in $$\Sq^1$$.

How about $$L(n)_0$$? Define $$D(n)$$ to be the cofiber of the map
$$\Sym^{p^{n-1}}\to \Sym^{p^n}$$ sending $$\ul{s}$$ to $$(\ul{s}, \cdots,
\ul{s})$$; this is homotopic to the map $$\Sym^{p^{n-1}} \xrightarrow{p}
\Sym^{p^{n-1}} \hookrightarrow \Sym^{p^n}$$. Then $$L(n)_0 = \Sigma^{-n}
D(n)/D(n-1)$$. One use the description of the cohomology of $$\Sym^{p^n}$$ above
to be similarly explicit about the cohomology of $$L(n)_0$$: it is isomorphic as
a vector space to the sub-vector space of $$A$$ spanned by admissible monomials
of length exactly $$n$$. 

For instance, consider the spectrum $$L(1)_1$$. We can then write out basis
vectors of its cohomology: these are just $$\Sq^i$$ for $$i=0,i\geq 2$$. Drawing
out the Steenrod module structure using the Adem relations, we find that the
cohomology of $$L(1)_1$$ in degrees $$\geq 2$$ is exactly that of
$$\Sigma^{\infty+1} \RP^\infty$$; in fact, the quotient of $$L(1)_1$$ by its
$$0$$-cell is homotopy equivalent to $$\Sigma^{\infty+1} \RP^\infty$$. At odd
primes, one replaces $$\RP^\infty$$ with $$B\Sigma_p$$.

In any case, a theorem due to Miller-Wilkerson says that if $$M$$ is a connected
Steenrod module which is free over $$A(n)$$, then $$\Ext_A(M,\FF_p)$$ has a
vanishing line of slope less than $$1/|v_n|$$. Now, multiplication by a
$$v_n$$-self map will be given on the Adams spectral sequence by multiplication
by an element living on a line of slope $$1/|v_n|$$. So if $$m>n$$ and if $$V$$
is any type $$m$$ spectrum, then multiplication by $$v_m$$ on the mapping
spectrum $$\Map(V, (\partial_{p^n} \wedge S^{p^n(2k-1)})_{h\Sigma_{p^n}})$$ will
necessarily be trivial. As such, $$(\partial_{p^n} \wedge
S^{p^n(2k-1)})_{h\Sigma_{p^n}}$$ is $$K(m)$$-locally trivial for $$m>n$$.

What's the intuition supposed to be? A theorem of Ching's says that the
collection $$\{\partial_n\}$$ forms an operad in spectra, and in fact,
$$\{\H_{1-n}(\partial_n;\Z)\}$$ is the Lie operad from classical algebra. Since
there is a Goodwillie spectral sequence whose $$E_1$$-page is $$\pi_t(\partial_n
\wedge \Sigma^\infty X^{\wedge n})$$ (stable homotopy), abutting to
$$\pi_t(X)$$ (unstable homotopy), we find that the $$E_1$$-page of this spectral
sequence is built from Lie brackets --- which in the case of spheres correspond
to Whitehead products --- and power operations. If we rationalize and let $$X$$
be an odd sphere, for instance, there are no nontrivial power operations, and so
the $$E_1$$-page is just the free Lie algebra on one generator (in the dimension
of the sphere). Since this generator lives in odd degree, it has no nontrivial
Lie bracket/Whitehead product with itself, and we find that the $$E_1$$-page is
just a copy of $$\QQ$$ in the dimension of sphere. This recovers Serre's
calculation of the stable homotopy of odd spheres. (For even spheres, it's
slightly more complicated, because the Whitehead product of the identity with
itself is no longer rationally trivial, and we find that the $$E_1$$-page is
$$\QQ\{\iota_{S^{2n}}\} \oplus \QQ\{[\iota_{S^{2n}}, \iota_{S^{2n}}]\}$$.) The
fact that $$(\partial_{p^n} \wedge S^{p^n(2k-1)})_{h\Sigma_{p^n}}$$ is
$$K(m)$$-locally trivial for $$m>n$$ tells us that after inverting $$v_n$$, the
$$E_1$$-page of this spectral sequence is only concentrated in a few lines. By
our discussion above, this is a statement about (unstable) Lie brackets and
power operations in the $$K(n)$$-local setting. This is discussed in more detail
in Mark's [book](https://www3.nd.edu/~mbehren1/papers/GoodEHPmem.pdf), which I'm
hoping to better understand.

In any case, the upshot of this is that if $$X$$ is an odd-dimensional sphere,
the $$v_n$$-periodic Goodwillie spectral sequence only has $$n$$ layers (namely,
$$D_1(X)$$ through $$D_{p^n}(X)$$). So the (unstable) $$v_n$$-periodic homotopy
type of $$X$$ has a filtration whose associated graded is $$\bigoplus_{i=0}^n
D_{p^i}(X)$$; this is the same as the associated graded of the Goodwillie
derivative filtration of $$P_{p^n}(X)$$, and the map $$X\to P_{p^n}(X)$$ is in
fact a $$v_n$$-periodic homotopy equivalence. The idea of the proof of this
final claim is to write the fiber, say $$J_{p^n}(X)$$, of the map $$X\to
P_{p^n}(X)$$ as an inverse limit of a tower $$\{\ol{P}_{p^i}(X) =
\mathrm{fib}(P_{p^n}(X) \to P_{p^i}(X))\}$$, whose layers are each
$$D_{p^i}(X)$$ for $$i>n$$, and use the fact that multiplication by $$v_n$$ acts
on any element in $$\Map(V,J_{p^n}(X))$$ (where $$V$$ is a finite type $$n$$
spectrum) in the Adams spectral sequence by multiplication by an element living
in a slope higher than the vanishing line of the Adams spectral sequence for
$$\Map(V,D_{p^i}(X))$$. This argument is sketched as the proof of Theorem 3.6
on page 15 of [this survey](https://arxiv.org/pdf/1902.00803.pdf); it's clear
that the argument is rather general, and could be applied to other situations
too.

We can now return back to [the
paper](https://pdfs.semanticscholar.org/7b6d/b29d723424fc72d494a19d6c952c77eb276c.pdf)
of Arone's we originally wanted to understand. In all of this, we considered the
$$n$$th layer $$D_n(X)$$ of the Goodwillie spectral sequence for the identity on
pointed space, and finally concluded that only $$k$$ of them were nontrivial
after inverting $$v_k$$; this told us that $$X$$ is equivalent to $$P_{p^k}(X)$$
after inverting $$v_k$$. Mahowald's and Mahowald-Thompson's work that we talked
about in the beginning of this post suggests that trying to understand the
layers $$D_n F_m(X)$$ might suggest a generalization of the results we mentioned
at the very beginning of this post. To understand this, we need to actually
define $$F_m$$, and then study its layers. Cohen's definition of $$F_2$$ (on
spheres) involved hard calculations in unstable homotopy theory, but Weiss
observed that one can actually construct it in a lot more generality.

Let $$\cL$$ denote the category of complex vector spaces with a positive
definite inner product and isometries, and let $$G:\cL \to \Top_\ast$$ be a
functor. Let $$G_1(V)$$ denote the fiber of the map $$G(V) \to G(V\oplus \cc)$$.
Then Weiss showed that if $$W\in \cL$$, there is a functor $$G_1':\cL\to
\Top_\ast$$ defined on objects by $$G_1'(V) = \Omega^V G_1(V\oplus W)$$ such
that the obvious map $$G_1(V) \to G_1'(V)$$ lifts the map $$G_1(V) \to
G_1(V\oplus W)$$, where the map $$G_1'(V) \to G_1(V\oplus W)$$ is given by
evaluation on $$0\in V$$. If we now define $$G(V)$$ to be $$\Omega^V \Sigma^V
X$$ for some space $$X$$, then $$G_1(\{0\})$$ is the fiber $$F_1(X)$$ of the
double suspension map $$X\to \Omega^2 \Sigma^2 X$$. Moreover, $$G_1(\cc) =
\Omega^2 F_1(\Sigma^2 X)$$, so the result cited above says that there is a
natural map $$G_1(\{0\}) = F_1(X) \to \Omega^2 G_1(\cc) = \Omega^4 F_1(\Sigma^2
X)$$. When $$X$$ is the sphere $$S^{2d-1}$$ (which we'll always assume), then
$$F_1(X)$$ is $$W_d$$, and this map is precisely Cohen's map (at $$p=2$$).

Having obtained this map $$F_1(X) \to \Omega^4 F_1(\Sigma^2 X)$$, we inductively
define $$F_m(X)$$ to be the fiber of the induced map $$F_{m-1}(X) \to
\Omega^{2m} F_{m-1}(\Sigma^2 X)$$. In Weiss' original paper, it's shown that
$$D_n F_m(X)$$ is equivalent to $$\Omega^\infty(\partial_n \wedge \Sigma^\infty
X^{\wedge n} \wedge \Sigma^\infty_+ \U(n-1)/\U(n-m-1))_{h\Sigma_n}$$, where
$$\Sigma_n$$ is regarded as a subgroup of $$\U(n-1)$$ via the reduced standard
representation. Let's write this as $$\Omega^\infty \DD_n F_m(X)$$. The main
point of Arone's paper is to calculate the homology of $$\DD_n F_m(X)$$ when
$$X$$ is an odd-dimensional sphere --- he shows that it vanishes for $$n$$ not a
power of a prime, and, like for $$\partial_n\wedge \Sigma^\infty X^{\wedge n}$$,
it's free over $$A(k-1)$$ if $$n=p^k$$. In fact, he shows that it's the exactly
homology of $$\partial_{p^k} \wedge \Sigma^\infty X^{\wedge p^k}$$ tensored up
with the exterior algebra generated by the Chern classes of
$$\U(p^k-1)/\U(p^k-m-1)$$.

The argument used in the linked [survey](https://arxiv.org/pdf/1902.00803.pdf)
to show that $$X\to P_{p^n} X$$ is a $$v_n$$-periodic equivalence (when $$X$$ is
an odd sphere, which will remain true for the rest of this post) in fact applies
to this situation as well (as one can see from the sketch of the proof of
Theorem 3.6 on page 15, all one needs to ensure is true in this case is that the
cohomology of each layer is free over $$A_k$$ for $$k>n$$ (so you know the
vanishing line of its Adams $$E_2$$-page), and that the connectivity of the
mapping spectrum $$\Map(V,\DD_{p^i}(X))$$ is sufficiently large), and we find
that the map $$F_m(X) \to P_{p^n} F_m(X)$$ is a $$v_k$$-periodic equivalence for
$$k\leq n$$.  In fact, if $$n$$ is the smallest integer for which $$m < p^n$$
(so $$n = v_p(m)+1$$), then $$F_m(X)$$ has trivial $$v_k$$-periodic homotopy for
$$k < n$$ (because $$\DD_n F_m(X)$$ vanishes, by Weiss' formula, for $$n < m$$,
and hence $$P_{p^k} F_m(X)$$ does too for $$p^k < m$$). Moreover, since
$$P_{p^n} F_m(X) \simeq \Omega^\infty \DD_{p^n} F_m(X)$$ (again by Weiss'
formula and our choice of $$n$$ given $$m$$), we find that the map $$F_m(X) \to
\Omega^\infty \DD_{p^n} F_m(X)$$ is a $$v_n$$-periodic equivalence. In other
words, $$\Phi_n F_m(X) \simeq \Lk \DD_{p^n} F_m(X)$$.

Recall that Mahowald proved (in our notation) that $$\Phi_1 F_1(X)$$ is (a shift
of; remember, $$X$$ is an odd-dimensional sphere) $$\Lone \S/p$$. One can
apparently just calculate that $$\DD_p F_1(X) = (\partial_p \wedge \Sigma^\infty
X^{\wedge p} \wedge \Sigma^\infty U(p-1)/U(p-2))_{h\Sigma_p}$$ is just a shift
of $$\S/p$$, so our discussion above recovers Mahowald's result. Similarly,
Arone claims that Mahowald-Thompson's result also follows by a calculation. In
any case, it is clear that the "correct" generalization of Mahowald *et al*'s
results is given by Arone's theorem.
