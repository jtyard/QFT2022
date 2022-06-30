# 
Plan for the talk:
- Begin by recalling the usual geometric Satake equivalence so that we can discuss why it is a bad statement.  
- Will replace it with something good (known)
- Generalize part 3 (Lie superalgebras) 
- Discuss relation to David's talk

## 
G=reductive algebraic group connected/C, Gv = Langlands dual

$K = K((t)) \supset O = C[[t]]$

Gr_G = G(K)/G(O)

Geometric Satake Theorem: $Perv_{G(O)}(Gr_G) = D-mod_{G(O)}(Gr_G) = Rep Gv$
- Doesn't hold as stated
- Doesn't extend to quantum level: Rep Gv has a natural deformation Rep_q Gv = representations of the corresponding quantum group

A form on g = Lie G is fixed, integral and even.  It defines a determinant line bundle L on Gr_G.  Try to study $Perv_{G(O)}(L^\circ)_q$.  Want an equivalence with Rep_q(Gv) but you really don't have it (LHS is vector space for generic q).

Remark: if q a root of 1, then LHS is equiv to Rep(H) where rk(H) = rk(G).

Tudor: RHS is a symmetric tensor category so it won't appear on the bulk in 4d but it can on the boundary.

## 

Better statement: FLE = Fundamental Local Equivalence [Lurie], [Gaitsgory], [Gaitsgory-Lysenko]

Whit(Gr_G) = (N(K),chi)-equivariant D-module
N subset G = maximal unipotent, chi = generic character

Then Whit(Gr_G) = Rep Gv is true on the derived level.  Also true for q though at roots of unity requires certain quantum group.

But here he keeps q generic.  Will discuss series of generalizations with exmpels of dual boundary conditions with generic KW-twisted 4d YM - mostly due to Gaiotto.

G = finite supergroup.  G_0 reductive.  g = g0 + g1 has an invariant nondegenerate symmetric bilinear form.  g1 becomes symplectic representation of G0.  Can talk about Rep_q(G).  

Goal: To present a series of generalizations of the FLE statement.
On the RHS:
Rep G = G0-equivariant modules over $\Wedge g_1$

On the LHS: Roughly speaking, some kind of category of sheaves on Gr_G0.

What are the supergroups in question?  GL(m|n), SoSp(2k|2n), F(4), Spin(7)xSL(2), SoSp(2k+1,2n), G(3), G_2 x SL(2).

Rough idea: G0 acting on symplectic M = g1.  Dual Mv with action of G0v.
$Perv_{G(O)}(X(k)) = Rep(G)$ and q-version.  Variant: Mv is some kind of twisted cotangent bundle i.e. 
Yv acted on by H and Xv = TYv // (H,chi)
Then 
$$Perv_{(H(K),\chi)\rtimes G^\vee(O)}(Y^\vee(K))$$

m leq n.  g1 = T*(Mat nxm) acts on G0 = GL(n) x GL(m)

Mv = ?
If m = n then Mv = T*(GL(n) x C^n) subset GL(n)xGL(n)

If m < n then $Mv = GL(n) \times S_{m,n}$ where Smn is the Slodowy slice to mxm Jordan block in Cmn.   

If m = n-1 then Mv = T*(GL(n)) subset GL(n)xGL(n-1)

LHS: m=n 

$$Perv_{GL(n,O)}(Gr_GL(n)xK^n) = Perv_{GL(n,K)}(Gr_{GL(n)xGL(n)}xK^n) = Rep(GL(n|n))$$

Some things with q.  m = n-1 get 
$$Perv_{GL(n-1,O)}(Gr_GL(n)) = Perv_{GL(n,K)}(Gr_{GL(n)xGL(n)}) = Rep(GL(n|n))$$
...

q=1: Braverman-Finkelberg-Ginzburg-Travkin m=n,n-1
Travkin-Hang any $m < n$
q generic $m=n-1$ Braverman-Finkelberg-Travkin

m=0 then Umn is maximal unipotent and we get the FLE for GL(n)

The derived category is the derived category of an abelian (t-heart?)

m=n not understood at roots of unity - don't even know what the right statement is

Lemma: In the above cases, g1 is lways a hyperspherical symplectic representation of G0.  

Gives a condition for M to define a boundary condition though more generally it defines a BC in some twisted version of 4d YM.  