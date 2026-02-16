---
title: Warwick-Imperial Maths Conference
subtitle: WIMP Spring 2026 itinerary
tags: [2026, events] # events, year, updates, talks

last_modified_at: 2026-02-15

show_author : true
author:
  name: Jakob Wood (Publications Officer)
  avatar: /assets/img/logo-large.PNG
 #location: "Location" (if applicable)

---

The **Warwick-Imperial Mathematics Conference** (WIMP) will take place on **Saturday 7th March**. The itinerary is as follows:

<img src="../assets/posts/2025-2026/WIMP Spring 2026 Itinerary.png" alt="WIMP Itinerary" width="95%"/>

Abstracts for the student talks can be found below.

The plenary talk is TBA.

<style>
blockquote {
    padding: 10px 20px 0 0;
    margin: 0 0 30px 0;
    font-size: 15px;
}
blockquote + blockquote {
    margin-top: -30px;
}
</style>

## Student talk abstracts

Jakob Kapelar (*Monsky’s Theorem: Dissecting Squares into an Odd Number of Triangles of Equal
Area*): 
>I would like to present a proof of Monsky’s Theorem, the surprising result that a
square cannot be dissected into an odd number of triangles of equal area. The talk would
follow the elegant approach in Proofs from THE BOOK. I would introduce p-adic valuations,
which are used to colour the unit square based on the 2-adic valuation of its coordinates.
Using an argument similar to Sperner’s Lemma we can find a triangle with a 2-adic norm of
the area > 1, contradicting the required area of 1/n for odd n. Preliminary knowledge: The
talk is largely combinatorial and self-contained.


Kshiraj Thummar (*Variational and Chaotic Dynamics in Strategic Systems: Lagrangian–Lyapunov Model
of Positional Complexity in Chess*):
> Traditional chess analysis relies on heuristic evaluation and tree search, offering
little insight into why positions destabilize or how complexity evolves. I develop a framework
treating chess as a continuous dynamical system on a 100-dimensional configuration
manifold, governed by variational principles from classical mechanics. I construct a
Lagrangian functional capturing the trade-off between kinetic energy (tactical volatility) and
potential energy (positional evaluation). And through Euler-Lagrange equations, we get a
second-order nonlinear system where positional acceleration follows the evaluation gradient.
The Hamiltonian formulation reveals conserved energy-like quantities, rapid tactical changes
must balance against positional quality. I have attempted to quantify chaos by Lyapunov
analysis through exponential divergence of nearby trajectories. I will prove that tactically
sharp positions, those with large positive Hessian curvature, exhibit exponential instability,
with divergence rates bounded by the square root of maximum eigenvalues. Poincaré
sections show how stable orbits disintegrate into chaos at critical thresholds. In critical
positions, such as Ding Liren’s blunder in the final game of the 2023 World Championship,
observing a sharp local increase in the dominant Lyapunov exponent, showing an
exponential divergence of the system’s trajectory and collapse of stability. Crucially, Hessian
analysis before the move predicted this catastrophe, genuine forecasting rather than the
post-hoc fitting we are accustomed to. I will establish major theorems on existence,
Lyapunov sensitivity, ergodicity, fractal dimension (observed ≈1.9), Pesin's entropy relation,
and variational-ergodic equivalence. Validation across 1000 grandmaster games yields ρ >
0.78 correlations between complexity metrics and error rates. Langevin dynamics with
temperature-dependent noise captures human imperfection, harder positions cause more
blunders across skill levels.What's more, the math extends beyond chess. Markets crash when Lyapunov exponents
surge. Evolution alternates between stasis and rapid change. Neural networks generalize
near intermediate curvature regions. Intelligent systems operate where order meets chaos,
where structure permits prediction but instability enables adaptation.
Even beyond chess, the model generalizes to any bounded-rational decision system
governed by nonlinear feedback and constrained optimization from adaptive learning
processes to market dynamics. My research also shows that strategic reasoning can be
viewed through the language of dynamical instability, looking at the analytic precision of
mathematics with the cognitive depth of decision-making. Not just a method for quantifying
complexity, but also a conceptual lens on how order and chaos coexist in human and
algorithmic intelligence.

 Jan Birmanns (*Proving the Hairy Ball Theorem*):
>The goal of the talk would be to follow the book "Topology from the Differentiable
Viewpoint" by Milnor to reach a proof of the hairy ball theorem. This would include a short
introduction of smooth functions, smooth manifolds, and tangent spaces, which would then
be followed by defining orientable manifolds, the degree of a function at a regular value, and
smooth homotopy. After discussing some examples and important properties of the degree,
such as the fact that it is preserved by smooth homotopy, I would present a sleek proof of
the hairy ball theorem as discussed on page 33 of the book. If there is enough time I would
also present a proof (strategy) for the properties of the degree. It is my goal to keep
prerequisites as low as possible, meaning that it should in theory be enough to simply know
what a derivative is. As I will be going somewhat quickly in the beginning though, familiarity
with multivariable calculus and manifolds should be very helpful.


Jonathan Glanfield (*Enumeration and Generation of Unlabelled Graphs*):
> Enumerating unlabelled graphs is a classic and notoriously difficult problem in
combinatorics. Unlike labelled graphs, where each vertex has a distinct identity, unlabelled
graphs consider graphs equivalent under relabelling of vertices, so counting them requires
considering graphs up to isomorphism, substantially increasing the complexity of the
problem. This talk presents two complementary approaches to this challenge. First, I explain how
group-theoretic tools can be used to enumerate unlabelled graphs by analysing the action of
the symmetric group on edge sets. I then describe a recursive algorithm for generating all
non-isomorphic graphs on a fixed number of vertices, using automorphism groups to limit
vertex extensions and canonical labelling to eliminate duplicates.
These approaches illustrate how group-theoretic insight and algorithmic techniques can be
used to attempt to tackle a classically hard enumeration problem.

