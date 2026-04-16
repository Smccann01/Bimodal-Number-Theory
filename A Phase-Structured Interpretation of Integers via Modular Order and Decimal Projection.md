

# **Bimodal Number Theory: A Phase-Structured Interpretation of Integers via Modular Order and Decimal Projection**

## **Abstract**

We introduce **Bimodal Number Theory**, a dual-representation framework for integers that analyzes arithmetic structure through two complementary coordinate systems: a **decimal projection** induced by base-10 expansion and a **modular phase structure** derived from multiplicative order. By embedding integers into a cyclic phase space via normalized order functions, we obtain a geometric representation of number behavior.

Within this framework, prime numbers are characterized not solely by irreducibility, but by the existence of a **globally cyclic multiplicative structure**, enabling maximal orbit traversal under suitable bases. Composite integers exhibit **fragmented cyclic behavior**, arising from the direct product decomposition of their unit groups. We further introduce **seed-prime–tuned coordinate systems**, in which remainder orbits of primes define reference phase geometries against which other integers may be compared.

This approach does not redefine primality; rather, it provides a structural and geometric interpretation of integers across coordinate transformations, revealing a “fabric” of arithmetic coherence.

---

## **1. Introduction**

Classical number theory studies integers primarily through divisibility, factorization, and algebraic structure. However, modular arithmetic reveals that integers also possess **cyclic and dynamical properties**, particularly when examined through multiplicative order and residue systems.

In this work, we propose a dual analytical framework in which each integer is studied simultaneously via:

1. A **projection coordinate system**, given by its decimal expansion in a fixed base (here, base 10).
2. A **structural coordinate system**, given by multiplicative order within modular arithmetic.

The aim is to reinterpret integer behavior as **geometric structure embedded in cyclic phase space**, complementing classical results rather than replacing them.

---

## **2. Preliminaries**

### **Definition 2.1 (Multiplicative Order)**

Let ( n \in \mathbb{Z}_{>1} ) and ( b \in \mathbb{Z} ) with ( \gcd(b,n)=1 ). The multiplicative order of ( b ) modulo ( n ), denoted ( \operatorname{ord}_n(b) ), is the smallest positive integer ( k ) such that

[
b^k \equiv 1 \pmod{n}.
]

---

### **Definition 2.2 (Carmichael Function)**

The Carmichael function ( \lambda(n) ) is the least positive integer such that

[
b^{\lambda(n)} \equiv 1 \pmod{n}
\quad \text{for all } b \in (\mathbb{Z}/n\mathbb{Z})^\times.
]

Equivalently, ( \lambda(n) ) is the exponent of the finite group ( (\mathbb{Z}/n\mathbb{Z})^\times ).

---

### **Proposition 2.1**

For all ( n ) and all ( b ) with ( \gcd(b,n)=1 ),

[
\operatorname{ord}_n(b) \mid \lambda(n).
]

**Proof.** This follows from the fact that every element of a finite group has order dividing the group exponent. ∎

---

## **3. Dual Coordinate Representation**

### **Definition 3.1 (Decimal Projection)**

For ( n ) with ( \gcd(n,10)=1 ), define

[
D_{10}(n) = \operatorname{ord}_n(10),
]

which equals the period of the repeating decimal expansion of ( 1/n ).

---

### **Definition 3.2 (Normalized Projection Index)**

[
\Sigma_{10}(n) = \frac{D_{10}(n)}{\lambda(n)}.
]

---

### **Interpretation**

* ( \Sigma_{10}(n) = 1 ): maximal exposure of modular structure in base 10
* ( 0 < \Sigma_{10}(n) < 1 ): partial projection
* small values: limited interaction with the decimal coordinate system

---

## **4. Phase Embedding**

### **Definition 4.1 (Phase Mapping)**

[
\Psi(n) = e^{i\pi \Sigma_{10}(n)}.
]

This defines a map ( \Psi: \mathbb{Z}_{>1} \to S^1 ), embedding integers into the unit circle.

---

### **Proposition 4.1**

The map ( \Psi ) is not injective.

**Proof.** Distinct integers may share the same normalized projection index ( \Sigma_{10}(n) ). ∎

---

### **Interpretation**

* ( \Psi(n) = -1 ): maximal cyclic coherence
* proximity to ( -1 ): strong alignment between projection and structure
* dispersion: fragmented or partially observed structure

