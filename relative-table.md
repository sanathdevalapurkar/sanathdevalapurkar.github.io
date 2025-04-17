---
layout: default
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


<h1>Examples in (generalized) relative Langlands duality</h1>

<a href = "https://www.math.ias.edu/~akshay/research/BZSVpaperV1.pdf">Ben-Zvi,
Sakellaridis, and Venkatesh</a> have recently proposed a matching between
objects in the Langlands program, namely that the relationship between $$G$$ and
its Langlands dual $$\check{G}$$ should extend to a duality between Hamiltonian
$$G$$-spaces $$M$$ and Hamiltonian $$\check{G}$$-spaces $$\check{M}$$. This goes
under the name of "*relative* Langlands duality". By now, others have compiled
comprehensive lists (e.g., <a href =
"https://www.jonathanpwang.com/notes/RelativeDualitydb.html">here</a> and <a
href =
"https://sites.rutgers.edu/chen-wan/wp-content/uploads/sites/518/2024/10/BZSVstonglytempered.pdf">here</a>)
of examples of such dualities. 

In two recent articles (<a href =
"https://sanathdevalapurkar.github.io/files/hyperboloid_spectral_decomp.pdf">here</a>
and <a href =
"https://sanathdevalapurkar.github.io/files/grG-regular.pdf">here</a>), I
proposed an extension of this duality to exotic coefficients on one side, which
amounts to a variant of the notion of a Hamiltonian space on the dual side.
Namely, if $$X$$ is a $$G$$-space, then $$M = T^\ast X$$ is a Hamiltonian
$$G$$-space, and the "usual" picture of relative Langlands proposes that there
is a dual Hamiltonian $$\check{G}$$-space $$\check{M}$$ which controls the
harmonic analysis of $$X$$, in the sense that (say) $$\mathrm{Shv}(X_F/G_O;
\mathbf{C})$$ is equivalent to $$\mathrm{QCoh}(\check{M}/\check{G})$$. If one
replaces $$\mathbf{C}$$ by complex K-theory $$\mathrm{KU}$$ or by an elliptic
cohomology theory $$k$$ with associated elliptic curve $$E$$, then $$\check{M}$$
must accordingly be replaced by a *quasi*-Hamiltonian or *elliptic* Hamiltonian
$$\check{G}$$-space, respectively. The table below is a list of examples of
these exotic Langlands duals. (Note that I am assuming throughout that my
starting data is $$X$$, not $$M$$.)

For simplicity, I will ignore the case of elliptic cohomology, and focus instead
on the generalized cohomology theory $$\mathrm{ku}$$ called "connective complex
K-theory": the Langlands dual side will involve a graded scheme
$$\check{M}_\beta$$ over $$\mathbf{A}^1/\mathbf{G}_m$$ with coordinate
$$\beta$$, whose special fiber over $$\beta = 0$$ produces the "usual" Langlands
dual Hamiltonian $$\check{G}$$-space, and whose generic fiber over $$\beta = 1$$
produces the quasi-Hamiltonian/$$\mathrm{KU}$$-theoretic dual. The phrase "for
ordinary cohomology" below means that I have not (yet) worked out the
$$\mathrm{ku}$$-theoretic dual to $$X$$, but that it should be interesting to do
so. There is a lot more information about these examples which I did not
include, like power operations (namely, Steenrod and Adams operations); for
this, see Section 9 of <a href =
"https://sanathdevalapurkar.github.io/files/grG-regular.pdf">this article</a>.

In the table below, $$T$$ denotes a maximal torus, $$B$$ a Borel subgroup, and
$$N$$ its unipotent radical; I will assume any unspecified reductive group is
connected and simply-laced.  Also, $$K_\beta$$ for a group scheme $$K$$ will
denote the deformation to the normal cone of the identity $$1\in K$$, so that
the special fiber of $$K_\beta$$ over $$\beta = 0$$ is the Lie algebra
$$\mathfrak{k}$$, and the generic fiber of $$K_\beta$$ over $$\beta = 1$$ is
$$K$$ itself. For example, $$\mathrm{SL}_{n,\beta}$$ is the group scheme of
$$n\times n$$-matrices $$A$$ such that $$\frac{\det(I + \beta A) - 1}{\beta} =
0$$. If $$V$$ and $$W$$ are vector spaces, let $$\mathcal{B}_\beta(V,W)$$ denote
the space of pairs $$(x,y) \in T^\ast(V \otimes W^\ast)$$ such that $$I + \beta
\langle x,y\rangle$$ is invertible; when $$\beta = 1$$, this is a multiplicative
quiver variety. The moment map associated to a $$\mathrm{ku}$$-Hamiltonian space
goes $$\check{M}_\beta \to G_\beta.$$

