---
layout: post
title:  "Another nilpotence theorem"
date:   2020-04-06
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

In the [previous post](/algebraic-topology/2020/04/04/nilpotence.html), we
described a way of proving the nilpotence theorem, at least at $$p=2$$. But it
sorta felt like cheating: we relied on the Hopkins-Mahowald $$\H\FF_p$$-theorem
to conclude. In this post, I would like to describe another nilpotence theorem,
and a generalization to arbitrary height will appear in my forthcoming paper.

Recall that the Hopkins-Mahowald theorem told us that the free $$\E_{2}$$-ring
with $$p=0$$ is $$\H\FF_p$$. This implies that if $$R$$ is an $$\E_{2}$$-ring,
and $$x\in \pi_\ast R$$ is such that $$px = 0$$ and $$x$$ has zero
$$\H\FF_p$$-Hurewicz image, then $$x$$ is nilpotent. Our goal is to prove the
following. There is another Hopkins-Mahowald theorem, telling us that the Thom
spectrum of the map

$$\Omega^2 S^3\langle 3\rangle \to \Omega^2 S^3 \xrightarrow{1-p}
\BGL_1(\S_{(p)})$$

is equivalent to $$\H\Z_p$$. The main result of this post is the following.

**Theorem:** The Hopkins-Mahowald $$\H\Z_p$$-theorem implies that if $$R$$ is a
$$p$$-local $$\E_{2}$$-ring spectrum, and $$x\in \pi_\ast R$$ is a class with trivial $$\H\Z_p$$-Hurewicz image such that:
* $$\alpha_1 x = 0$$ in $$\pi_\ast R$$; and
* the Toda bracket $$\langle p, \alpha_1, x\rangle$$ contains zero;

then $$x$$ is nilpotent.

*Proof:* We claim that the composite

$$\Omega^2 S^3\langle 3\rangle\to \BGL_1(\S_{(p)})\to \BGL_1(R[1/x]) \quad
(\ast)$$

is null. To show this, we recall another construction of the map $$\Omega^2
S^3\langle 3\rangle\to \BGL_1(\S_{(p)})$$. (This construction has nothing to do
with $$\BGL_1(\S_{(p)})$$.) There's an old result (due to Selick? I'm not gonna
try to find the reference right now) stating that $$\Omega^2 S^3\langle
3\rangle$$ retracts off $$\Omega^2 P^{2p+1}(p)$$, where, recall, $$P^{n+1}(p) =
S^n\cup_p e^{n+1}$$. This splitting is compatible with the canonical map
$$\Omega^2 S^3\langle 3\rangle\to \Omega^2 S^3$$ in the following sense. The
$$p$$-torsion element $$\alpha_1\in \pi_{2p}(S^3)$$ defines a map
$$P^{2p-1}(p)\to \Omega^2 S^3$$, and hence a map $$\Omega^2 P^{2p+1}(p)\to
\Omega^2 S^3$$, which we'll abusively denote $$\alpha_1$$. Then, the following
composite is homotopic to the canonical map $$\Omega^2 S^3\langle 3\rangle\to
\Omega^2 S^3$$:

$$\Omega^2 S^3\langle 3\rangle\to \Omega^2 P^{2p+1}(p) \xrightarrow{\alpha_1}
\Omega^2 S^3,$$

where the first map is a retraction of $$\Omega^2 S^3\langle 3\rangle$$ off
$$\Omega^2 P^{2p+1}(p)$$. 

Back to $$\BGL_1(\S_{(p)})$$: a slight bit more work shows that the above
discussion implies that the map $$\Omega^2 S^3\langle 3\rangle\to
\BGL_1(\S_{(p)})$$ is homotopic to the composite

$$\Omega^2 S^3\langle 3\rangle\to \Omega^2 P^{2p+1}(p) \xrightarrow{\alpha_1}
\BGL_1(\S_{(p)}),$$

where the final map is the extension of $$\alpha_1: P^{2p-1}(p)\to
\BGL_1(\S_{(p)})$$ along the double suspension $$P^{2p-1}(p)\to \Omega^2
P^{2p+1}(p)$$.

So, in order to achieve our goal of showing that $$(\ast)$$ is null, it suffices
to show that the composite

$$\Omega^2 P^{2p+1}(p)\to \BGL_1(\S_{(p)})\to \BGL_1(R[1/x])$$

is null. Since this composite is one of double loop spaces, it further
suffices to show that the composite

$$P^{2p-1}(p)\to \BGL_1(\S_{(p)})\to \BGL_1(R[1/x])\quad (\ast\ast)$$

is null. The bottom cell $$S^{2p-2}$$ of $$P^{2p-1}(p)$$ maps trivially to
$$\BGL_1(R[1/x])$$, because the bottom cell detects $$\alpha_1$$ (by our
discussion above), and $$\alpha_1$$ is nullhomotopic in $$R[1/x]$$. Therefore,
the map $$(\ast\ast)$$ factors through the top cell $$S^{2p-1}$$ of
$$P^{2p-1}(p)$$.  The resulting map

$$S^{2p-1}\to \BGL_1(\S_{(p)})\to \BGL_1(R[1/x])$$

detects an element of the Toda bracket $$\langle p, \alpha_1, x\rangle$$, but
this contains zero by hypothesis, so is nullhomotopic.

OK, now, since the map $$(\ast)$$ is null, the Hopkins-Mahowald
$$\H\Z_p$$-theorem implies that there is a ring map $$\H\Z_p\to R[1/x]$$. In
particular, the composite of the map $$x:\Sigma^{|x|} R\to R$$ with the unit
$$R\to R[1/x]$$ factors as the composite

$$\Sigma^{|x|} R \to \H\Z_p \wedge \Sigma^{|x|} R \xrightarrow{x} \H\Z_p \wedge
R \to R[1/x].$$

The middle map, however, is null, because $$x$$ has zero $$\H\Z_p$$-Hurewicz
image. Therefore, the element $$x\in \pi_\ast R[1/x]$$ is null, and hence
$$R[1/x]$$ is contractible. We win!