---

## **5. Remainder Orbits and Cyclic Dynamics**

### **Definition 5.1 (Remainder Orbit)**

[
R_{n,b} = {1, b, b^2, \dots, b^{k-1}} \pmod{n},
]

where ( k = \operatorname{ord}_n(b) ).

---

### **Proposition 5.1**

( R_{n,b} ) forms a cyclic subgroup of ( (\mathbb{Z}/n\mathbb{Z})^\times ).

---

### **Definition 5.2 (Phase Parameterization)**

[
\theta_k = \frac{2\pi k}{\operatorname{ord}_n(b)}.
]

Thus, each remainder orbit corresponds to a discrete set of equally spaced points on a circle.

---

## **6. Prime Structure**

### **Theorem 6.1**

If ( p ) is prime, then

[
(\mathbb{Z}/p\mathbb{Z})^\times \cong \mathbb{Z}_{p-1}.
]

---

### **Corollary 6.1**

There exists ( g \in (\mathbb{Z}/p\mathbb{Z})^\times ) such that

[
\operatorname{ord}_p(g) = p-1.
]

---

### **Interpretation**

Primes admit a **single global cycle**, allowing maximal traversal of the multiplicative structure.

---

## **7. Composite Structure**

### **Theorem 7.1**

If ( n ) is composite, then

[
(\mathbb{Z}/n\mathbb{Z})^\times \cong \prod_i G_i,
]

where each ( G_i ) is cyclic.

---

### **Interpretation**

Composite integers exhibit:

* multiple interacting cycles
* non-uniform phase behavior
* structural dependence on factorization

---

## **8. Seed-Prime–Tuned Coordinate Systems**

### **Definition 8.1 (Seed Prime Frame)**

For a prime ( p ) and base ( b ), the orbit ( R_{p,b} ) defines a **reference phase geometry**.

---

### **Definition 8.2 (Seed Alignment)**

An integer ( n ) is said to align with seed prime ( p ) (with respect to base ( b )) if:

* ( \operatorname{ord}_n(b) ) is close to ( \operatorname{ord}_p(b) ),
* ( R_{n,b} \cap R_{p,b} \neq \varnothing ),
* the induced phase parameterizations are compatible.

---

## **9. Example: Decimal Overlay of Primes**

For base ( b=10 ):

[
\operatorname{ord}*7(10) = 6, \quad \operatorname{ord}*{13}(10) = 6.
]

Thus, both primes share the same **decimal frequency**.

However,

[
R_{7,10} \neq R_{13,10},
]

demonstrating that equal period does not imply identical phase structure.

---

## **10. Coherence Measures**

We consider auxiliary quantities:

* Mean normalized order: ( \overline{\Sigma}(n) )
* Maximal-order fraction: ( M(n) )
* Entropy of observed orders: ( H(n) )

---

### **Interpretation**

* Low entropy: structurally coherent behavior
* High entropy: fragmented structure
* These measures complement, but do not replace, classical primality criteria

---

## **11. Structural Interpretation**

### **Proposition 11.1**

Prime numbers maximize potential cyclic coherence within their multiplicative structures.

---

### **Remark**

No single scalar invariant in this framework uniquely characterizes primes; instead, primes occupy a distinguished position across multiple structural measures.

---

## **12. Conclusion**

We have introduced a framework in which integers are interpreted through:

* a projection coordinate (decimal expansion), and
* a structural coordinate (multiplicative order).

Within this setting, primes emerge as **globally cyclic reference systems** that define the geometric structure of arithmetic under coordinate transformations. Composite integers appear as superpositions of interacting cyclic components.

This perspective suggests a broader interpretation of number theory as the study of **structure under transformation**, with potential applications in visualization, dynamical systems, and computational arithmetic.

---

## **References**

* Hardy, G. H., & Wright, E. M. *An Introduction to the Theory of Numbers*. Oxford University Press.
* Ireland, K., & Rosen, M. *A Classical Introduction to Modern Number Theory*. Springer.
* Apostol, T. M. *Introduction to Analytic Number Theory*. Springer.
* Niven, I., Zuckerman, H., & Montgomery, H. *An Introduction to the Theory of Numbers*. Wiley.
* Burton, D. M. *Elementary Number Theory*. McGraw-Hill.