| $$G$$ | $$X$$ | $$\check{G}$$ | (Affinization of) $$\check{M}_\beta$$ | Moment map $$\check{M}_\beta \to {G}_\beta$$ |
| -- | -- | -- | -- | -- |
| $$H \times H$$ | $$H$$ | $$\check{H} \times \check{H}$$ | $$\check{H} \times {H}_\beta$$ | $$(\mathrm{projection}, \mathrm{conjugation})$$ |
| $$G$$ | $$G/_\psi N$$ | $$\check{G}$$ | $$\ast$$ | Identity |
| $$\mathbf{G}_m$$ | $$\mathbf{A}^1$$ | $$\mathbf{G}_m$$ | $$\mathcal{B}_\beta(\mathbf{A}^1, \mathbf{A}^1)$$ | $$(u,v)$$ is sent to $$1 + \beta \langle u,v\rangle$$ |
| $$H \times T$$ | $$H/N$$ | $$\check{H} \times \check{T}$$ | $${\check{H} \times^{\check{N}} B_\beta}$$ | Adjoint action | 
| $$H \times T$$ | $$H$$ | $$\check{H} \times \check{T}$$ | Affine closure of $${\check{H} \times^{\check{N}} B_\beta}$$ | Adjoint action | 
| $$\mathrm{PGL}_2$$ | $$\mathrm{PGL}_2/\mathbf{G}_m$$ | $$\mathrm{SL}_2$$ | $$\mathcal{B}_\beta(\mathbf{A}^1, \mathbf{A}^2)$$ | $$(u,v)$$ is sent to $$I + \beta u \otimes v$$ |
| $$\mathrm{GL}_n \times \mathrm{GL}_n$$ | $$\mathrm{GL}_n \times \mathbf{A}^n$$ | $$\mathrm{GL}_n \times \mathrm{GL}_n$$ | $$\mathcal{B}_\beta(\mathbf{A}^n, \mathbf{A}^n)$$ | $$(u,v)$$ is sent to $$(I + \beta uv, I + \beta vu)$$ |
| $$\mathrm{GL}_n \times \mathrm{GL}_{n-1}$$ | $$\mathrm{GL}_n$$ | $$\mathrm{GL}_n \times \mathrm{GL}_{n-1}$$ | $$\mathcal{B}_\beta(\mathbf{A}^n, \mathbf{A}^{n-1})$$ | $$(u,v)$$ is sent to $$(I + \beta uv, I + \beta vu)$$ |
| $$\mathrm{GL}_{2n}$$ | $$\mathrm{GL}_{2n}/\mathrm{Sp}_{2n}$$ | $$\mathrm{GL}_{2n}$$ | $$\mathrm{GL}_{2n} \times^{\mathrm{GL}_n} \mathfrak{gl}_n$$, where $$\mathrm{GL}_n$$ is embedded into $$\mathrm{GL}_{2n}$$ by $$\mathrm{diag}(g,g)$$ | $$g \mapsto \begin{pmatrix} I + \beta^2 g & \beta I \\ \beta g & I \end{pmatrix}$$ |
 $$\mathrm{PSO}_{2n} \times \mathrm{SO}_{2n+1}$$ | $$\mathrm{SO}_{2n+1}$$ | $$\mathrm{Spin}_{2n} \times \mathrm{Sp}_{2n}$$ | $$u\in \mathrm{Hom}(\mathbf{A}^{2n}, \mathbf{A}^{2n})$$ such that $$I + \beta u u^\ast$$ is invertible | $$(u,v)$$ is sent to $$(I + \beta u u^\ast, I + \beta u^\ast u)$$ |
