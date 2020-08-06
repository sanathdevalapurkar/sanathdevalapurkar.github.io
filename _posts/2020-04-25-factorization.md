---
layout: post
title:  "Confusion about factorization algebras"
date:   2020-04-25
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
\newcommand{\Aff}{\mathrm{Aff}} \newcommand{\BGL}{\mathrm{BGL}}
\newcommand{\an}{\mathrm{an}} \newcommand{\Tel}{\mathrm{Tel}}
\renewcommand{\|}{|}$$

In this brief post, I'd like to talk about something I'm confused about. The
question is: what is the precise relationship between factorization algebras and
$$\E_2$$-algebras? Here's how I would like it to go. Let $$Y$$ be a smooth
complex variety. The Riemann-Hilbert correspondence gives an equivalence between
regular holonomic D-modules on $$Y$$ and constructible sheaves on
$$Y^\mathrm{an}$$, given by the de Rham/solutions functor. Let's suppose we can
somehow apply this to $$Y = \Ran(X)$$, where $$X$$ is a smooth algebraic curve
(this can't be done literally, because $$\Ran(X)$$ is just a functor.
Whatever.). Then, we obtain a comparison between regular holonomic D-modules on
$$\Ran(X)$$ and constructible sheaves on $$\Ran(X^\mathrm{an})$$.

Here is where I get confused.
* Let $$X = \AA^1$$, so $$X^\mathrm{an} = \cc$$. We know that $$\E_2$$-algebras
  in topology correspond to sheaves on $$\Ran(\cc)$$ which are constructible
with respect to a *particular* stratification (namely, the order stratification
on $$\Ran(\cc)$$), whereas the Riemann-Hilbert correspondence just constructs a
sheaf on $$\Ran(X^\mathrm{an})$$ which is constructible for *some*
stratification.  Maybe this is obviously not an issue (perhaps because
$$\Ran(X^\mathrm{an})$$ is contractible)?
* Is it obvious that the factorizability condition on D-modules on $$\Ran(X)$$
  realizes under the de Rham/solutions functor to the factorizability condition
on $$\Ran(X^\mathrm{an})$$? It seems like this is in fact *not* the case! But
I'm probably missing something...

However, here's one thing you can do to get an $$\E_2$$-space from an ind-proper
factorization space (following [this paper](https://arxiv.org/abs/1710.05366)).
Let's say that $$X = \AA^1$$, and let $$\dY$$ be a factorization space over
$$X$$. To describe a (nonunital) $$\E_2$$-space $$Y$$, I just have to tell you a
space $$Y(D)$$ for every disk $$D \subseteq \cc$$, and coherent maps
$$\prod^n_{i=1} Y(D_i) \to Y(D)$$ for every inclusion $$\coprod_{i=1}^n D_i \to
D$$ of disks, such that for every embedding $$D \subseteq D'$$ of disks, the
induced map $$Y(D) \to Y(D')$$ is an equivalence ("local constancy").  So,
suppose $$D\subseteq \cc$$; then, you get an inclusion $$\Ran(D)\subseteq
\Ran(\cc) = \Ran((\AA^1)^\mathrm{an})$$, and $$Y(D)$$ is defined to be the
preimage of $$\Ran(D)$$ under $$\dY(\cc)\to \Ran(\cc)$$.

The factorization condition on $$\dY$$ now gets you coherent maps
$$\prod^n_{i=1} Y(D_i) \to Y(D)$$ for every inclusion $$\coprod_{i=1}^n D_i \to
D$$ of disks. How about local constancy? This is the hard part, but I think by
arguing as in Jeremy's and Allen's paper, it's true that if $$\dY\to \Ran(X)$$
is such that $$\dY\times_{\Ran(X)} X^I$$ is ind-proper for every finite set
$$I$$, then the canonical map $$\dY(\cc)\times_{\Ran(\cc)} \{x\} \to Y(D)$$ is
an equivalence for every $$x\in D\subseteq \cc$$. This obviously implies local
constancy.

Although nice, this isn't terribly terribly satisfying... It's not like the
Riemann-Hilbert correspondence, which tells you that upon putting some
restrictions on allowed singularities, you get an identification between
topological information (constructible sheaves) and algebraic information
(D-modules). So: what is the analogue of Riemann-Hilbert for factorization
*spaces* and $$\E_2$$-*spaces*?
