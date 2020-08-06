---
layout: post
title:  "Exponential sums"
date:   2019-12-22
categories: algebraic-geometry
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
\newcommand{\AA}{\mathbf{A}} \newcommand{\Frob}{\mathrm{Frob}}$$

In the [last post](/number-theory/2019/12/18/cubes.html), I talked about one of
the projects I worked on for 18.821 this semester. In this post, I'd like to
talk about another one, which I worked on under Roman Bezrukavnikov. Most of
this stuff only uses elementary algebraic geometry. The interested reader should
also consult
[Eisenbud-Harris](https://scholar.harvard.edu/files/joeharris/files/000-final-3264.pdf)
and [Roman's MathOverflow
question](https://mathoverflow.net/questions/290939/varieties-with-no-new-cohomology-in-hyperplane-sections).

Let $$p$$ be a prime number, and let $$V$$ be a $$\FF_p$$-vector space. For any
$$\lambda\in V^\ast$$ and primitive $$p$$th root of unity $$\zeta_p$$, the
function $$V\to \cc^\times$$ defined by $$v\mapsto \zeta_p^{\lambda(v)}$$
defines an additive character of $$V$$. Consequently, one may define the Fourier
transform $$\Phi_f$$ of a function $$f:V\to \cc$$ to be the function $$\Phi_f:
V^\ast\to \cc$$ given on any $$\lambda\in V^\ast$$ by

$$\Phi_f(\lambda) = \sum_{v\in V} \zeta_p^{\lambda(v)} f(v).$$

Our goal in this project was to study some properties (such as independence of
$$\lambda$$ for generic $$\lambda$$ and bounds on $$\Phi_f(\lambda)$$) of the
Fourier transform of special functions in this context.

We can rewrite this problem in language that makes it more amenable to
approaches from algebraic geometry. Let $$k$$ be a finite field of
characteristic $$p>0$$, and fix an embedding $$k \hookrightarrow \cc^\times$$.
Let $$V \cong k^{n+1}$$ be an $$(n+1)$$-dimensional $$k$$-vector space. Under
the chosen embedding of $$k$$ into $$\cc^\times$$, any linear functional
$$\lambda:\AA^{n+1}_k(k)\to k$$ on the $$(n+1)$$-dimensional $$k$$-vector space
$$V = \AA^{n+1}_k(k)$$ defines a function $$\psi_\lambda:V\to \cc^\times$$.

Here's an example. Let $$f$$ be the characteristic function of an
$$m$$-dimensional linear subspace $$W$$ of $$V$$. Then the Fourier transform of
$$f$$ at $$\lambda$$ is $$0$$ unless the restriction of $$\lambda$$ to $$W$$ is
$$0$$, in which case it is $$\# W = q^m$$. Indeed, the Fourier transform is
given on any $$\lambda \in V^\ast$$ by the sum over all elements of $$W$$ of the
additive character $$\psi_{\lambda|_W}$$, but the sum over all elements of an
abelian group of an additive character defined on the abelian group vanishes
unless the character is trivial.

In the general case, the problem of understanding the Fourier transform of
characteristic functions of conical subsets of affine space may be rewritten as
follows. Let $$X\subseteq \PP(V)$$ be a projective variety. Denote by
$$C_X\subseteq \AA^{n+1}_k$$ the affine cone on $$X$$, so that $$C_X = \{0\}\cup
\pi^{-1}(X)$$, where $$\pi:\AA^{n+1}_k-\{0\}\to \PP(V)$$ is the canonical
projection. Any functional $$\lambda\in V^\ast$$ restricts to a function on
$$C_X(k) \subseteq V$$, which in turn defines a function $$\psi_\lambda:X(k)\to
\cc^\times$$. Let $$f:V\to \cc$$ denote the characteristic function of
$$C_X(k)$$. The Fourier transform $$\Phi_f:V\to \cc$$ from the dual space
$$V^\ast = \Hom_k(V, k)$$ of $$V$$ then sends $$\lambda\in V^\ast$$ to

$$ \Phi_f(\lambda) = \sum_{x\in C_X(k)} \psi_\lambda(x) =: \FT_X(\lambda).$$

This is exactly the Fourier transform of the characteristic function of
$$C_X(k)\subseteq V$$. To emphasize the dependence on $$X$$, we have denoted the
sum (as indicated above) by $$\FT_X(\lambda)$$. Our goal in this project may
therefore be restated as the study of $$\FT_X$$ for various projective varieties
$$X$$.
The vanishing locus of any $$\lambda\in V^\ast$$ defines a hyperplane
$$H_\lambda \subseteq \PP^n_k$$. Then, for any $$\lambda\in \PP^n_k$$, we have

$$\FT_X(\lambda) = 1 + \#k\cdot \#(X \cap H_\lambda)(k) - \# X(k),$$

where $$X\cap H_\lambda$$ denotes the set-theoretic intersection of $$X$$ with
the hyperplane $$H_\lambda$$.
To see this, recall that $$C_X = \{0\}\ \cup\ \pi^{-1}(X)$$. Since $$\lambda$$
vanishes at $$0$$, we find that the sum defining $$\FT_X$$ can be rewritten as:

$$\FT_X(\lambda) = 1 + \sum_{x\in X(k)} \sum_{a\in \pi^{-1}(\{x\})}
\psi(a).$$

The fiber of any point $$x$$ in $$\PP^n_k$$ consists of $$k$$-points in
$$\AA^{n+1}_k - \{0\}$$ which lie on a line (namely, the line defined by $$x$$),
and the function $$\psi$$ on this line is an additive character. The sum of all
the values of an additive character $$\psi$$ over a finite abelian group vanish
unless $$\psi$$ is trivial, in which case it is the order of the group.
Therefore, the sum $$\sum_{a\in \pi^{-1}(\{x\})} \psi(a)$$ vanishes for $$x\in
X(k)$$ unless $$\psi$$ vanishes on the line defined by $$x$$, in which case the
sum is $$\#k$$. The condition that $$\psi$$ vanish on the line defined by $$x$$
is precisely the statement that $$x$$ be a $$k$$-point of the intersection
$$X\cap H_\lambda$$. This yields the claim.

We'll be interested in the following question: when is $$\#(X\cap
H_\lambda)(k)$$, and hence $$\FT_X(\lambda)$$, independent of $$\lambda$$ for
generic $$\lambda$$? One would like to apply the Weil conjectures to answer this
question, but in order to do so, the hyperplane section $$X\cap H_\lambda$$ must
a smooth projective variety. Even if $$X$$ is smooth, this hyperplane section
will not always be smooth, since the hyperplane $$H_\lambda$$ may not intersect
$$X$$ transversely. In order to utilize the Weil conjectures, we therefore need
to ensure that $$\lambda$$ is such that $$H_\lambda$$ intersects $$X$$
transversally. Let us call this assumption $$(\ast)$$.

Of course, not all $$\lambda$$ will satisfy $$(\ast)$$, so we need to understand
the question of which linear functionals $$\lambda$$ satisfy $$(\ast)$$. We'll
address this in the next post. We'll use the weak and hard Lefschetz hyperplane
theorems to show that if $$X\subseteq \PP^n$$ is a smooth projective variety of
dimension $$m>2$$ whose dual variety $$X^\ast \subseteq (\PP^n)^\ast$$ is *not*
a hypersurface, then $$\#(X\cap H_\lambda)(k)$$, and hence $$\FT_X(\lambda)$$,
is independent of $$\lambda$$ for generic $$\lambda$$. We then construct
examples of varieties satisfying this property: we show, for instance, that
*scrolls* (such as the image of the Segre embedding $$\PP^1\times \PP^n
\hookrightarrow \PP^{2n+1}$$) provide examples of such varieties. We'll also
show that if $$X$$ denotes the image $$\nu_2(\PP^d)\subseteq \PP^{(n+2)(n+1)/2 -
1}$$ of the $$2$$-fold Veronese embedding for $$n$$ even, then
$$\FT_X(\lambda)$$ is independent of $$\lambda$$ for generic $$\lambda$$, even
though $$X$$ does not satisfy the hypotheses of the result regarding dual
varieties.

Let's denote $$X\cap H_\lambda$$ by $$X_\lambda$$; assume $$(\ast)$$. We can
apply Deligne's resolution of the Weil conjectures to conclude that

$$\#(X\cap H_\lambda)(k) = \sum_{i=0}^{2(\dim(X) - 1)} (-1)^i \Tr(\Frob_k |
\H^i((X_\lambda)_{\ol{k}};\QQ_\ell)),$$

