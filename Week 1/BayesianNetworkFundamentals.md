# Bayesian Network Fundamentals
#### January 17
#### Lecturer: Daphne Koller
#### Scribe: Jonathan Baum

## Semantics and Factorization

Begin with a collection of random variables.

Developing and relationships between the variables creates a Bayesian network.

Model is a representation of how we believe the world works.

Each node (random variable) is annotated with a CPD (conditional probability
distribution). In which each node is parametrized by its relationships with the
other variables.

The chain rain rule takes all the CPDs and multiplies them together (and is
a factor product). Formally given $\forall X_i, P(X_1, X_2, \ldots X_n) = 
\prod P(X_i\mid E_{in}(X_i))$

Given a specific set of state(s) of the variable(s) 

**Bayesian Networks** are directed acyclic graphs (DAGs) $G$ whose nodes 
represent the random variables $X_1, \ldots X_n$. Where each node is $X_i$ there 
is a CPD $P(X_i \mid \text{Par}_G(X_i))$. 

The BN represents a joint distribution over the chain rule for BN.

We can show $P \gt 0$ by that P is a product of CPDs. CPDs are non-negative.

We can show that $\sum P = 1$ via the following proof.

**See 13:00 min for extended proof.**

$P$ factorizes over $G$ that is it can be represented by $G$ if the chain rule
applies.

## Reasoning Patterns

**Causal reasoning** uses the unidirectional edges of the Bayesian graph $G$, 
such that the conditioning occurs in the direction of the edges.

**Evidential Reasoning** uses the unidirectional edges of the Bayesian graph 
$G$, such that the conditioning occurs in the opposite direction of the edges.

**Intercausal Reasoning** uses a combination of causal and evidential reasoning 
to condition and obtain its conclusions. 

Intercausal reasoning can make a significant difference in the behavior of the 
resultant probabilities after conditioning.



