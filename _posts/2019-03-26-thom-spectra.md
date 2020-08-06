---
layout: post
title:  "Certain finite Thom spectra"
date:   2019-03-26
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
\newcommand{\GL}{\mathrm{GL}} \newcommand{\Ln}{L_n}
\newcommand{\Lt}{L_{K(t)}} \newcommand{\W}{\mathrm{W}}
\newcommand{\BU}{\mathrm{BU}} \newcommand{\SU}{\mathrm{SU}}
\newcommand{\MU}{\mathrm{MU}} \newcommand{\ul}[1]{\underline #1}
\newcommand{\Sq}{\mathrm{Sq}}$$

In the [previous post](/algebraic-topology/2019/03/25/c-or.html), we focused on
the Hopkins-Mahowald theorem, exhibiting $$\H\FF_2$$ as a Thom spectrum over
$$\S$$. Here is a silly related observation: $$\H\FF_2$$ is the Thom spectrum
of a map $$X\to B\GL_1(\H\Z)$$ that factors through $$B\GL_1(\S)$$. Namely,
since $$\H\FF_2 \simeq \H\Z \wedge \S/2$$, we can simply choose $$X = S^1$$,
and the map $$X \to B\GL_1(\S)$$ classifying $$-1\in \pi_0(\S)^\times$$. More
nontrivially, one can ask if $$\H\FF_2$$ is the Thom spectrum of a map $$X\to
B\GL_1(\ko)$$ that factors through $$B\GL_1(\S)$$. 

There is a finite spectrum $$A_1$$ such that $$\ko \wedge A_1\cong
\H\FF_2$$, i.e., such that $$\H_\ast(A_1;\FF_2) \cong A(1)_\ast$$ as Steenrod
comodules. Let me briefly recall two constructions of this spectrum:

* Let $$Q$$ denote the question mark complex, constructed as the cofiber of the
  map $$\eta:S^2 \to S/2$$ obtained by choosing a lifting $$\Sigma\eta:S^2 \to
S^1$$ through $$S/2$$. Denote by $$DQ$$ its Spanier-Whitehead dual, which, upon
shifting (so that its bottom cell is in dimension zero) can alternatively be
constructed the Thom spectrum of the real bundle over $$\Sigma\RP^2$$
determined by the map $$\Sigma\RP^2 \to \BO$$ that's adjoint to the inclusion
$$\RP^2 \hookrightarrow \RP^3 = \mathrm{SO}(3) \hookrightarrow \Omega \BO$$.
(One can alternatively construct this bundle via clutching functions.) Consider
the smash product $$Q\wedge DQ$$. Then, the unit and evaluation maps compose to
give the map $$S^0 \to Q\wedge DQ \to S^0$$ given by multiplication by the
Euler characteristic of $$Q$$. It is easy to compute this Euler characteristic:
it's precisely multiplication by $$1$$. We conclude that $$S^0$$ splits off of
$$Q\wedge DQ$$; let $$F$$ denote the other summand. Then the cohomology of
$$F$$ is isomorphic to $$A(1)$$, so $$F$$ is an example of such a spectrum
$$A_1$$.

* The second construction is from Davis-Mahowald's *$$v_1$$- and
  $$v_2$$-Periodicity in Stable Homotopy Theory*.  Consider the suspension
  spectrum $$P^n$$ of real projective space; the cell structure of $$P^{18}$$ is
  illustrated below (the bottom cell is in dimension $$1$$):
  
  <img style="display: block; margin: auto;" height="25%" width="25%"
  alt="photo" src="/assets/P18.png">
  
  We can restrict to the bottom $$8$$ cells, and this tells us the cell structure
  of $$P^8$$. Let $$P^n_k = \RP^n/\RP^{k-1}$$ denote the subcomplex consisting of
  the cells between dimensions $$k$$ and $$n$$. Consider the map $$P^4_3 =
  \Sigma^3 S/2 \to P^8_3 \xrightarrow{2} P^8_3$$. Since the multiplication by
  $$2$$ map on $$S/2$$ is homotopic to the composite $$S/2 \to S^1
  \xrightarrow{\eta} S^0 \hookrightarrow S/2$$, and $$\eta$$ is nilpotent, we
  find that the map $$2:P^8_3 \to P^8_3$$ factors through the cofiber of the
  inclusion $$P^4_3 \to P^8_3$$, i.e., through $$P^8_5$$. Let $$t:P^8_5 \to
  P^8_3$$ denote the resulting map. We note that $$P^8_5 \simeq \Sigma^4 P^4$$
  (by James periodicity, or just direct visualization); $$\Sigma P^8_5$$ is the
  same as the "top four cells of $$A_1$$", so we'd like to construct a map from
  $$P^8_5$$ into a $$4$$-cell complex which agrees with the bottom four cells of
  $$A_1$$.
  
  By direct analysis, we see that the $$4$$-skeleton of $$A_1$$ is the same as (a
  shift of) $$P^6_3$$, so we want a map $$P^8_5 \to P^6_3$$. Since $$P^6_3$$ is
  the fiber of the map $$P^8_3 \to P^8_7$$, we would just need to show that the
  map $$P^8_5 \to P^8_3$$ is zero when projected down to $$P^8_7$$. But if we
  take the Spanier-Whitehead dual of the composite $$P^8_5 \to P^8_3 \to P^8_7$$,
  then the same argument as above shows that the resulting map is null (so the
  original map is also null); this gives us the desired map $$f:P^8_5 \to
  P^6_3$$. By calculations with the Adem relations, we find that the cofiber of
  $$f$$ indeed does have cohomology isomorphic to $$A(1)$$.

We can now ask the following question: is $$A_1$$ the Thom spectrum of a
spherical fibration (of virtual dimension zero) classified by a map $$X\to
B\GL_1(\S)$$? Before addressing this question, let's try to work out some
simpler examples.

* We showed above that the dual question mark complex $$DQ$$ is indeed a Thom
  spectrum: it's associated to a real bundle over $$\Sigma \RP^2$$.
* The question mark complex $$Q$$ is *not* a Thom spectrum; see
  [here](https://mathoverflow.net/questions/320709/finite-complexes-which-are-not-thom-spectra).
  Indeed, suppose otherwise, and assume that $$Q = X^\mu$$ for a spherical
  fibration $$\mu$$ over a space $$X$$, and write $$\H^\ast(X;\FF_2) \cong
  \FF_2\{1,x_1,x_3\}$$. Let $$u$$ be the Thom class, so that $$\H^\ast(Q;\FF_2)
  \cong \FF_2\{u,ux_1,ux_3\}$$. We know that $$\Sq^1(u) = ux_1$$ and
  $$\Sq^2(ux_1) = ux_3$$. But
  
  $$\Sq^2(ux_1) = \Sq^2(u) x_1 + \Sq^1(u) \Sq^1(x_1)+ u\Sq^2(x_1)$$
  
  by the Cartan formula. By unstability, $$\Sq^2(x_1) = 0$$, and by
  dimension considerations, we know that $$\Sq^2(u) = 0$$ and $$\Sq^1(x_1) = 0$$.
  Therefore $$\Sq^2(ux_1) = 0$$; contradiction!
* Along similar lines, the "Joker" $$J$$ is also not a Thom spectrum. This is a
  $$5$$-cell complex whose cohomology is $$\H^\ast(J;\FF_2)$$ is the quotient
  of the Steenrod algebra $$\mathcal{A}$$ by the left ideal generated by
  $$\Sq^3$$ and $$\Sq^i \mathcal{A}$$ for $$i\geq 4$$; it's constructed using the
  Toda bracket $$\eta^2\in \langle 2, \eta, 2\rangle$$. Suppose that $$J =
  X^\mu$$ for a spherical fibration $$\mu$$ over a space $$X$$, and write
  $$\H^\ast(X;\FF_2) \cong \FF_2\{1,x_1,x_2,x_3,x_4\}$$. Let $$u$$ be the Thom
  class, so that $$\H^\ast(J;\FF_2) \cong \FF_2\{u,ux_1,ux_2,ux_3,ux_4\}$$. We
  know that $$\Sq^1(u) = ux_1$$ and $$\Sq^2(u) = ux_2$$. Moreover, $$\Sq^2
  \Sq^1(u) = ux_3$$. Therefore:
  
  $$ux_3 = \Sq^2(ux_1) = \Sq^2(u) x_1 + \Sq^1(u) \Sq^1(x_1) + u\Sq^2(x_1) =
  ux_1(x_2 + \Sq^1(x_1)).$$
  
  Here, we used the fact that $$\Sq^2(x_1) = 0$$ by unstability. Now,
  $$\Sq^1(x_1) \in \FF_2\{x_2\}$$, so $$\Sq^1(x_1) = 0$$ or $$x_2$$. If
  $$\Sq^1(x_1) = x_2$$, then $$ux_3 = 0$$ --- contradiction. Therefore,
  $$x_1^2 = \Sq^1(x_1) = 0$$, and $$ux_3 = ux_1x_2$$, i.e., $$x_3 = x_1 x_2$$. We
  also know that $$ux_4 = \Sq^1(ux_3)$$, so
  
  $$ux_4 = \Sq^1(u) x_1 x_2 + u \Sq^1(x_1) x_2 + u x_1 \Sq^1(x_2).$$
  
  We showed that $$\Sq^1(x_1) = 0$$. Since $$\Sq^1(u) = ux_1$$ and $$x_1^2 = 0$$,
  the term $$\Sq^1(u) x_1 x_2$$ also vanishes. Therefore, $$ux_4 =
  ux_1\Sq^1(x_2)$$. But $$\Sq^1(x_2)\in \FF_2\{x_3\}$$. If $$\Sq^1(x_2) = 0$$, we
  run into a contradiction. If $$\Sq^1(x_2) = x_3 = x_1 x_2$$, then since $$x_1^2
  = 0$$, we also run into a contradiction, as desired.

Alright, let's return back to $$A_1$$. Suppose that $$A_1 = X^\mu$$; let's try
to deduce the structure of $$\H^\ast(X)$$ (we'll now just work with mod $$2$$
coefficients). Note that we're technically being a bit crass here: there are
four different things one might mean by $$A_1$$, but we'll address this later.
Let's first look at the action of the subalgebra $$A(1) = \langle \Sq^1,
\Sq^2\rangle$$. Suppose that $$\H^\ast(X) =
\FF_2\{1,b_1,b_2,b_3,b_3',b_4,b_5,b_6\}$$, and let $$u$$ be the Thom class. We
know that $$\Sq^1(u) = ub_1$$ and $$\Sq^2(u) = ub_2$$. Arguing as in the case
of the Joker, we have $$\Sq^1(b_1) = b_1^2 = 0$$ and $$b_3 = b_1 b_2$$.
Moreover, we know that $$ub_3' = \Sq^1(ub_2) = u(b_1b_2 + \Sq^1(b_2))$$, so
that $$b_3' = b_3 + \Sq^1(b_2) = b_1b_2 + \Sq^1(b_2)$$. Since

$$ub_4 = \Sq^1(ub_3) = \Sq^1(u) b_1 b_2 + u \Sq^1(b_1) b_2 + u b_1 \Sq^1(b_2) =
u b_1^2 b_2 + 0 + u b_1 \Sq^1(b_2) = u b_1 \Sq^1(b_2),$$

so we need $$b_4 = b_1 \Sq^1(b_2)$$. We also have

$$ub_5 = \Sq^2(ub_3') = \Sq^2(u) b_3' + \Sq^1(u) \Sq^1(b_3') + u \Sq^2(b_3') =
u b_2 b_3' + u b_1 \Sq^1(b_3') + u \Sq^2(b_3').$$

We calculate that

$$\Sq^1(b_3') = \Sq^1(b_1b_2 + \Sq^1(b_2)) = b_1\Sq^1(b_2) = b_1 b_3',$$

where we used $$\Sq^1 \Sq^1 = 0$$. Moreover,

$$\Sq^2(b_3') = \Sq^2(b_1b_2 + \Sq^1(b_2)) = \Sq^2 \Sq^1 (b_2) + b_1 \Sq^2(b_2)
= \Sq^2 \Sq^1(b_2) + b_1 b_2^2.$$

Therefore,

$$ub_5 = \Sq^2(ub_3') = ub_2(b_1b_2 + \Sq^1(b_2)) + u b_1 (b_1 b_3') + u(\Sq^2
\Sq^1(b_2) + b_1 b_2^2) = u b_2 \Sq^1(b_2) + u \Sq^2 \Sq^1(b_2).$$

Now, $$\Sq^1(b_2)$$ is nonzero --- otherwise, since $$b_3' = b_3 +
\Sq^1(b_2)$$, we'd have $$b_3' = b_3$$, which is absurd. Since $$\Sq^2
\Sq^1(b_2)\in \FF_2\{b_5\}$$, we need $$\Sq^2 \Sq^1(b_2) = 0$$ and $$b_5 = b_2
\Sq^1(b_2)$$. Finally, we know that

$$ub_6 = \Sq^2(ub_4) = \Sq^2(u) b_4 + \Sq^1(u) \Sq^1(b_4) + u \Sq^2(b_4) = u
b_2 b_4 + u b_1 \Sq^1(b_4) + u \Sq^2(b_4).$$

Now, since $$\Sq^1(b_4) = \Sq^1(b_1 \Sq^1(b_2))$$ and $$\Sq^1(b_1) = 0$$ and
$$\Sq^1 \Sq^1 = 0$$, we find that $$\Sq^1(b_4) = 0$$. Moreover, $$\Sq^2(b_4) =
b_1 \Sq^2 \Sq^1(b_2) = 0$$, since we observed that $$\Sq^2 \Sq^1(b_2) = 0$$.
Therefore, $$ub_6 = ub_2 b_4$$, i.e., $$b_6 = b_2 b_4 = b_1 b_2 \Sq^1(b_2)$$.
Let's check that this makes sense: we also know that $$\Sq^1(ub_5) = ub_6$$,
but

$$\Sq^1(ub_5) = \Sq^1(u) b_5 + u \Sq^1(b_5) = ub_1b_5 + u \Sq^1(b_2)^2,$$

we need

$$b_6 = b_1 b_5 + \Sq^1(b_2)^2 = b_1 b_2 \Sq^1(b_2) + \Sq^1(b_2)^2.$$

But $$\Sq^1(b_2)^2 = \Sq^3 \Sq^1(b_2)$$, and since $$\Sq^3 = \Sq^1 \Sq^2$$,
we find that $$\Sq^1(b_2)^2 = 0$$. 

That was some painful algebra, so let's summarize what we've found. The
cohomology of $$X$$ is of the form $$\FF_2\{1, b_1, b_2, b_1 b_2, \Sq^1(b_2),
b_1 \Sq^1(b_2), b_2 \Sq^1(b_2), b_1 b_2 \Sq^1(b_2)\}$$, where $$b_1^2 = 0$$ and
$$\Sq^2\Sq^1(b_2) = 0$$. (We haven't said anything about the action of
$$\Sq^2$$ on $$b_2$$, i.e., what $$b_2^2$$ should be.)

So far, we've only looked at the $$A(1)$$-module structure on $$\H^\ast(X)$$;
it's now time to bring in the entire $$A$$-module structure. As shown in Figure
1.1 of [this paper](https://arxiv.org/pdf/1406.3297.pdf), there are four
different refinements of the $$A(1)$$-module structure on $$\H^\ast(A_1)$$ to
an $$A$$-module structure. In each of these refinements, $$\Sq^4$$ is nonzero
on the class in dimension $$1$$, i.e., $$ub_1$$; in other words, $$ub_5 =
\Sq^4(ub_1)$$. But $$\Sq^4(ub_1) = \Sq^3(u) \Sq^1(b_1) + \Sq^4(u) b_1$$ by
the Cartan relations and unstability. Since $$\Sq^1(b_1) = 0$$, it follows that
$$ub_5 = \Sq^4(u) b_1$$. In particular, $$\Sq^4(u)$$ cannot vanish; this rules
out the spectra denoted $$A_1[00]$$ and $$A_1[01]$$ in *loc. cit*. as being
Thom spectra.

Since $$\Sq^4(u)\in \FF_2\{ub_4\}$$, we need $$\Sq^4(u) = ub_4 = u b_1
\Sq^1(b_2)$$. It follows that

$$ub_5 = \Sq^4(ub_1) = \Sq^4(u) b_1 = u b_1^2 \Sq^1(b_2) = 0,$$

which is a contradiction (since $$b_5$$ cannot vanish)! In particular, we find
the (perhaps disappointing?) fact that $$A_1$$ is *not* the Thom spectrum of a
spherical fibration (of virtual dimension zero) classified by a map $$X\to
B\GL_1(\S)$$. I expect the same to be true of the spectra $$A_2$$, but proving
it seems like a real pain.
