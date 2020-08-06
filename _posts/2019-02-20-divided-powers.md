---
layout: post
title:  "Divided powers and the sphere spectrum"
date:   2019-02-20
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
\newcommand{\top}{\mathrm{top}} \newcommand{\der}{\mathrm{der}}$$

Divided power rings play a pretty prominent role in a bunch of areas of math.
For example, it's used to define crystalline cohomology, which (after inverting
the implicit prime) provides an example of a Weil cohomology theory; [related to
this](https://arxiv.org/abs/1802.03261), it shows up when studying the
Hochschild homology of finite fields; and related to this, it naturally comes
up when studying the cohomology of loop spaces. One natural reason why divided
powers come up so often in algebraic topology is because the dual of a
polynomial algebra in one generator, regarded as a bialgebra by letting its
generator be primitive, is a divided power algebra. In algebraic geometry, the
appearance of divided powers in crystalline cohomology is morally justified
essentially because of Berthelot's de Rham-crystalline comparison theorem.

Let's recall the definition of divided powers. Let $$A$$ be a ring and $$I$$ an
ideal. Then a divided power structure on $$I$$ is a collection of maps
$$\{\gamma_n: I \to I\}$$ that's roughly supposed to send $$x$$ to
"$$x^n/n!$$"; we won't write down the axioms, but two important properties that
are required are:

$$\gamma_n(x)\gamma_n(x) = \binom{m+n}{m} \gamma_{m+n}(x), \text{ and }
\gamma_n(x+y) = \gamma_n(x) + \gamma_n(y) + \sum_{i=1}^{n-1}
\gamma_i(x)\gamma_{n-i}(y).$$

For instance, if $$A$$ is a DVR of mixed characteristic $$(0,p)$$, then the
maximal ideal of $$A$$ admits a divided power structure if and only if the
ramification index $$e$$ is at most $$p-1$$; this is not hard to prove using
the classical calculation of the $$p$$-adic valuation of $$n!$$. In particular,
the ideal $$(p)$$ inside $$\Z_p$$ admits a divided power structure, since
$$p^n/n!\in \Z_p$$.

In basic algebraic topology, one source of divided power algebras comes from
the cohomology of loop spaces of spheres. Let $$\Gamma[x]$$ denote the divided
power polynomial algebra on one generator (i.e.,
$$\Z[x_1,x_2,\cdots]/\left(\binom{m+n}{n} x_{m+n} = x_m x_n\right)$$) and
$$\Lambda(x)$$ the exterior algebra on one generator; then, a classical
computation with the Serre spectral sequence shows that

$$\H^\ast(\Omega S^n) = \begin{cases}
\Gamma[x_{n-1}] & \text{ if }n\equiv 1\pmod{2}\\
\Lambda(x_{n-1}) \otimes \Gamma[y_{2(n-1)}] & \text{ else}.
\end{cases}$$

Here, the degrees of the generators are given in the subscripts. The reason for
this is essentially due to the fact mentioned above about divided power
algebras being dual to polynomial algebras, and that $$\H_\ast(\Omega S^n)
\cong \Z[x_{n-1}]$$ as bialgebras, where the generator $$x_{n-1}$$ is
primitive.

Things get a bit wonky in positive characteristic, though: by induction, we can
prove that in $$\Gamma[x]$$, we may identify $$x_n = x^n/n!$$. We then conclude
that if $$p=0$$ in a base field $$k$$, we'd have $$x^p = 0$$. In fact, it's not
hard to show that the divided power algebra is $$\Gamma[x]\otimes k \cong
k[x_1,x_p,\cdots]/(x_1^p, x_p^p, \cdots)$$. That doesn't look very nice...

Let's trudge on anyway. I mentioned above that you can also get a divided power
algebra by studying the Hochschild homology of a finite field, so let's do
that. We'll do an explicit calculation: recall that the Hochschild homology of
a commutative ring $$R$$ is equivalent to the (everywhere derived) tensor
product $$R\otimes_{R\otimes R} R$$, so if we'd want to compute the Hochschild
homology of $$\FF_p$$, our first task would be to compute the derived tensor
product $$\FF_p\otimes \FF_p$$. To do this, we'd need to resolve $$\FF_p$$ as a
commutative DGA, but this is easy: we can just use $$\Z[t]/t^2$$, where $$\d t
= p$$ and $$|t| = 1$$. Our task is then reduced to understanding
$$\FF_p\otimes_{\Z[t]/t^2} \FF_p$$.  We can now resolve $$\FF_p$$ as a
$$\Z[t]/t^2$$-algebra by considering the divided power algebra
$$A[x_1,x_2,\cdots]/\left(\binom{m+n}{n} x_{m+n} = x_m x_n\right)$$, where $$A
= \Z[t]/t^2$$, $$|x_n| = 2n$$, and $$\d x_n = tx_{n-1}$$. Base-changing this up
to $$\FF_p$$ shows that the Hochschild homology of $$\FF_p$$ is a commutative
DGA which is quasi-isomorphic to its homology.

As I said before, this appearance of divided powers in characteristic $$p$$ is
sort of pathological, and we'd like to resolve this. A philosophy that's been
becoming more prevalent recently is that the existence of divided powers is
because one's working with $$\H\Z$$ as the base; if one instead regards the
sphere spectrum as one's base, then the divided power pathology vanishes. Let's
see this concretely in the case of Hochschild homology.

The topological Hochschild homology of an $$\E_\infty$$-ring $$A$$ is the smash
product $$A\wedge_{A\wedge A} A$$, so we'd like to understand what happens when
$$A = \H\FF_p$$. See
[here](https://mathoverflow.net/questions/320190/revisiting-thh-mathbbf-p). We
first need to understand $$\H\FF_p\wedge \H\FF_p$$. A theorem of Hopkins and
Mahowald's says that $$\H\FF_p$$ is the free $$p$$-local $$\E_2$$-algebra with
a nullhomotopy of $$p$$, i.e., $$\H\FF_p$$ is the smash product $$S^0
\otimes_{\F_{\E_2}(x)} S^0$$, where one of the maps to $$S^0$$ sends $$x$$ to
$$p$$, and the other sends $$x$$ to zero. We know that $$\H\FF_p\wedge
\H\FF_p$$ is therefore the free $$\E_2$$-$$\H\FF_p$$-algebra with $$p=0$$.
After smashing the entire diagram with $$\H\FF_p$$ and taking the colimit, we
obtain $$\H\FF_p\wedge_{\F_{\E_2\text{-}\H\FF_p}(x)} \H\FF_p$$, where the maps
$$\F_{\E_2\text{-}\H\FF_p}(x)\to \H\FF_p$$ are the augmentations. It follows
that the smash product above is $$\F_{\E_2\text{-}\H\FF_p}(\Sigma x)$$. Using
the bar construction, we find that the pushout $$\mathrm{THH}(A) =
\H\FF_p\wedge_{\F_{\E_2\text{-}\H\FF_p}(\Sigma x)} \H\FF_p$$ is
$$\F_{\E_1\text{-}\H\FF_p}(\Sigma^2 x)$$. The homotopy groups of this object is
exactly $$\pi_\ast(\H\FF_p\wedge \Omega S^3) \cong \H_\ast(\Omega S^3; \FF_p)
\cong \FF_p[u_2]$$. The canonical map $$\pi_\ast\mathrm{THH}(\H\FF_p) \to
\mathrm{HH}_\ast(\FF_p)$$ sends $$u_2$$ to the element denoted $$x_1$$ above.

Morally speaking, why does working over the sphere resolve the issue of divided
powers? The unit map $$S^0 \to \H\Z$$ is the group-completion of the map
$$\mathrm{FinSet}_\simeq \to \mathbf{N}$$ of monoids in spaces, and this map
quotients out symmetric groups; taking symmetric quotients is like working with
divided powers. This might not be a satisfactory explanation, so let's try for
another. 

One philosophy adopted in chromatic homotopy theory is that the sphere spectrum
should be the global sections of some sheaf of $$\Eoo$$-ring spectra on the
moduli stack $$\Mfg$$ of formal groups. In particular, a natural algebraic
approximation to the sphere spectrum is $$\Mfg$$; so instead of considering the
derived tensor product $$\FF_p\otimes_{\FF_p\otimes_\Z \FF_p} \FF_p$$, let us
consider the fiber product $$\spec \FF_p\times^\mathbf{L}_{\spec \FF_p
\times_{\Mfg} \spec \FF_p} \spec \FF_p$$. Let's specialize to the case when
$$p=2$$; then, $$\spec \FF_2 \times_{\Mfg} \spec \FF_2 \cong \Aut(\hat{\GG}_a)
\cong \spec A_\ast$$, where the last isomorphism was discussed in the beginning
of [this post](/chromotopy/2019/02/14/the-cusp.html). In particular, $$\spec
\FF_2\times^\mathbf{L}_{\spec \FF_2 \times_{\Mfg} \spec \FF_2} \spec \FF_2
\cong \mathrm{Tor}_{A_\ast}(\FF_2, \FF_2) \cong \Lambda_{\FF_2}[\sigma \zeta_1,
\sigma \zeta_2, \cdots]$$, where $$|\sigma \zeta_n| = |\zeta_n| + 1 = 2^n$$;
this is the $$E_2$$-page of the Kunneth spectral sequence for
$$\mathrm{THH}(\H\FF_2)$$. (More precisely, the algebra above is generated by
$$I/I^2$$, where $$I$$ is the augmentation ideal of the dual Steenrod algebra.)
You could do this at any odd prime, too, and you'd still get an exterior
algebra. I'm not sure if one should consider this to be "pathological" in the
same way that the ordinary Hochschild homology of $$\FF_p$$ is pathological:
the Kunneth spectral sequence degenerates at the $$E_2$$-page, and the only
data required to solve the extension problems is precisely the data of the
Dyer-Lashof operations (for instance, $$Q^2(\zeta_1) = \zeta_2$$, so the
generator $$\sigma \zeta_1$$ should square to $$\sigma \zeta_2$$).

We can run this argument more generally by replacing $$\spec \FF_2$$ with
$$\spec \pi_0 A$$ for any Landweber-exact even-periodic $$\Eoo$$-ring $$A$$.
Suppose that $$\GG$$ is the associated formal group over $$\spec \pi_0 A$$;
then, the fiber product $$\spec \pi_0 A\times^\mathbf{L}_{\spec \pi_0 A
\times_{\Mfg} \spec \pi_0 A} \spec \pi_0 A$$ is isomorphic to $$\spec \pi_0
A\times^\mathbf{L}_{\Aut_{\pi_0 A}(\GG)} \spec \pi_0 A$$. This is the derived
loop space $$L\Aut_{\pi_0 A}(\GG)$$ (in the sense of *derived*, not spectral,
algebraic geometry) of the $$\pi_0 A$$-group scheme $$\Aut_{\pi_0 A}(\GG)$$.
The global sections of this derived stack over $$\pi_0 A$$ is the $$E_2$$-page
of the Kunneth spectral sequence computing $$\mathrm{THH}(A)$$; the difference
between $$L\Aut_{\pi_0 A}(\GG)$$ and $$\mathrm{THH}(A)$$ is precisely the
difference between $$L\Aut_{\pi_0 A}(\GG)$$ and the spectral loop space
$$L\Aut_A(\wt{\GG})$$, where $$\wt{\GG}$$ is the spectral formal group living
over $$A$$.

Let's look at another natural source of divided powers: the representation
theory of the additive group scheme $$\GG_a$$. Since $$\GG_a \cong \spec
\Z[x]$$, we find that representations of $$\GG_a$$ are equivalent to comodules
over $$\Z[x]$$, which in turn are equivalent to modules over the divided power
ring $$\Gamma_\Z[x]$$. Given this, one might ask: what are the representations
of the "spectral additive group"?

There are two different notions of what one might mean by the phrase "spectral
additive group". Let's first consider the spectral affine line (because the
underlying scheme of the additive group is the affine line). In the classical
world, the affine line $$\AA^1_R$$ over a discrete ring $$R$$ is defined as
$$\spec$$ of the polynomial ring $$R[x]$$ in one generator. In the spectral
setting, a natural replacement for the polynomial ring over an $$\Eoo$$-ring
$$R$$ might therefore be the free $$\Eoo$$-ring $$R\{x\}$$ on one generator. We
almost immediately run into issues: the free $$\Eoo$$-ring on one generator is
not flat over $$R$$; in fact, it'll be flat if and only if $$R$$ is a
$$\QQ$$-algebra.

Let's make a brief digression. In the classical setting, a map $$X\to Y$$ is
smooth if, Zariski-locally, it admits an etale cover by affine space. In the
spectral setting, one might want to imitate this definition. Since there is a
reasonable definition of etaleness, and the phrase "Zariski locally" makes
sense, we only need to decide on a definition of affine space. In particular,
the notion of smoothness resulting from using the free $$\Eoo$$-ring as the
affine line, termed "differentially smooth" by Lurie, does not reduce to the
classical definition in the discrete case (so, for example, $$\PP^1_R$$ is not
differentially smooth when $$R$$ is discrete). Moreover, $$\pi_0 R\{x\}$$ need
not look like a polynomial ring on one generator over $$\pi_0 R$$. This
suggests a natural replacement: there is an $$\Eoo$$-ring $$\Sigma^\infty_+
\mathbf{N}$$, and we can define this to be a polynomial ring $$S[t]$$ over the
sphere spectrum. Working with the resulting notion of smoothness ("fiber
smoothness") affords a lot of rigidity not available with differentially smooth
morphisms.

The upshot of the above discussion is that we have two different candidates for
the spectral affine line: $$\AA^1_\top = \spec S^0\{x\}$$ and $$\AA^1_\der =
\spec \Sigma^\infty_+ \mathbf{N}$$. Both admit the structure of group schemes,
so we'll denote these group schemes by $$\GG_a^\top$$ and $$\GG_a^\der$$. We
can then consider representations of these algebraic groups. Representations of
$$\GG_a^\der$$ are the same as modules over the dual of the $$\Eoo$$-algebra
$$\Sigma^\infty_+ \mathbf{N}$$. By the discussion in Section 1.4
[here](http://www.math.harvard.edu/~lurie/papers/Elliptic-II.pdf), these are
the same as modules over the free smooth coalgebra over the sphere spectrum on
one generator. This is a flat $$S^0$$-algebra $$A$$ such that $$\pi_0 A \cong
\Gamma_\Z[x_0]$$.

Let's now instead consider representations of $$\GG_a^\top$$. These are the
same as modules over the dual of the $$\Eoo$$-algebra $$S^0\{x\}$$. By the
Barratt-Priddy-Quillen theorem, $$S^0\{x\} \cong \coprod_{n\geq 0} B\Sigma_n$$
(where $$B\Sigma_n$$ really means the unpointed supension spectrum). Since
$$B\Sigma_n = S^0_{h\Sigma_n}$$, we find that the dual of $$S^0\{x\}$$ is
$$\prod_{n\geq 0} (S^0)^{h\Sigma_n}$$. This *a priori* has nothing to do with
divided powers, but it's also just a hopelessly unapproachable object. To
attempt to understand this beast, let's $$K(n)$$-localize the entire situation
(for some implicit prime $$p$$ and a fixed height $$n$$), and consider the
$$K(n)$$-local dual of $$L_{K(n)} (S^0\{x\}) \simeq (L_{K(n)} S^0)\{x\} =:
L_{K(n)} S^0\{x\}$$. By the discussion above, we are reduced to understanding
the $$K(n)$$-local dual of $$L_{K(n)} B\Sigma_m$$ for all integers $$m$$. 

We claim that the $$K(n)$$-local dual of $$L_{K(n)} B\Sigma_m$$ is equivalent
to $$L_{K(n)} B\Sigma_m$$. A consequence of the classical work of [Hovey and
Sadofsky](https://www.ams.org/journals/proc/1996-124-11/S0002-9939-96-03495-8/S0002-9939-96-03495-8.pdf)
and Example 5.1.10 of [Hopkins and
Lurie](http://www.math.harvard.edu/~lurie/papers/Ambidexterity.pdf) is that the
$$K(n)$$-local Spanier-Whitehead dual of $$L_{K(n)} B\Sigma_m$$ is equivalent
to a shift of $$L_{K(n)} B\Sigma_m$$ by an element of the Picard group of
$$L_{K(n)} \mathrm{Sp}$$. Let's not bother ourselves with this Picard shift
(see [here](https://arxiv.org/pdf/math/0502184.pdf), though); then, we find
that the $$K(n)$$-local Spanier-Whitehead dual of $$L_{K(n)} S^0\{x\}$$ is
equivalent to the infinite product $$\prod_{m\geq 0} L_{K(n)} B\Sigma_m$$. In
fact, I think that the "$$K(n)$$-local divided power algebra" given by the
Spanier-Whitehead dual of $$L_{K(n)} S^0\{x\}$$ is equivalent to the completion
of $$L_{K(n)} S^0\{x\}$$ at the ideal generated by $$(x)$$; see Example 3.14
[here](https://arxiv.org/pdf/math/0306098.pdf).

This is very much analogous to the situation involving divided power algebras
in characteristic zero: in this case, we can simply divide by $$n!$$, so the
free divided power algebra $$\Gamma_k[x]$$ over a field of characteristic $$k$$
is simply the polynomial algebra $$k[x]$$. There's no pathological behavior
here! The upshot of this entire discussion is that if we regard "divided
powers" as arising via duals of polynomial algebras, then upon passing to the
sphere spectrum, there should be no distinction between divided powers and free
$$\Eoo$$-algebras at all the "finite primes" of $$S^0$$; the only divergence
occurs at the "infinite prime" $$(p,v_1,v_2,\cdots)$$.
