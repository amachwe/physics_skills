# Monads and Adjunctions

## Adjunctions
Two functors $F: \mathcal{C} \to \mathcal{D}$ and $G: \mathcal{D} \to \mathcal{C}$ are adjoint (denoted $F \dashv G$) if there is a natural isomorphism:
$$\text{Hom}_{\mathcal{D}}(F(A), B) \cong \text{Hom}_{\mathcal{C}}(A, G(B))$$

## Monads
A monad is a triple $(T, \mu, \eta)$ where $T$ is an endofunctor ($T: \mathcal{C} \to \mathcal{C}$), $\mu$ is a natural transformation $\mu: T^2 \to T$, and $\eta$ is a natural transformation $\eta: Id \to T$.
- Monads are fundamental in functional programming (e.g., State, Maybe, List monads).
