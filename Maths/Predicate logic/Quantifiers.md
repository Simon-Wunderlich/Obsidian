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

- - -
# De Morgan's law
### $$\neg \forall x P(x) \equiv \exists x \neg P(x)$$
If not all values of x are true, there must exist a value for which P(x) is false
### $$\neg \exists  x P(x) \equiv \forall x \neg P(x) $$
 If no x exists for which P(x) is true, P(x) false for all values of x

- - -
# Nested quantifiers
Read left to right
$$
\exists x \forall y(x+y=0)
$$
###### FALSE
$$
\forall x \exists y(x+y=0)
$$
###### TRUE
- - -
### Switching quantifiers
$$\exists x \forall y P(x) \not\equiv \forall y \exists x P(x) $$
$$
\forall x \forall y P(x) \equiv \forall y \forall x P(x) 
$$
ie. can swap alike quantifiers
### De Morgans law
![[Pasted image 20250819184336.png]]

### Moving quantifiers
#### Null qualification rule
For expression $A$ which does not contain $y$,
$$
A \space \wedge \space \forall y \space F(y,*) \equiv \forall y \space (A \wedge F(y,*))
$$

