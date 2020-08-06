---
layout: post
title:  "The secretary problem"
date:   2020-04-19
categories: misc
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

I think I'm going to start posting some non-math thoughts on this blog (but the
posts will primarily be math), but not in this post.

In this post, I'd like to talk about a fun question regarding the secretary
problem. Let's recall what it is. There are $$n$$ candidates interviewing for a
position, and they're interviewed one-by-one. There is a total ordering on the
set of candidates. The interviewer has to accept or reject a candidate
immediately after their interview. What policy should the interviewer adopt?

It turns out that one can show that the best policy is of the following form.
Let $$\pi_k$$ denote the policy where the interviewer interviews (the first)
$$k-1$$ candidates, and then accepts the next best candidate. So, the question
is: what value of $$k$$ is optimal? Let's call $$p_k$$ the probability that the
best ranked candidate is chosen under policy $$\pi_k$$, so we're trying to
maximize $$p_k$$.

What is $$p_k$$? Let's write down the order of appearance of the candidates as a
permutation $$\sigma_1, \cdots, \sigma_n$$, and use the standard total ordering
on the set $$\{1, \cdots, n\}$$ as the ranking. So, $$\pi_k$$ wins if the top
ranked candidate appears at spot $$m$$ with $$k\leq m$$, and also if the top
candidate appears at spot $$m$$, then the minimum of $$\{x_1, \cdots,
x_{m-1}\}$$ must be in spots $$1, \cdots, k-1$$, i.e., must be one of the first
$$k-1$$ candidates. (The latter requirement states that the second best
candidate, relative to the ones the interviewer has seen so far, appear in the
first $$k-1$$ candidates; this is because the policy $$\pi_k$$ states that the
interviewer will accept the best candidate relative to the previous ones after
interviewing the first $$k-1$$.) The probability that the top candidate appears
at spot $$m$$ is $$1/n$$ (because there are $$n$$ candidates), and the
probability that the minimum of $$\{x_1, \cdots, x_{m-1}\}$$ must be in spots
$$1, \cdots, k-1$$ is $$(k-1)/(m-1)$$. So, in total,

$$p_k = \frac{k-1}{n} \sum_{k\leq m\leq n} \frac{1}{m-1}.$$

(Obviously, this doesn't work when $$k=1$$; but when $$k=1$$, the interviewer
just chooses the first candidate!) Let $$x = \lim_{n\to \infty} (k-1)/n$$, so
that this sum is

$$\lim_{n\to \infty} p_k = x\int^1_x \frac{dz}{z} = -x\ln(x).$$

This is maximized when $$x = e^{-1} \approx 0.368$$, so as $$n\to \infty$$, the
optimal $$k$$ is $$n/e$$. In other words, the interviewer should pick someone
after interviewing about $$36.8\%$$ of the candidates, at least if the number of
candidate grows to $$\infty$$.

Let's call the policy $$\pi_{n/e}$$ the "optimal highest rank policy". (OK,
$$n/e$$ isn't an integer, but you get what I mean.)

This was all classical. I came across the following question: pick some $$r\leq
n$$; what is the probability that the candidate picked has rank $$r$$? To answer
this, one just runs a slight variant of the above argument. Let's write
$$p_k(r)$$ to denote the probability that the candidate picked under policy
$$\pi_k$$ has rank $$r$$. What is $$p_k(r)$$? (Note, obviously, $$p_k(1) =
p_k$$.)

If the first $$k-1$$ candidates are, by some strange luck, all the worst, then
the highest possible rank for the $$k$$th candidate is $$n-(k-1)$$. So,
$$p_k(r)$$ is positive only when $$r\leq n-k+1$$. Let's assume $$r$$ satisfies
this. Then, $$\pi_k$$ wins if and only if the $$r$$th ranked candidate appears
at some spot $$k\leq m$$. Moreover, this candidate should appear before the
candidates with ranks equal to $$1, \cdots, r-1$$. So, $$m$$ must be at most
$$n-(r-1)$$. The probability that the $$r$$th ranked candidate appears at spot
$$m$$ is $$1/n$$. Out of the other $$n-1$$ possible choices, there are $$r-1$$
choices for the candidates with ranks equal to $$1, \cdots, r-1$$. Moreover,
these $$r-1$$ choices are all worse than the choices of rank $$m$$, so are made
from the group of size $$n-m$$. In total, the probability of the $$r$$th ranked
candidate appearing at some spot $$k\leq m$$ and before the candidates with
ranks equal to $$1, \cdots, r-1$$ is given by $$n^{-1} \binom{n-m}{r-1} /
\binom{n-1}{r-1}$$.

Next, because $$r$$ appears at spot $$m$$, the minimum of $$\{x_1, \cdots,
x_{m-1}\}$$ (i.e., the first $$m-1$$ candidates) must be in spots $$1, \cdots,
k-1$$, and the probability of that happening is $$(k-1)/(m-1)$$. We conclude
that the total probability is

$$p_k(r) = \frac{k-1}{n} \binom{n-1}{r-1}^{-1} \sum_{k\leq m\leq n-(r-1)}
\binom{n-m}{r-1} \frac{1}{m-1}.$$
