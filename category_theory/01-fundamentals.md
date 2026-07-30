# Category Theory Foundations

## What is a Category?
A category $\mathcal{C}$ consists of:
- A collection of **objects** $A, B, C \dots$
- For every pair of objects $(A, B)$, a set of **morphisms** $f: A \to B$.
- An **identity morphism** $1_A: A \to A$ for every object $A$.
- A **composition law**: if $f: A \to B$ and $g: B \to C$, then there exists $g \circ f: A \to C$.

## Functors
A functor $F: \mathcal{C} \to \mathcal{D}$ is a mapping between categories that preserves structure:
- Objects $A \in \mathcal{C} \implies F(A) \in \mathcal{D}$.
- Morphisms $f: A \to B \implies F(f): F(A) \to F(B)$.
- Preservation of identity and composition.

## Natural Transformations
A natural transformation $\alpha$ is a way of transforming one functor $F$ into another functor $G$. It is a family of morphisms $\alpha_A: F(A) \to G(A)$ such that for every $f: A \to B$, the following diagram commutes:
$$G(f) \circ \alpha_A = \alpha_B \circ F(f)$$