where $$\H^i((X_\lambda)_{\ol{k}};\QQ_\ell)$$ denotes the $$\ell$$-adic
cohomology of $$(X_\lambda)_{\ol{k}}$$ and $$\Frob$$ denotes the map induced on
cohomology by the geometric Frobenius. To understand this $$\QQ_\ell$$-vector
space and the corresponding action of Frobenius, we use the Lefschetz hyperplane
theorem for $$\ell$$-adic cohomology. We recall the statement of this theorem
(albeit not in its maximum level of generality):

* *Weak Lefschetz:* Let $$k$$ be a perfect field of characteristic $$p\geq 0$$,
  and let $$X$$ be a smooth projective $$k$$-scheme of dimension $$n$$. Let
$$Y$$ be a linear section of $$X$$ of codimension $$d$$. Then for any $$j\geq
0$$, the map $$\H^i(X_{\ol{k}}; \QQ_\ell(j)) \to \H^i(Y_{\ol{k}}; \QQ_\ell(j))$$
is an isomorphism for $$i\leq n-d-1$$ and an injection for $$i = n-d$$.
* *Hard Lefschetz:* Let $$k$$ be a perfect field of characteristic $$p\geq 0$$,
  and let $$X$$ be a smooth projective $$k$$-scheme of dimension $$n$$. Let