Hongyu Wang (*Algebraic D-modules and their Formalisation*):

> Algebraic D-modules serve as the foundational language of modern Geometric
Representation Theory, providing an essential bridge between the representation theory of
semisimple Lie algebras and the geometry of flag varieties via the celebrated
Beilinson--Bernstein localisation theorem. While well- established in pen-and-paper
mathematics, their implementation in interactive theorem provers remains a frontier in
digitised mathematics.
In this talk, based on my undergraduate thesis supervised by Prof. Travis Schedler, I
introduce the formalisation of algebraic D-modules using the Lean 4 theorem prover Lean 4.
We begin with an introduction to formal verification, explaining how standard set-theoretic
objects map to Type Theory. We then focus on the affine case, constructing the $n$-th Weyl
algebra $A_{n}(\mathbb{C})$ in Mathlib. We discuss the challenges of formalising
non-commutative rings defined by generators and relations (specifically the canonical
commutation relation $[\partial_{i}, x_{j}] = \delta_{ij}$) and defining D-modules as typeclass
instances.Finally, we outline the roadmap from this affine foundation toward the global geometry
required for the Beilinson--Bernstein theorem, illustrating how proof assistants can verify
deep results in algebraic geometry. No prior knowledge of Lean or D-module theory is
assumed beyond basic ring and module theory.



 Sean Tan (*Optimal Transport*):
> Optimal transport is an important topic in both pure and applied mathematics.
Given two probability distributions and a cost function, we would like to "transport" one
distribution to the other in an optimal way that minimises cost. This has many applications in
applied maths, such as in economics, data science, biology, machine learning, etc, but more
surprisingly, has applications in pure mathematics too, such as in geometric analysis and the
analysis of some PDEs.In my talk I will introduce the optimal transport problem, motivate why it is such an important
area of mathematics (it really is), and derive the celebrated Sinkhorn's Algorithm, a
numerical scheme for solving the problem in the discrete case. I will also go through some of
my experimental results from stress-testing the algorithm on large data sets.

Chenyang Zhao (*Implicit Representations of Rational Curves and Surfaces via Syzygy Matrices*):
> This talk studies implicit representations of rational algebraic curves and surfaces
using matrices constructed from syzygies of their parametrizations. Starting from moving
lines and moving planes, we explain how to build Sylvester-type and hybrid matrices whose
rank and corank reflect geometric properties of the parametrized image. For plane and
space curves, these matrices are obtained from the syzygy module of the parametrization
and can be used to test membership and compute fiber multiplicities. We then extend the
construction to rational hypersurfaces and tensor-product surfaces by using graded kernels
and bidegree syzygies. In these cases, the resulting matrices give determinantal criteria for
points lying on the image and allow the recovery of fibers and intersections via generalized
eigenvalue problems. The methods are illustrated with examples and explicit computations
in Macaulay2, with applications to geometric modeling and elimination problems.


 Tim Gunaydin (*Diophantine Estimates on Tree Automorphism Groups and the Spectral Gap Property*):
> In this talk, we consider the group of automorphisms of an infinite d-regular tree.
This is a non-compact tdlc Hausdorff group. We will focus on a particular subgroup thereof,
the subgroup fixing a single vertex (we call this the stabilising subgroup since the choice of
vertex is often irrelevant). This group is a compact metrisable topological group with a
left-invariant metric and a Haar probability measure. More importantly, it is residually finite.
Using this rich structure of the group, combined with ideas from fractal geometry such as
Hausdorff and Minkowski dimension, we investigate Diophantine estimates on the stabilizing
subgroup. In particular, we show that a slightly weaker version of the Diophantine property
holds for the stabilising subgroup of the infinite d-regular tree automorphism group, for all
integers d greater than 2. Roughly speaking, this means that for almost every k-tuple chosen
from the group, random products of these approximate the identity rather poorly. This has
important implications in the context of the spectral gap property, which has further links to
the behaviour of random walks on the group. It is also an interesting result in its own right,
being a natural generalisation of Diophantine approximation on the real line.


Yu Coughlin (*Kleinian Singularities*)
> I'll define Kleinian singularities as quotients of C^2 by nice groups and talk about
their coordinate rings as the ring of invariants, with which we can very nicely classify the
singularities. I'll then discuss blowups and compute some blowups of Kleinian singularities at
the origin. From these we can associate a quiver which roughly looks like the curves in the
premiage of the singular point in the Kleinian singularity which I'll show some diagrams for,
finally we see that these are the ADE diagrams, and maybe briefly mention the idea of the
McKay correspondence which relates these graphs to representations of our initial group.

Alexander Cridland (*The geometry of Noether's Theorem*)
> In mathematical physics, notably classical mechanics, Noether’s theorem
provides a rich connection between two ubiquitous concepts in the field: symmetry and
conservation. Empirical laws such as conservation of momentum and energy are taken
precisely as their titles imply, as laws, but Noether provides the necessary background to
reframe such maxims as the consequence of a single encompassing theorem, stating that
every conservation law is directly equivalent to a physical symmetry. In this way we bridge
the gap between axiomatic and empirical approaches to physics and provide a unified
perspective on the matter, which is of great pedagogical value. We will explore how to
formulate and prove Noether’s theorem by studying the Hamiltonian formalism of classical
mechanics and the language of symplectic geometry, which naturally encodes the structure
of phase space dynamics. Finally, we will explore notable applications of the theorem and
discuss its implications in modern mathematical physics.
