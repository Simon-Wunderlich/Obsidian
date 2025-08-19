Created: Aug 19 2025
Class: [[Maths]]
- - -
# For all 
## $\forall xP(x)$ 
###### Universal quantifier: 
P(x) is true for all values of x in the domain

# There exists
## $\exists xP(x)$
###### Existential quantifier:
There exists a value of x for which P(x) is true
P(x) is true for at least 1 value of x

# De Morgan's law
### $$
 \neg \forall x P(x) \equiv \exists x \neg P(x)
 $$
If not all values of x are true, there must exist a value for which P(x) is false
### $$
\neg \exists  x P(x) \equiv \forall x \neg P(x)
 $$
 If no x exists for which P(x) is true, P(x) false for all values of x

# Nested quantifiers
Read left to right
$$
\exists x \exists y \forall z(x*y=z)
$$
###### FALSE
$$
\forall z \exists x \exists y (x*y=z)
$$
###### TRUE
### Switching quantifiers
For equations $\exists x \forall y \forall z P(x):$
$$
\exists x \forall y \forall z P(x) \not\equiv \forall y \exists x \forall z P(x) 
$$
$$
\exists x \forall y \forall z P(x) \not\equiv \exists x \forall z \forall y P(x) 
$$
ie. can swap alike quanitifiers