$$Y$$ be a smooth hyperplane section of $$X$$, so $$Y$$ defines a hyperplane
class $$\eta\in \H^2(X_{\ol{k}}; \QQ_\ell(1))$$. Then for any $$j\geq 0$$, the
homomorphism $$\eta^j:\H^{n-j}(X_{\ol{k}}; \QQ_\ell) \to \H^{n+j}(X_{\ol{k}};
\QQ_\ell(j))$$ is an isomorphism. In particular,

$$\Tr(\Frob_k | \H^{n+j}(X_{\ol{k}}; \QQ_\ell)) = q^j \Tr(\Frob_k |
\H^{n-j}(X_{\ol{k}}; \QQ_\ell)). $$

In the statement of the weak Lefschetz theorem, the map $$\H^i(X_{\ol{k}};
\QQ_\ell) \to \H^i(Y_{\ol{k}}; \QQ_\ell)$$ is injective when $$i = n-d$$. The
orthogonal complement in dimension $$n-d$$ is given by the (dual space to the)
rational vanishing cycles of any Lefschetz pencil on $$X$$.
OK. In order to apply Lefschetz, we first split the sum for $$\#(X\cap
H_\lambda)(k)$$ into three terms:

$$\#(X\cap H_\lambda)(k) = \sum_{i=0}^{m-2} (-1)^i \Tr(\Frob_k |
\H^i((X_\lambda)_{\ol{k}};\QQ_\ell)) + (-1)^{m-1} \Tr(\Frob_k |
\H^{m-1}((X_\lambda)_{\ol{k}};\QQ_\ell)) + \sum_{i\geq m}^{2(m-1)} (-1)^{i}
\Tr(\Frob_k | \H^i((X_\lambda)_{\ol{k}};\QQ_\ell)).$$

Applying weak Lefschetz in the case of $$X_\lambda$$ being a codimension $$1$$
subvariety of $$X$$ shows that the map $$\H^i(X_{\ol{k}};\QQ_\ell)\to
\H^i((X_\lambda)_{\ol{k}};\QQ_\ell)$$ is an isomorphism for $$i\leq m-2$$. In
particular, it is independent of $$\lambda$$. Therefore, the first sum in the
equation for $$\#(X\cap H_\lambda)(k)$$ is independent of $$\lambda$$.
The third sum can be approached similarly by combining weak and hard Lefschetz.
Indeed, by hard and weak Lefschetz, we have the following for $$j\geq 1$$:

