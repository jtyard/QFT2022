# Langlands duality for periods and L-functions via E-M duality

w/ Sakellardis and Venkatesh

What is the spectral version of periods of automorphic forms?  Will propose an answer inspired by S-duality.

Givenm a holomorphic moduilar form, can compute its period integrals. N-period measures the constant term a0 so it tells you if it's a cusp form.  (N,psi)-period or Whittaker period measures the linear term a1.  The "T-period" integrates the form along the vertical axis (maybe against a character) giving the Mellin transform i.e. the Dirichlet series associated to the form.  

Langlands correspondence takes Hecke eigenform to a 2d Galois rep.  a0 = 0 means rho is irreducible.  a1 corresponds to constant function 1  (Whittaker normalization).  Dirichlet series gives the L-function L(rho,s) = prod det(1-p^{-s} rho(Fr_p)).  We're just gonna look at the value at s=0 in this talk.  L(rho = 0,s) = zeta(s).  Then zeta(0) = -1/2 (number of positive integers).  If you can write your L-function as the period of a modular form then you get a lot of other properties.  

What is the science behind matching of L-function and periods?  Answer: BZ-S-V periods are boundary conditions for the 4d A-model A_G.  L-functions are boundary condition for the 4d B-model B_{G^v}.  Matching the hamiltonian invariants between the two groups.

Langlands d'apres' Kapustin-Witten.  G = complex reductive group and its Langlands dual G^v.  

A_G(Sig) = Shv(Bun_G(Sig)) ~ D-mod on Bun_G~ Fuk(T^*(Bun(Hitchin)))

B_{G^v}(Sig) = QC(Loc_G^v(Sig)) (ind-coherent)

Key features: matches action of defect operators on two sides: local, line, surface operators (codim 4,3,2).

- Local operators H^*(BG), <-> O(G^*[2]/G)
- Line operators (main thing) 't Hooft <-> Wilson (matching of Hecke operators)
- Surface operators adding ramification (ramified version of the Langlands corresponce)  So now Bun_G replace with bundles with level struicture.  <-> local systems + singularities


## 
Richest story: codim 1

Gaiotto-Witten, Hilburn-Yoo.  Boundary conditions and interfaces - i.e. BC for a product group can be seen as an interface between them.

Examples come from quantizations of hyperkahler G/G^v spaces.  3d A/B model coupled to 4d.  

Hamiltonian action of G on M holomorphic symplectic, graded Hamiltonian action on g*.  Leads to Gaiotto Lagrangian:

Bun_G,M = jets of G-bundles + 1-form valued section 

Image of Bun_G,M -> T*Bun_G defines Lagrangian in the moduli space of Higgs bundles and underlies a BAA brane in A_G(Sig).  Spectral Gaiotto Lagrangian: BBB brane on Loc_Gv 
Loc_Gv,Mv = Gv-loc systems + flat section of Mv-bundle.

Loc_Gv,Mv -> T*[1]Loc_Gv (quantization is coherent sheav on Loc_Gv)

Simplest example: O_Loc, Mv = pt (Neumann) i.e. Gamma_Loc(-1) (functor of taking global sections of cohere sheaves) <-> Hitchin section of the Hitchin integrable system = Whittaker sheaf in the GL literature, or has to do with principle Nahm pole BC in Witten

M = T*G//_psi N for a nondegenerate character psi of the group of upper triangular matrices. 

Davide had an insight: move to a trivial point in the moduli space where the gauge group breaks down to a torus.  Then you have the abelian theory on one side and the original one on the other.  N is not a brane: it is just a displacement of the D3-branes.

##

How to match the story with number theory:

Dictionary: MMMR  Mazur, Mumford, Morshida,... ?? Knots and primes dictionary.

F = global field.  Think of Spec O_F as a noncompact (because of non-archimedean places) unoriented 3-manifold. Local fields are 2-manifolds.  