| $$\mathrm{PSO}_{2n} \times \mathrm{SO}_{2n-1}$$ | $$\mathrm{PSO}_{2n}$$ | $$\mathrm{Spin}_{2n} \times \mathrm{Sp}_{2n-2}$$ | $$u\in \mathrm{Hom}(\mathbf{A}^{2n-2}, \mathbf{A}^{2n})$$ such that $$I + \beta u u^\ast$$ is orthogonal and $$I+\beta u^\ast u$$ is symplectic | $$(u,v)$$ is sent to $$(I + \beta u u^\ast, I + \beta u^\ast u)$$ |
| $$\mathrm{SO}_3^{\times 3}$$ | $$\mathrm{SO}_3^{\times 3}/\mathrm{SO}_3^\mathrm{diag}$$ | $$\mathrm{SL}_2^{\times 3}$$ | $$u\in \mathrm{Hom}(\mathbf{A}^2, (\mathbf{A}^2)^{\otimes 2})$$ such that $$I + \beta u u^\ast$$ is orthogonal and $$I+\beta u^\ast u$$ is symplectic | <a href = "https://annals.math.princeton.edu/wp-content/uploads/annals-v159-n1-p03.pdf">Bhargava cubes</a> (see <a href = "https://sanathdevalapurkar.github.io/files/PGL2-cubes.pdf">here</a> for elaboration) |
| (Nonsplit) $$G(\!(t)\!)$$ for $$G = \mathrm{PGL}_2$$ | $$G(\!(t)\!)/G(\!(t^3)\!)$$ | $$\mathrm{SL}_2$$ | Orbit closure in $$\mathrm{Sym}^3(\mathbf{A}^2)$$ of the parametric family $$a\mapsto ax^3+3xy^2-\beta y^3$$ | Quadratic resolvent |
| (Nonsplit) $$G(\!(t)\!)$$ for $$G = \mathrm{PGL}_2$$ | $$G(\!(t)\!)/G(\!(t^n)\!)$$, $$n>1$$ odd | $$\mathrm{SL}_2$$ | Affine cone on secant variety of rational normal curve $$\mathbf{P}^1 \hookrightarrow \mathbf{P}^n$$ (for ordinary cohomology) | Moment map on $$\mathrm{Sym}^n(\mathbf{A}^2)$$ |

**Some comments:**
In the line involving $$H \times T$$ acting on $$H$$,
$$\mathrm{QCoh}(\check{M}_\beta/\check{G})$$ is only equivalent to the full
subcategory of the corresponding geometric sheaf category which is generated
under the spherical Hecke action by the $$\delta$$-sheaf of $$X_O \subseteq
X_F$$. Similarly for the nonsplit examples above; so in these cases, we are only
talking about the *affinization* of the true ($$\mathrm{ku}$$-)Hamiltonian
space. Some of these $$\mathrm{ku}$$-theoretic analogues, like the
Gan-Gross-Prasad period (concerning $$\mathrm{SO}_{2n} \times
\mathrm{SO}_{2n+1}$$ acting on $$\mathrm{SO}_{2n+1}$$), have not yet been
written up in any public document; but they can be deduced using techniques
similar to those used in some of my work (e.g., in <a href =
"https://sanathdevalapurkar.github.io/files/PGL2-cubes.pdf">this article</a>).
The "triple product period" is a special case of the Gan-Gross-Prasad period,
corresponding to $$n=2$$.  The above table isn't comprehensive; there are other
examples, like some rank one spherical varieties, which can be found in <a href = "https://sanathdevalapurkar.github.io/files/hyperboloid_spectral_decomp.pdf">this article</a>. Also, the table clearly mostly contains only homogeneous $$G$$-spaces, and is missing other Whittaker-induced examples; this is not because there is any mathematical problem, but is rather due to my laziness.

For the examples in the above table, I have verified the
$$\mathrm{ku}$$-theoretic analogue of the first conjecture of <a href =
"https://arxiv.org/abs/2310.19770">this paper</a> (which corresponds to a part
of Conjecture 3.5.11 <a href =
"https://sanathdevalapurkar.github.io/files/hyperboloid_spectral_decomp.pdf">here</a>);
it roughly says that the set of $$B$$-orbit closures in $$X$$ is in bijection
with the set of irreducible components of $$\check{M}_\beta \times_{G_\beta}
N_\beta$$. This is an important sanity check for any candidate dual.
