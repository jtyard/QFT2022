# 3d theories and twists II

Physical scenarios mapped to mathematical structures such that physical dualities mapped to conjectures relating such structures. 

Want to find some intermediate mathematical field/string theory.  Some kind of S-sector or cohomological structure is often enough. 

Once we have a mathematical definition of some BPS sector of the theory we an start defining the objects more precisely than in the purely physical scenario. 


-4d N=4 has EM duality and a topological twist -> geometric Langlands 
-4d N=2 has webs of EM-like dualities has holomorphic topological twist -> Seiberg-Witten geometry, Hitchin systems, Kontsevich-Soibelman wall crossing, VOAs, AGT correspondence. 
- 3d N=4 has 3d mirror symmetry -> after a topological twist expect to find a lift of homological mirror symmetry and applications to knot homology, applic and extensions of symplectic duality.  Holomorphic-topological twists of 3d N=4 gives elliptic cohomology in hyperkahler setting (explained by Dedushenko-Nekrasov...)
- 3d N=2 doesn't have a topological twist.  It has vast big webs of dualities.  Has a HT twist.  Elliptic cohomolgy of hyperkahler spaces.  Topological invariants $T[M^3]$ of 3-manifolds 3d-3d correspondence.  Categorification of quantum invariants of 3-manifolds. 

## 3d N=2
Spinors in 3d are 2d.  SUSY algerba enerated by two  

$Q_\alpha, \bar Q_\alpha$ where $\alpha = 1$ and $2$.

Pauli matrices are interwtiners between two copies of the spinor representation and the vector representation 

$$[Q_\alpha, \bar Q_\beta]_+ = \sigma_{\alpha\beta}^\mu \partial_\mu$$

On $C_z \times R_t$ these are 

$$[Q_+, \bar Q_+]_+ = \partial_{\bar{z}} $$ 

$$[Q_-, \bar Q_-]_+ = \partial_z $$

$$[Q_+, \bar Q_-]_+ = [Q_-, \bar Q_+]_+ = \partial_t$$.

SUSY algebra is infinitesimal symmetry of fields (embeds into Fields).  Thus acts on operators that can be thought of as functions $O_F$ of the fields.
In particular, SUSY acts on local operators
$Ops_{z,\bar z,t}$ = functions on the [infinite jet space](https://en.wikipedia.org/wiki/Jet_bundle#Infinite_jet_spaces) of fields at $z,\bar z, t$.  These are the basic thing that enters correlation functions. 

HT twist <-> $Q = \bar Q_+$ cohomology.

Upshot: Correlation functionf of Q-closed operators only depend holomorphically on $z$.
- Q-cohomology of the bulk local operators Ops becomes a commutative (no singularities) shifted Poisson vertex algebra.  Correlation functions only depend on $z$ (not $\bar z$.)  
$\lim_{z\to w} \phi_q(z) \phi_2(w)$
- GIven a BC B for $R_+\times C$ (along the complex direction), get a potentially nonsingular = noncommutative vertex algebra $V_B$.  There is a bulk-boundary map and the things that commute come from the bulk.  
$\beta_B : V \to Z(V_B)$.


- $V$ and $V_B$ are graded by spin $Z$.  This means rotations in $C$ around the support of a particular operator.  This plays the role of a conformal grading.
- If lucky also graded by $R$-charge corresponding to additional U(1) symmetry that extends the SUSY algebra in the sense that $deg(Q_\alpha) = -1$ and $deg(\bar Q_\alpha) = 1$.  Upshot is that we use $Q$ as a differential.  This will be a (co)homological degree. 
- Characters $\chi(V) = Tr_V(-1)^R q^J$ "3d index"
- $\chi(V_B) = Tr_{_B} (-1)^R q^J$ "3d half-index".  Intimimately related to the sort of theta functions that show up in elliptic cohomology.  
SHeaf of Hilbert spaces over a dual elliptic curve having to do with global symmetries.  To produce classes in elliptic cohomology, or states in the hilbert space, fix a boundary condition. Whole "elliptic cohomology stable envelope game" $E\times R$. 

"Holomorphic flavor connection on an elliptic curve".

- Line operators form a dg-category.  GIven lines L and L', the junction between them is in Hom(L,L').  Coposition is along the topological (z) direction.  V = End_V(I) and expect that 
$HH_*^{spin}(C)$ should equal equivariant quantum K-theory. But this category has not yet been defined except in trivial examples.  But there are some obvious guesses.  Roughly K-theory of coherent sheaves on the loop space of the category. 

Given a variety X that appears as the stable locus of the stack V/G then we expect it to be the quantum K-theory of X. 

Lines can also collide with each other in the z-direction.  While you might think that would lead to singularities, it turns out that 

- Given a correlation function in the presence of two line operators at z and w.  What happens as z -> w?  Is i singular or not? Turns not not as it is locally constant.  Correlations of configurations that are time independent are also independent of z.  Operators preserve 
$\bar Q_+$ and $Q_- $.  
Note that $[\bar Q_+,Q_-]_+ = \partial_t$. $\tilde Q = \bar Q_+ + Q_-$ squares to $\partial_t$ so can also be used as a differential. 
Also equals $\tilde Q,\bar Q_-]_+$.  

Expect meromorphic tensor category.  This is analogous to giving you harmonic forms.  GIven 3 line operators L parallel to L' joined to L'' can eb re-expressed as a sum over $(z-w)^{-n}$ times the correlation function of the single line $L\otimes L'$ joined to $L\otimes L''$ by a junction $a^{(n)}$.

## Examples from 3d N=2 gauge theory

data: $G$ reductive, $V$ complex , W:V/G -> C, $k\in H^4(BG)$.

Or can ignore $G$ for easier example.  Chiral multiplets valued in V.  Twisted BV formalism: $\Phi \in V[d\bar z, dt] dz^j$
$\Psi \in V^*[d\bar z,dt] dz^{1-j}[1]$ (shifted)
Kevin wrote something similar $\int \eta d'\phi$ where $d' = \partial_{\bar z} dz + \partial_t dt$. Related to this lecture via 
$\Phi = \phi + ...$, $\Psi = \psi + \eta^{(1)} + ...$

BV action $S = \int \Psi d' \Phi + W(\Phi)$ 

## BV rules
Space of fields is  [-1]-shifted symplectic, which means functions on fields has a degree +1 Poisson bracket defined to give $\delta^{(3)}(x-x')$ on $\Phi(x)$ and $\Psi(x')$

Q = {S,-}
Q^2=0 <-> {S,S}= 0