G/F reductive group.  $Bun_G = [G]_F$  really need to fix a level structure along a linik in your 3-manifold.  What is Bun_G?  Not an algebraic stack.  

Finite field: Bun_G(Sig)(F_q)
Number field: arithmetic locally symmetric space 
G_Z\G_R/K e.g. PSL_2 Z\ H.  There is an adelic double quotient 
G(F)\G(A_F)/G(O_AF).  

A_G: Study C-linearization of Bun_G (e.g. H*(something))

Loc_Gv: character stack of Galois reps into Gv/C.

B_Gv: Algebraic functions/distribuitions on the character variety Loc_Gv

Langlands says A_G(*F) simeq B_Vv(F) as modules over Hecke algebras.  Automorphic forms live on the A-side.  

Local Langlands: K a local field.  G(K)-reps a subcategory of A_G(K).  B-side??

Where to periods sit here?  Give H subset G, Bun_H subset BunG. 

Define H-period of automorphic form as integral over Bun_H (again maybe with a character).  Replace H with X = G/H and consdider X-periods.  Bun_G = G(F)\G(A)/G(O_A)
X(A)/G(O_A) = prod X(K )/G(O)
Related by a correspondence (not a map).

Theta-series operator is intertwiner 

Theta: L^2(prod X(A)/G(O_A)) -> L^2(Bun_G)

period: pairs phi on RHS with test function on LHS

Riemann wrote completed zeta(s) (i.e. times Gamma pi..) as Mellin transform (integrate against a gaussian, which is because it corresponds to a manifold with boundary).  Iwasawa, Tate: Abelian L-functions are periods: integrate againsts Theta series of test function for G = G_m (mult group).

Bun_G,X -> Bun_G
P_X...??
X-period sheaf exactly quantizes the Gaiotto Lagrangian for M = T*X.

Tate's thesis: functional equation for Riemann zeta comes from the Fourier transform on A^1 (which is technically a symmetry on T*A^1) which is why you want periods to be indexed by Hamiltonian spaces. 

## 

Spherical varieties (G acting on X) are the nonabelian version of toric varieties.  For G a torus they are toric.  

Need G supset B to have an open orbit on X.  

In affine case (over alg closed field) need k[X] to be multiplicity-1. Looking at loop space of L_X, need discrete orbits of L_G+ (e.g. geometric Satake).  Other things that appear: toric, flag G/N as a GxT space, symmetric spaces G/K, GxG acting on G, multiplicity-1 restriction problems for classical groups (GL_n x GL_{n-1} acting on GL_n - or SO = Gan-Gross-Prasad program).  Hecke PGL_2 / T.

Davide and Sascha wondering what the spherical condition means physically.  Like does it maybe make the dual smaller?  Microlocal version X -> M -> g* with G action.  Spherical: coisotropic mult/one.  
$k[M]^G$ Poisson commutative.  hyperspherical varieties = nonabelian generalization of hypertoric varieties.  Includes Whittaker and Nahm pole case, which includes twisted version.  In number theory there is a Theta correspondence where you can look at symplectic representations of groups that are not polarized.

Structure theorem BZSV.  Assume here M smooth, affine, hyperspherical.  Generic stabilizer... 
Then M obtained by Whittaker-twisted hamiltonian induction from symplectic representation S of H subset G, M = T*G x S quotiented by a diagonal action of H.  

Knop, Gaitsgory-Nadler, S, SV, SW - Given a spherical variety X acted on by G you can ...

BZSV: Collect all the data into a spectral period Mv = T*Gv which is a Hamiltonian Gv space.

Meta-conjecture: If M and Mv are dual hyperspherical varieties then M defines a BC P_M for the A_G side and L_Mv defines a BC for B_Gv and these match under S-duality.

Geometrically have Shv(LX/LGv) simeq QC(Mv).. 


Euler products: local -> global
Factorization homology: local -> global 
Trace of frobenius maps factorization homology to Euler products.  Can also put the Theta series operator into the TFT framework.  Not just coincidences but *science*.  