$$\Tr(\Frob_k | \H^{m-1+j}((X_\lambda)_{\ol{k}}; \QQ_\ell)) = q^j
\Tr(\Frob_k | \H^{m-1-j}((X_\lambda)_{\ol{k}}; \QQ_\ell)) = q^j \Tr(\Frob_k |
\H^{m-1-j}(X_{\ol{k}}; \QQ_\ell)) \text{ if }j\geq 1.$$

For $$j\geq 1$$, we have $$m-1-j\leq m-2$$, so weak Lefschetz can then be
applied. We note that instead of appealing to hard Lefschetz, one could also use
Poincare duality to reduce to studying the trace of Frobenius on cohomology
below the middle dimension, at which point can again apply weak Lefschetz.
Combining the above observations together yields:

$$\#(X\cap H_\lambda)(k) = (-1)^{m-1} \Tr(\Frob_k |
\H^{m-1}((X_\lambda)_{\ol{k}};\QQ_\ell)) + \text{terms independent of
}\lambda.$$

Here's an example. Suppose $$X$$ is a curve or a proper smooth complete
intersection of dimension $$d$$. Then it follows from weak and hard Lefschetz
that for $$i\neq d$$, the $$\ell$$-adic cohomology $$\H^i(X_{\ol{k}};
\QQ_\ell)$$ is isomorphic to $$\H^i(\PP^n;\QQ_\ell)$$. Recall that
$$\H^i(\PP^n;\QQ_\ell)$$ vanishes unless $$0\leq i\leq 2n$$ is even, in which
case it is the Tate twist $$\QQ_\ell(-i/2)$$. The Frobenius acts on the
$$1$$-dimensional $$\Gal(\ol{k}/k)$$-module $$\QQ_\ell(i)$$ by multiplication by
$$q^{-i}$$. Consequently, we find that $$\H^i(X_{\ol{k}}; \QQ_\ell)$$ vanishes
unless $$i$$ is even, in which case it is $$1$$-dimensional and the Frobenius
acts on it by multiplication by $$q^i$$. In particular, the terms independent of
$$\lambda$$ in can be made explicit in this case. Indeed, the first sum in the
expression for $$\#(X\cap H_\lambda)(k)$$ is $$\sum_{i=0}^{\lfloor m/2\rfloor-1}
q^i$$, while the third sum is $$\sum_{i\geq 1, \ m+i\ \text{odd}}^{m-1}
q^{(m+j-1)/2}$$. In other words:

$$\#(X\cap H_\lambda)(k) = (-1)^{m-1} \Tr(\Frob_k |
\H^{m-1}((X_\lambda)_{\ol{k}};\QQ_\ell)) + \sum_{i=0}^{\lfloor m/2\rfloor-1} q^i
+ \sum_{i\geq 1, \ m+i\ \text{odd}}^{m-1} q^{(m+j-1)/2}.$$

Returning to the general case, it follows that it
remains to understand the middle-dimensional cohomology
$$\H^{m-1}((X_\lambda)_{\ol{k}};\QQ_\ell)$$, as is typical in all flavors of
geometry. The question of when $$\#(X\cap H_\lambda)(k)$$ is independent of
$$\lambda$$ for generic $$\lambda$$ can now be reduced to the question of when
$$\H^{m-1}((X_\lambda)_{\ol{k}};\QQ_\ell)$$ is independent of $$\lambda$$ for
generic $$\lambda$$. Obviously, one such case would be when the map
$$\H^{m-1}(X_{\ol{k}};\QQ_\ell)\to \H^{m-1}((X_\lambda)_{\ol{k}};\QQ_\ell)$$ is
an isomorphism, i.e., when the weak Lefschetz theorem extends to the middle
cohomology of the hyperplane section. This will not always be the case, but we
can nonetheless provide general conditions on when this result would hold.

