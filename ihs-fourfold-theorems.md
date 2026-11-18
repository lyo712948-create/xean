# Selected results on compact irreducible holomorphic symplectic fourfolds

These statements come from the first two runs of the classification project, completed on 18 November 2026. They give a sufficient criterion for Hilbert-square type, describe what the integral intersection data can and cannot force, and settle the outcome of two specified families of torus quotient constructions. The full deformation classification remains unresolved by these results. The cited papers supply established inputs and identify known overlaps. Priority for the remaining statements has not been established.

Throughout, an **IHS fourfold** is a simply connected compact Kähler manifold of complex dimension four whose holomorphic two-forms are spanned by a nondegenerate form. Projectivity is not assumed. The two deformation types referred to below are the Hilbert square $S^{[2]}$ of a K3 surface and the generalized Kummer fourfold $K_2(A)$, the zero fiber of the summation map $A^{[3]}\to A$ for a complex two-torus $A$. In the quotient statements, a *symplectic resolution* is a proper holomorphic resolution on which the symplectic form of the smooth locus extends to a nondegenerate holomorphic two-form. [Beauville, *Variétés Kähleriennes dont la première classe de Chern est nulle*](https://math.univ-cotedazur.fr/u/beauvill/pubs/jdg.pdf) and [Beauville, *Surfaces K3*](https://www.numdam.org/item/AST_1985__126__181_0/).

## 1. Sharp determinant thresholds and a criterion for Hilbert-square type

**Theorem.** Let $L$ be a nondegenerate even integral lattice of signature $(3,n-3)$, where $n\in\{5,6,7,8,23\}$. Use the following bounds.

| Rank $n$ | $5$ | $6$ | $7$ | $8$ | $23$ |
| --- | ---: | ---: | ---: | ---: | ---: |
| $T_n$ | $32$ | $64$ | $128$ | $192$ | $2^{23}$ |

If $\lvert\det L\rvert<T_n$, then $L$ contains an orthogonal direct summand isometric to the integral hyperbolic plane $U$. Thus there are $e,f\in L$ with $q(e,e)=q(f,f)=0$ and $q(e,f)=1$, where $q$ is the bilinear form on $L$. For each listed rank there exists an even lattice of the same signature whose bilinear form is primitive, whose absolute determinant is $T_n$, and which contains no such summand. Here primitive means that the pairings $q(x,y)$ generate $\mathbb Z$.

**Corollary.** Let $X$ be a smooth compact IHS fourfold. Write $q_X$ for its primitive integral bilinear Beauville–Bogomolov–Fujiki form on $H^2(X,\mathbb Z)$, $D_X=\lvert\det q_X\rvert$, and $c_X$ for the Fujiki constant in the normalization

$$
\int_X x^4=c_X q_X(x,x)^2.
$$

Suppose $b_2(X)=n\ge 5$, $c_X=3$, and $D_X<T_n$. Then $X$ is deformation equivalent to a K3 Hilbert square. In particular,

$$
b_2(X)=23,\qquad c_X=3,\qquad D_X<2^{23}
\quad\Longrightarrow\quad X\text{ is of }\mathrm{K3}^{[2]}\text{ type}.
$$

There is no square-class condition on $D_X$. For $n=5,6,7,8$, the hypotheses of the corollary are incompatible with $b_2(X)=n$, since Hilbert-square type has $b_2=23$.

The lattice bound gives integral classes $l,m$ with $q_X(l,l)=q_X(m,m)=0$ and $q_X(l,m)=1$. Polarized Fujiki then gives $\int_X l^4=0$ and $\int_X l^2m^2=2$, the exact hypotheses of the published deformation criterion. The determinant threshold is sharp for even lattices. Applying it to an arbitrary fourfold would also require a geometric argument for the hypotheses on $c_X$ and $D_X$. [Guan, *On the Betti numbers of irreducible compact hyperkähler manifolds of complex dimension four*](https://archive.intlpress.com/site/pub/files/_fulltext/journals/mrl/2001/0008/0005/MRL-2001-0008-0005-a008.pdf) and [Debarre–Huybrechts–Macrì–Voisin, Theorem 1.5](https://arxiv.org/abs/2201.08152v3).

*Campaign notes from round 2: w71.2–w71.4.*

## 2. The exact spectrum of isotropic mixed intersections

**Theorem.** Let $(L,q)$ be a nondegenerate integral symmetric bilinear lattice of rank at least three, with a nonzero isotropic vector in $L\otimes\mathbb Q$. Write $D=\lvert\det q\rvert$. For a prime $p\mid D$, let $L_p=L\otimes\mathbb Z_p$ and set

$$
S_p=\{s\in\mathbb Z_{\ge 0}:\text{ there is a primitive }u\in L_p
\text{ with }q(u,u)=0\text{ and }q(u,L_p)=p^s\mathbb Z_p\}.
$$

A vector is primitive if its coordinates generate the coefficient ring. Each $S_p$ is nonempty and contained in $\{0,\ldots,\lfloor v_p(D)/2\rfloor\}$, where $v_p(D)$ is the exponent of $p$ in $D$. The divisibilities of primitive integral isotropic vectors are exactly

$$
\left\{\prod_{p\mid D}p^{s_p}:s_p\in S_p\text{ for every }p\mid D\right\}.
$$

Here the divisibility of $l$ is the positive generator of $q(l,L)$, and the choices of $s_p$ are independent. In particular, $d_*=\prod_{p\mid D}p^{\min S_p}$ is attained, and the set of pairings $q(l,m)$ with $0\ne l\in L$ isotropic and $m\in L$ is exactly $d_*\mathbb Z$. An empty product is $1$.

**Corollary.** Let $X$ be a smooth compact IHS fourfold with $b_2(X)\ge 5$. Use $(H^2(X,\mathbb Z),q_X)$ in the theorem and define $A_{\min}=(c_X/3)d_*^2$. Then $A_{\min}$ is a positive integer. For $l,m\in H^2(X,\mathbb Z)$ with $l\ne 0$ and $\int_X l^4=0$, the positive values of

$$
a(l,m)=\frac12\int_X l^2m^2
$$

are exactly $A_{\min}k^2$ for integers $k\ge 1$. If $A_{\min}\le 8$, the triple $(A_{\min},c_X,d_*)$ belongs to

$$
\{(1,3,1),\ (3,9,1),\ (4,3,2),\ (4,12,1)\}.
$$

The first triple forces $\mathrm{K3}^{[2]}$ deformation type. The other triples are necessary numerical alternatives under the bound $A_{\min}\le 8$. The result gives an exact local description of the obstruction to finding the two integral classes required by the published criterion. [Debarre–Huybrechts–Macrì–Voisin, Theorem 1.5](https://arxiv.org/abs/2201.08152v3).

*Campaign notes from round 1: w9.1–w9.2.*

## 3. Formal Poincaré duality rings with the Hilbert-square numerical data

**Theorem.** Fix a K3 Hilbert square $X_0$ and write $R_0=H^*(X_0,\mathbb Z)/\mathrm{torsion}$. Its second cohomology lattice is

$$
L_0=U^{\oplus 3}\oplus E_8(-1)^{\oplus 2}\oplus\langle-2\rangle
$$

with bilinear form $q_0$. Here $E_8(-1)$ is the negative definite even unimodular lattice of rank eight. For each prime $p$ there is a sublattice $M_p\subset L_0$ of index $p^{11}$ with the following properties.

1. The unrescaled restriction $q_p=q_0|_{M_p}$ is primitive and even, has signature $(3,20)$, and has absolute determinant $2p^{22}$. The smallest divisibility of a nonzero primitive isotropic vector in $M_p$ is $p$. Every sublattice of $L_0$ of index $p^j$ with $0\le j\le 10$ contains $U$ for the unrescaled form.
2. There exists a graded integral Poincaré duality ring $R_p$ of degree eight, concentrated in degrees $0,2,4,6,8$, with ranks $1,23,276,23,1$ in those degrees. It has $R_p^2=M_p$, the same oriented rational graded ring as $R_0$, and the same integral middle intersection lattice as $R_0$.
3. The images of $c_2(X_0)$ and $c_4(X_0)$ define labels $\gamma_2\in R_p^4$ and $\gamma_4\in R_p^8$. With the top-degree functional $\int$ inherited from $R_0$, they satisfy, for all $x,y\in M_p$,

   $$
   \int x^4=3q_p(x,x)^2,\qquad
   \int\gamma_2xy=30q_p(x,y),\qquad
   \int\gamma_2^2=828,\qquad \int\gamma_4=324.
   $$

   The associated formal Riemann–Roch polynomial is $P(t)=\binom{t/2+3}{2}$, and $P(q_p(x,x))$ is integral for every $x\in M_p$.
4. The positive half-mixed intersections $\tfrac12\int l^2m^2$ with $0\ne l,m\in M_p$ and $\int l^4=0$ are exactly $p^2k^2$ for integers $k\ge 1$.

For odd $p$, choose an eleven-dimensional totally isotropic subspace $W$ of $L_0/pL_0$ containing the reduction of a fixed hyperbolic basis vector. Take $M_p$ to be the inverse image of $W^\perp$. For $p=2$, choose hyperbolic pairs $e_i,f_i$ for $1\le i\le 3$, a generator $\delta$ of $\langle-2\rangle$, and corresponding bases $z_j,z'_j$ of the two $E_8(-1)$ summands. Take

$$
M_2=2L_0+
\left\langle e_1+f_1,\ e_1+e_2+f_2,\ e_2+f_2+\delta,\ e_3,\
z_j+z'_j\ (1\le j\le 8)\right\rangle_{\mathbb Z}.
$$

The ring $R_p$ is obtained inside $R_0\otimes\mathbb Q$ by replacing $R_0^2$ with $M_p$ and $R_0^6$ with the lattice dual to $M_p$ under the top pairing, keeping all other degrees and inheriting the products.

These examples show that the displayed ranks, middle pairing, Chern-number identities and Riemann–Roch integrality do not force a unit isotropic pairing. In particular, the $p=2$ formal example attains determinant $2^{23}$ with least positive half-mixed intersection $4$. The construction is in the category of graded rings. Realization by a smooth manifold with the stated tangent Chern classes, let alone by an IHS fourfold, would require additional arguments.

*Campaign notes from round 1: w3.3 and w9.3–w9.4.*

## 4. Symplectic resolutions for full surface wreath actions on four-tori

**Theorem.** Let $\Gamma$ be a finite group acting faithfully by affine holomorphic automorphisms on a compact complex four-torus $T$. Assume its derivative image is the full wreath product

$$
H\wr S_2=(H\times H)\rtimes S_2
$$

on $E\oplus E$, where $E$ is a two-dimensional complex vector space, $H$ is a finite subgroup of $\mathrm{SL}(E)$, the two factors of $H\times H$ act separately, and the transposition exchanges the copies of $E$. Equip $E\oplus E$ with the sum of the two copies of a nonzero determinant form on $E$. Write $N$ for the kernel of the derivative homomorphism, a finite group of translations.

1. If $H$ is nontrivial, then up to complex linear conjugacy it is one of

   $$
   C_2,\ C_3,\ C_4,\ C_6,\ Q_8,\ \mathrm{Dic}_3,\ T_{24}.
   $$

   Here $C_j$ is cyclic of order $j$, $Q_8$ is quaternion of order eight, $\mathrm{Dic}_3$ is binary dihedral of order twelve, and $T_{24}$ is binary tetrahedral of order twenty-four.
2. If $H$ is nontrivial, every Kähler symplectic resolution of $T/\Gamma$ is a smooth compact IHS fourfold of $\mathrm{K3}^{[2]}$ deformation type.
3. If $H$ is $C_6$, $\mathrm{Dic}_3$, or $T_{24}$, the induced affine action on $T/N$ splits. More precisely, there is an affine identification $T/N\simeq A^2$ for a complex two-torus $A$ under which the action is the product of two copies of an affine $H$-action on $A$, together with factor exchange. If $S$ is the K3 surface obtained by minimally resolving $A/H$ for this surface action, then the map

   $$
   S^{[2]}\longrightarrow \operatorname{Sym}^2(A/H)\simeq T/\Gamma
   $$

   supplies a compact Kähler symplectic resolution. The affine action on $A$ can be used without requiring a common fixed point.
4. If $H$ is trivial, every compact Kähler resolution of $T/\Gamma$ has a holomorphic map of generic rank two to a two-dimensional complex torus. It has at least two independent holomorphic one-forms and cannot be IHS.

Part 2 rules out a third deformation type from a Kähler symplectic resolution in this representation family. Part 3 guarantees existence for the three stated groups. The surface group list and the local Hilbert–Chow construction have published antecedents. [Fujiki, Lemma 3.3 and §3.4](https://ems.press/journals/prims/articles/3404) and [Fu–Namikawa, Example 2.7](https://doi.org/10.5802/aif.2008).

*Campaign note from round 2: w89.1 and its supporting results.*

## 5. The doubled standard dihedral actions

**Theorem.** Let $\Gamma$ be a finite group acting faithfully and affinely on a compact complex four-torus $T$, preserving a translation invariant holomorphic symplectic form. Suppose its derivative image is the dihedral group

$$
D_{2m}=\langle r,s\mid r^m=s^2=1,\ srs=r^{-1}\rangle
$$

of order $2m$, with $m\ge 3$, in the direct sum of two copies of its faithful two-dimensional standard representation. Thus $r$ has eigenvalues $\zeta_m,\zeta_m^{-1}$ on each copy, for a primitive $m$-th root of unity $\zeta_m$. Write $N$ for the finite translation kernel and $T'=T/N$. Then $m\in\{3,4,6\}$, and the following alternatives hold.

### Order six ($m=3$)

The induced $S_3$-action on $T'$ has a common fixed point. There is a complex two-torus $A$ and a subgroup $C\le A[3]$, with $\lvert C\rvert=3^k$ and $0\le k\le 4$, such that after moving the common fixed point to the origin the action is equivariantly isomorphic to coordinate permutations on $B(A)/C_{\mathrm{diag}}$, where

$$
B(A)=\{(x,y,z)\in A^3:x+y+z=0\},\qquad
C_{\mathrm{diag}}=\{(c,c,c):c\in C\}.
$$

The quotient $T/\Gamma$ admits a symplectic resolution if and only if $C=0$. In that case the generalized Kummer map $K_2(A)\to B(A)/S_3$ is one such resolution, and every Kähler symplectic resolution is a smooth compact IHS fourfold of $\mathrm{Kum}_2$ deformation type.

If $k>0$, there are exactly $(81-3^{4-k})/2$ isolated singularities, each of type $\mathbb C^4/\mu_3$ with a generator acting by $\operatorname{diag}(\zeta_3,\zeta_3,\zeta_3^{-1},\zeta_3^{-1})$. The respective counts are $27,36,39,40$ for $k=1,2,3,4$. The quotient admits neither a symplectic resolution nor a flat analytic one-parameter smoothing.

### Order eight ($m=4$)

The quotient $T/\Gamma$ admits a symplectic resolution exactly when both of the following conditions hold.

1. The induced $D_8$-action on $T'$ has a common fixed point.
2. After moving that point to the origin, write the resulting linear action on

   $$
   (A\times A)/\{(c,\theta(c)):c\in C\}
   $$

   for a complex two-torus $A$, a subgroup $C\le A[2]$, and an automorphism $\theta$ of $C$ with $\theta^2=\operatorname{id}$. The group is generated by $(x,y)\mapsto(-x,y)$ and $(x,y)\mapsto(y,x)$ on this quotient. In this normal form, either $C=0$, or $C=A[2]$ and $\theta=\operatorname{id}$.

In the two allowed cases, $T/\Gamma$ is isomorphic to $\operatorname{Sym}^2(A/\{\pm1\})$. If $S$ is the Kummer K3 surface of $A$, the map $S^{[2]}\to T/\Gamma$ gives a compact Kähler symplectic resolution, and every Kähler symplectic resolution is IHS of $\mathrm{K3}^{[2]}$ type. If either condition fails, there is also no flat analytic one-parameter smoothing.

### Order twelve ($m=6$)

The induced action on $T'$ has a common fixed point. Its central involution acts as $-\operatorname{id}$ after moving that point to the origin. Exactly $210$ of its $256$ fixed points have stabilizer consisting only of the identity and the central involution. They give exactly $35$ isolated points of $T/\Gamma$ with germ $\mathbb C^4/\{\pm 1\}$, where $-1$ acts as minus the identity on all four coordinates. Other singularities may occur. The quotient admits neither a symplectic resolution nor a flat analytic one-parameter smoothing.

The obstruction statements apply even to resolutions whose source is not Kähler. The conclusions on deformation type concern Kähler resolutions, including nonprojective ones. Earlier work established cohomological results for the order-six and order-eight representations. The statements here specify affine normal forms, existence conditions, and the deformation types of the Kähler resolutions under the given hypotheses. [Andreatta–Wiśniewski, Theorems 6.2 and 6.4](https://arxiv.org/abs/0804.4611v2). The deformation comparison uses the theorem for bimeromorphic compact Kähler IHS manifolds. [Huybrechts, Theorem 2.5](https://arxiv.org/abs/math/9909109v2).

*Campaign notes from round 2: w76.2–w76.3, i82.1, w83.1–w83.5, and i85.1–i86.1.*
