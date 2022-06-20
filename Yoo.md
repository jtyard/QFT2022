# Philsang Yoo

Kevin talked about twists of 3d theories, their EOMs and geometric quantization.

The goal of this talk is to give more general context away from 3d. 

## Classical BV formalism

Input data for Lagrangian formalism of $d$-dimensional field theory
- Spacetime: $d$-manifold $M$ 
- Fields: $F = F(M)$ space of sections of a bundle over $M$
- Action functional $S : F \to C$. 

Output of classical field theory 
- $Crit(S) = \{\psi \in F :  d\psi = 0}$

Example: CS theory
- $M$ is a 3-manifold
- $F = \Omega^1(M,g)$ space of connections
- $S : F \to C$
$$A \mapsto \frac 12 \int \langle A,dA\rangle + \frac 16 \int_M\langle A,[A,A] \rangle$$

For simplicity 
- $M = pt$ (a point). 
- $F = X$ vector space (e.g. $C^n$)
- $S : X \to C$ a polynomial

Classical BV formalism = consider $Crit(S)$ in a derived manner.

$Crit(S) = Graph(dS)$ where $dS : X \to T^*X$ with $0 : X \to T^*X$ the zero section.

$$O(Crit(S)) = O(Graph(dS))\otimes_{O(T^*X)}) O(X)$$

Derived critical locus is same but with derived tensor product replacing $O(X)$ with $O(\tilde X)$

$$O(dCrit(S)) = O(Graph(dS))\otimes_{O(T^*X)}) O(\tilde X)$$?????

In coordinates, 
$O(X) = C[x^i] = C[x^1, ... , x^n]$  $O(T^* X) = Sym_{O(X)}(T_X)$

$O(X) = C[x^i,p_i] = C[x^1, ... , x^n,p_1,...,p_n]$

$O(Graph(dS)) = C[x^i,p_i]/\left(\frac{\partial S}{\partial x^i} - p_i\right)$

$O(X) \simeq O(\tilde X) = C[x^i,p_i]$??

##


$C[x^i,\xi_i]$, $deg(x^i) = 0$ and $\deg(\xi_i) = -1$. $d\xi_i = \frac{\partial S}{\partial x^i}$

$O(\tilde X) = Sym_{O(X)}(T_X[1] \oplus T_X)$

$O(dCrit(S)) = ...$

$O(T^*[-1]X) = Sym_{O(X)}(T_X[1])$ = -1-shifted cotangent space of $X$

Fact: Derived symplectic geometry: dCrit(S) always has a -1-shifted symplectic structure


Example: CS Theory $\Omega^0 \to \Omega^1 \to \Omega^2 \to \Omega^3$ (degrees -1,0,1,2)

Integrating against the CS form gives pairings 
$\Omega^0\times \Omega^3 \to C$ and $\Omega^1\times \Omega^2 \to C$ 

[He talked about this in the last workshop](https://pirsa.org/speaker/Philsang-Yoo)

Try to write in a more global langage.  EOM(M) = dCrit(S) = ??_G(M)

If we solve EOM for a surface $\Sigma$ then we get 
$$\Omega^0 \to \Omega^1 \to \Omega^2$$
It has a 0-shifted symplectic structure.

Idea can be formalized via the the AKSZ formalism.

Facts:
- If $X$ is $d$-oriented and $Y$ $n$-shifted symplectic then $Map(X,Y)$ is $(n-d)$-shifted symplectic.
- $T^*$[?]...  couldn't read it
- Fact: If M is compact oriented $d$-manifold then $M_B$ is $d$-oriented.  
In particular, $Loc_G(M) = Map(M_B,B,G)$ is 
$(2-d)$-shifted. (B = Betti)
- If $X$ is smooth proper CY $d$-fold then $X$ is $d$-oriented.  In particular, $Bun_G(X) = Map(X,BG)$ is $(2-d)$-shifted. (Algebraic category)
- If X is smooth proper variety of dimension m, then $X_dR is 2m$-oriented so that $Flat_G(X) = Map(X_dR,BG)$ is $(2-2m)$-shifted
- $X_Dol$ is $Higgs_G(X) = Map(X,???)$...

$n$-shifted symplectig $\Rightarrow$ (n+1)$-dim theory 

Ex: $X$ symplectic, $Map(M_B,X)$.  Is topological classical mechanics with target $X$.
- If $X$ is CY $n$-fold, then $Map(\Sigma_B,T^*[1]X)$ is the B-model 

$Map(M_3,BG)$ is CS Theory

$Map(M_B \times X,BG)$ is 4d, 5d, (6d aka holomorphic) CS Theory.  M CPT oriented, X CY.

$Map(M_B^3,X)$ is Rozansky-Witten theory $Z/2$-graded.


## TQFT

In the sense of Atiyah-Singer.  
- $d=2$, $Z: Bord_2 \to Vect_C$ classified by commutative (can move holes around) Frobenius algebras $Z(S')$ (plugging together pants)
- Extended TQFT: $Bord_2 \to Cat_C$ $Z(pt)$ = category of boundary conditions
- $Z(-,B_1,B_2)$ = space of open string states satisfying boundary conditions $B_1,B_2 \in Z(pt)$ at the ends.

Note 
- $Z(S^{d-1}) \in E_d-alg(Vect_C)$ = the space of point operators
- $Z(S^{d-2}) \in E_{d-1}-alg(Cat_C)$ = the space of line operators 
- $Z(S^1)$ = space of closed string states 

Ex: B-model with target X
- $Z_B(pt) = Coh(X)$ (derived category of cohreent sheaves on X)
- $Z_B(X^1) = HH_*(Coh(X)) = \Omega(X)$ (differential forms on X)

Ex: CS Theory
- $Z_{CS}(S1) \in E_2-alg(Cat_C)$ = braided monoidal categories = category of line operators of CS theory


## From BV to TQFT

Elliot-Yoo, Safranov, Hilburn-Yoo

The idea is to geometrically quantize $EOM(-)$ to get $Z(-)$

For example, 
- $EOM(N^{d-1}) \to Z(N)$ (0-shifted symplectic to vector space)
- $EOM(Y^{d-2}) \to Z(Y)$ 1-category

Ex: B-model 
- $EOM(\Sigma) = Map(\Sigma_B,T^*[1]X)$
- $EOM(pt) = T^*[1]X \to Coh(X)$ (because it is 1-shifted you should expect to see a category not functions)
- $EOM(S^1) = Map(S^1_B,T^*[1]X) \simeq T^*(T[-1]X) \to O(T[-1]X) = \Omega(X)$


This sort of machinery will not help answer what is Z_CS(pt).  It is hard because 
 $EOM_{CS}(pt) = BG$