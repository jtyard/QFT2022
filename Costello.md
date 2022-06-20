# Costello Intro to twisted theories

Usual pattern: mysterious duality between SQFTs maps to a math conjecture.  

$Spin(3,1) = SL_2(C)$.  Spin representation $S = \bC^2$ and vector representation $Sym^2 S$.


$Q^2 = \frac 12 [Q,Q] = 0$ means it is a dirfferential.  Twisting replaces everything in the QFT by its $Q$-cohomology.

H = Hilbert space of QFT, $H^*(\script{H},Q)$ is Hilbert space of twisted theory.

What kind of thing is the twisted theory?  How do loop operators in the twisted theory behave?  As $Q$ is a symmetry, correlation functions of $Q$-closed operators descend to $Q$-cohomology.

For $O_1,\dotsc,O_n \in H^*$(local operators,$Q)$,
what kind of functions are $\langle O_1(x_1)\cdots O_n(x_n)\rangle$.  Witten found that $4d$ $N=2$ theories these don't depend on position.  But in 3d some coordinate dependence is left. 

$[Q,Q_2^\alpha] = \frac{\partial}{\partial x_{1\alpha}}$ so the vector fields $ \frac{\partial}{\partial x_{1\alpha}}$ are exact.  Null for 11, real for 12.  We can choose new coordinates $t,z,\bar z$ with $z = x+iy$
on $R\times C$ so that 
$\frac{\partial}{\partial x_{11}}  = \frac{\partial}{\partial \bar z}$ and 
$\frac{\partial}{\partial x_{1\alpha}}= \frac{\partial}{\partial t}$.

On $Q$-cohomology, correlation functions re topological in $t$ while holomorphic in $z$ and $\bar z$.

## 

Data of a 3d N=2 theory:

- Group $G$
- Representation $R$ of $G$
- $G$-invariant function $W \in \scriptO(R)^G$
- CS level in $H^4(BG)$

We will write a Lagrangian for twisted theory based on this.  We start with pure gauge theory ($R = 0$).  HEre, fields of the twisted theory are those that do not contain the twisted component
 $A \in \Omega^1(R\times C)/dz)\otimes g$ where $A = A_t dt + A_{\bar z} d\bar z$.

 There's also $B\in dz \Omega^0(R\times C)\otimes g^*$.  Lagrangian is just 

 $$\int BF(A) + K_{CS}\int A\partial A$$

 will ignore the second term for this first lecture and set $K_{CS} = 0$.

 In this case, what are the EOMs?  
 - Vary $B$ to get $F_{t\bar z}(A) = 0$.  
 - Vary $A$ to get $d_AB = 0$

 In Euclidean signature $\bar z$ is not a "real" coordinate (what kind of real??)

 At each timestep $t$ $A|_{C\times t}$ defines a holomorphic bundle.  If we parallel transport from $t=t_0$
 to $t=t_1$ using $A_t$, then the first eqn tells us that this is an isomorphism of holomorphic bundles.  For ecample if $G = GL_n$ and $\psi \in C^n$ the vector representation then $(\partial_{\bar z} + A_{\bar z})\psi(z,t_0)$.  Define $\psi(z,t)$ b parallel transport $(\partial_{\bar z} + A_{\bar z})\psi(z,t) = 0$
as $(\partial_t + A_t)(\partial_{\bar z} + A_{\bar z})\psi(z,t) = 0$.

## 

What happens when we introduce matter?  Let's set the superpotential $W = 0$ for now.  Fields of the twisted theory are $\phi\in \Omege^0(R\times C,R)$ with $\eta \in (dz \Omega^1(R\times C)/dz) \otimes R^*$????

Lagrangian is $\int \eta d\phi + \int BF(A) + K\int A\partial A$, $\eta = \eta_{zt} + \eta_{z\bar z}$.  Funny feature:  although this is just matter, it has a gauge symmetry $\eta \to \eta + d_A \chi$, where $|chi \in dz \Omega^0(R\times C)\otimes R^*$.  Easy to see using EOMs of for A that this (what?) is the gauge symmetry of this Lagrangian.

How can you see things like the affine Grassmannian appear in these 3d N=2 theories. 

## Hilbert spaces of local operators 

General CFT/QFT yoga: In any classical field theory in dimension $d$, if $M$ is a closed $d-1$-manifold then the space of solns to the EOMs on $M\times (-\epsilon,\epsilon)$ is a symplectic manifold (typically infinite dimensional).  Hilbert space is obtained by carefully performing geometric quantization.

Get that the local operators is the Hilbert space on the 2-sphere $S^2$.  Easier: local operators on the boundary, with boundary conditions $A = 0$ (Dirichlet boundary conditions).  For now pure gauge.  Hilbert space on the disc ending on the boundary.  

##

Phase space is the cotangent bundle of the affine grassmannian.

Want to study the space of solns to the EOMs on a disc on the boundary (draws a long tube with one end glued to a plane).  $t=0$, $C\times R_{\geq 0}$, $A=0$ at $t=0$
$|z|= 1$ and $0\leq t \leq 1$ union $|z| \leq 1$, $t=1$.

Solns: A: at $t=1$ holomorphic bundle on disc.  At $t=0$, trivial bundle on bounary of the disc. $0\leq t \leq 1$ get an isomorphic between these.  $\Rightarrow$ a $G$-bundle on $D$ trivialized on $\partial D$.

$= LG/Hol(D,G)$

If we want really local operators, we should take $D$ very small in which case we replace Hol(D,G) by the Taylor expansion $G[[z]]$ and $LG \to G((z))$  
and this becomes the affine Grassmannian $Gr_G = G((z))/G[[z]]$.

B: No constraints at the boundary $t=0$.  $B \in dz Hol(D,g^*) - dz g^*[[z]]$ (if A trivial, or better a section on the disc $D$ of $K\otimes $ the associated bundle for $g^*$.)
$B \in T^*_A Gr_G$ is now inthe cotangent bundle.  LEt's check the tangent space at the origin $T_0 Gr_G = z^{-1} g[[z^{-1}]]$ (it contains only the purely negative loops) and is dual to $dz g^*[[z]]$ 
using residues.

So the phase space is $T^* = Gr_G$.  

We know from geometric Langlands that sheaves on the affine grassmannian should make an appearance.  It can be derived in this context.