So: we've reduced to understanding when the middle dimensional cohomology of a
hyperplane section of $$X$$ does not depend on the hyperplane itself. One of our
main results shows that this is the case when the dual variety of $$X$$ is not a
hypersurface (at least when $$X$$ has dimension $$>2$$). The question of when
the dual variety is not a hypersurface was studied in great detail
[here](https://link.springer.com/article/10.1007/BF01391495); we shall take a
more elementary approach in this section.

We begin with by recalling some basics. If $$X\subseteq \PP^n$$ is a smooth
projective variety, then the dual variety $$X^\ast\subseteq (\PP^n)^\ast$$ of
$$X$$ is the set of hyperplanes $$H\in (\PP^n)^\ast$$ such that $$X\cap H$$ is
singular. Our main source of examples for when the weak Lefschetz theorem
extends to the middle cohomology of the hyperplane section comes from the
following:

**Theorem:** Let $$X\subseteq \PP^n$$ is a smooth projective variety of
dimension $$m\geq 2$$, and suppose that $$X^\ast\subseteq (\PP^n)^\ast$$ is
*not* a hypersurface. If $$H$$ is a hyperplane such that the hyperplane
section $$X\cap H$$ is smooth, then the map $$\H^{m-1}(X_{\ol{k}}; \QQ_\ell)\to
\H^{m-1}((X\cap H)_{\ol{k}}; \QQ_\ell)$$ is an isomorphism.

The proof we present of this theorem only uses the weak Lefschetz theorem
combined with the Leray spectral sequence. There is an alternative proof of this
result, suggested to us by Roman Bezrukavnikov; this argument relies on
(elementary aspects of) the theory of perverse sheaves, but we do not present it
here.

Let's begin the proof. We will assume that $$m>2$$ (so $$X$$ is not a surface);
the argument in the case $$m=2$$ only requires slight modifications. Assume that
$$X^\ast$$ is not a hypersurface, so its codimension is $$\geq 2$$. Suppose that
$$\PP^1\subseteq (\PP^n)^\ast$$ is a line defining a family of hyperplanes which
do not meet $$X^\ast$$ (so the resulting family of hyperplane sections on $$X$$
is smooth). This is possible by the codimension restriction on $$X^\ast$$. Let
$$f:\wt{X}\to \PP^1$$ denote the associated pencil given by restricting the
family of hyperplane sections to $$\PP^1$$. Since $$\wt{X}\subseteq \PP^1 \times
X$$ is a smooth hyperplane section of dimension $$d$$, the weak Lefschetz
theorem gives an isomorphism $$\H^{m-1}(\PP^1\times X; \QQ_\ell)\to
\H^{m-1}(\wt{X}; \QQ_\ell)$$. We shall use this to prove the desired result.

Recall that if $$f:Y\to S$$ is a smooth proper morphism, then one has the Leray
spectral sequence

$$E_2^{s,t} = \H^s(S; \mathrm{R}^t f_\ast \QQ_\ell) \Rightarrow \H^{s+t}(Y;
\QQ_\ell).$$

As a consequence of the hard Lefschetz theorem, Deligne proved that this
spectral sequence degenerates at the $$E_2$$-page. Applying this degeneration to
the morphism $$f:\wt{X}\to \PP^1$$ and using the fact that the cohomology of
$$\PP^1$$ vanishes above dimension $$2$$ gives a short exact sequence

$$0\to \H^2(\PP^1; \mathrm{R}^{m-3} f_\ast \QQ_\ell)\to \H^{m-1}(\wt{X};
\QQ_\ell)\to \H^0(\PP^1; \mathrm{R}^{m-1} f_\ast \QQ_\ell)\to 0.$$

Since $$\PP^1$$ is simply connected, the local coefficient systems appearing
above are constant. Therefore, if $$H$$ is a hyperplane living on the chosen
line $$\PP^1\subseteq (\PP^n)^\ast$$, then $$\mathrm{R}^t f_\ast \QQ_\ell$$ is
the constant local system on $$\H^t((X\cap H)_{\ol{k}}; \QQ_\ell)$$. In other
words, the above exact sequence becomes

$$0\to \H^2(\PP^1; \QQ_\ell)\otimes \H^{m-3}((X\cap H)_{\ol{k}}; \QQ_\ell) \to
\H^{m-1}(\wt{X}; \QQ_\ell)\to \H^{m-1}((X\cap H)_{\ol{k}}; \QQ_\ell) \to 0.$$

Applying the degeneration of the Leray spectral sequence to the projection
morphism $$\PP^1\times X\to \PP^1$$ also produces an exact sequence

$$0\to \H^2(\PP^1; \QQ_\ell)\otimes \H^{m-3}(X_{\ol{k}}; \QQ_\ell) \to
\H^{m-1}(\PP^1\times X; \QQ_\ell)\to \H^{m-1}(X_{\ol{k}}; \QQ_\ell) \to 0.$$

There is a map of short exact sequences from the second one to the first one.
The second and third maps in this map of short exact sequences are isomorphisms
by the weak Lefschetz theorem and the observation from the previous paragraph
that $$\H^{m-1}(\PP^1\times X; \QQ_\ell)\cong \H^{m-1}(\wt{X}; \QQ_\ell)$$. By
the five lemma, this forces the map $$\H^{m-1}(X_{\ol{k}}; \QQ_\ell)\to
\H^{m-1}((X\cap H)_{\ol{k}}; \QQ_\ell)$$ to be an isomorphism, as desired.

Note that the statement of this theorem is not an if-and-only-if; namely, the
map $$\H^{m-1}(X_{\ol{k}}; \QQ_\ell)\to \H^{m-1}((X\cap H)_{\ol{k}}; \QQ_\ell)$$
being an isomorphism for all hyperplanes $$H$$ does not imply that $$X^\ast
\subseteq (\PP^n)^\ast$$ is not a hypersurface. For instance, we shall find
below that the image of the $$2$$-fold Veronese embedding $$\PP^n\to
\PP^{(n+2)(n-1)/2 - 1}$$ satisfies the conclusion of the theorem, but its dual
variety is a hypersurface.

It is quite unlikely that the dual variety of a smooth projective variety is not
a hypersurface. Nonetheless, we have the following examples. One expects the
dual variety to a variety $$X$$ to not be a hypersurface if $$X$$ is "constant
in the vertical direction". This is made precise by the notion of a scroll.
Recall that a (smooth) $$m$$-dimensional scroll is a variety $$X\subseteq
\PP^n$$ which is the union of a one-parameter family of $$(m-1)$$-planes
contained in $$\PP^n$$. In other words, a scroll is a smooth $$m$$-dimensional
variety with a surjective morphism $$\pi:X\to C$$ to a smooth curve $$C$$ such
that the fiber over every point is isomorphic to $$\PP^{m-1}$$.

For instance, the Segre embedding $$\PP^1\times \PP^n\hookrightarrow
\PP^{2(n+1)-1} = \PP^{2n+1}$$ evidently defines a smooth $$(n+1)$$-dimensional
scroll in $$\PP^{2n+1}$$.
Another example: a two-dimensional scroll $$X$$ is a ruled surface. Quadric
surfaces provide examples of ruled surfaces (at least, over a finite field).
Since an $$m$$-dimensional scroll $$X$$ is a union of a one-parameter family of
$$(m-1)$$-planes, one expects the dual variety to $$X$$ to not be a
hypersurface. 

This indeed turns out to be the case: if $$X\subseteq \PP^n$$ is a
smooth $$m$$-dimensional scroll with $$m\geq 2$$, then $$X$$ satisfies the
hypotheses of the theorem, i.e., the dual variety $$X^\ast$$ is not a
hypersurface.  Again, we assume $$m>2$$; only slight modifications are required
for $$m=2$$. If a hyperplane is tangent to $$x\in X$$ (i.e., it contains the
tangent plane to $$x$$), then it will also contain the tangent plane to all
points in the fiber over $$\pi(x)\in C$$. This fiber is an $$(m-1)$$-plane
$$\PP^{m-1}$$, so the codimension of the dual variety $$X^\ast$$ in
$$(\PP^n)^\ast$$ must be at least $$m-2$$. In particular, if $$X\subseteq
\PP^n$$ is a smooth $$m$$-dimensional scroll, then the dual variety $$X^\ast$$
has dimension at most $$n-m+2$$, and hence is not a hypersurface.

In particular, we find that if $$X\subseteq \PP^n$$ is an $$m$$-dimensional
scroll for $$m>2$$, then the Fourier transform $$\FT_X(\lambda)$$ is independent
of $$\lambda$$ for generic $$\lambda$$.

We shall end by showing that the surface given by the image of the double
Veronese embedding $$\PP^2 \to \PP^5$$ is another surface for which
$$\H^1(X_{\ol{k}}; \QQ_\ell) \to \H^1((X\cap H)_{\ol{k}}; \QQ_\ell)$$ is an
isomorphism; this is in fact true more generally for the double Veronese
embedding of an even-dimensional projective space.
Let $$\nu_d:\PP(V)\to \PP(\Sym^d V)$$ denote the $$d$$-fold Veronese embedding
associated to a vector space $$V$$. This map sends a line in $$V$$ spanned by
$$v\in V$$ to the line in $$\Sym^d V$$ spanned by $$v^d$$. (Note that
$$\nu_d(\PP(V))$$, being isomorphic to $$\PP(V)$$, is very far from being a
scroll.)

Then: let $$N = \binom{n+d}{d} - 1$$. The dual variety to $$\nu_d(\PP^n)
\subseteq \PP^{N}$$ is the hypersurface in $$\PP^N$$ given by the vanishing
locus of the discriminant of a general degree $$d$$ homogeneous polynomial in
$$n+1$$ variables.
It follows from the moduli-theoretic description of the Veronese embedding and
the definition of the dual variety that points of $$\nu_d(\PP^n)^\ast$$ classify
singular hypersurfaces of degree $$d$$ in $$\PP^n$$. Therefore,
$$\nu_d(\PP^n)^\ast$$ must be the hypersurface in $$\PP^N$$ given by the
vanishing locus of the discriminant of a degree $$d$$ homogeneous polynomial in
$$n+1$$ variables.

In particular, $$\nu_d(\PP^n) \subseteq \PP^N$$ will *not* satisfy the
hypotheses of the theorem. Nonetheless, we have:

**Proposition:** Let $$n$$ be even, and let $$N = \binom{n+2}{2} - 1 =
(n+2)(n+1)/2 - 1$$. Suppose $$\nu_2(\PP^n)\cap H \subseteq \PP^N$$ is a smooth
hyperplane section of $$\nu_2(\PP^n)$$. Then the map
$$\H^{n-1}(\nu_2(\PP^n)_{\ol{k}}; \QQ_\ell) \to \H^{n-1}((\nu_2(\PP^n)\cap
H)_{\ol{k}}; \QQ_\ell)$$ is an isomorphism; in fact, both groups are zero.

Here's a sketch. there is a bijective correspondence between hyperplanes $$H$$
in $$\PP^N$$ and hypersurfaces of degree $$d$$ in $$\PP^n$$ via sending $$H$$ to
$$H\cap \nu_d(\PP^n) \subseteq \nu_d(\PP^n)$$. To prove the proposition, it
therefore suffices to show that $$\H^{n-1}(\PP^n_{\ol{k}}; \QQ_\ell) \to
\H^{n-1}(X_{\ol{k}}; \QQ_\ell)$$ is an isomorphism when $$X\subseteq \PP^n$$ is
a smooth hypersurface of degree $$2$$, i.e., when $$X$$ is a smooth quadric.
Since $$n$$ is even, $$n-1$$ is odd, and therefore $$\H^{n-1}(\PP^n_{\ol{k}};
\QQ_\ell) = 0$$. Upon base-changing to an algebraically closed field, the
quadric $$x$$ can be diagonalized to one of the form $$x_0^2 + \cdots + x_n^2 =
0$$. This explicit form allows one to calculate that $$\H^{n-1}(X_{\ol{k}};
\QQ_\ell) = 0$$ when $$n$$ is even. The map $$\H^{n-1}(\PP^n_{\ol{k}}; \QQ_\ell)
\to \H^{n-1}(X_{\ol{k}}; \QQ_\ell)$$ is then an isomorphism.

We conclude that if $$X = \nu_2(\PP^n)\subseteq \PP^{(n+2)(n+1)/2 - 1}$$ is the
image of the $$2$$-fold Veronese embedding of an even-dimensional projective
space, then the Fourier transform $$\FT_X(\lambda)$$ is independent of
$$\lambda$$ for generic $$\lambda$$.
