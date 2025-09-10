Created: Sep 10 2025
Class: [[Maths]] 
#unsure 
- - -
Used to show [[Satisfiability|unsatisfiability]] of a propositional formula and hence prove [[Entailment]]

Prove $KB \vDash \varphi$, where KB (knowledge base) is a set of formulas known to be true, and $\varphi$ is the formula we want to prove is satisfiable

$$
KB \rightarrow \varphi \space is \space always \space true
$$
$$or$$
$$KB \land \neg \varphi \space is \space always \space false$$
# Main steps
$\vdots$
# Resolution methods
## Inference
For KB
$A \rightarrow B$
$B \rightarrow C$

And $\varphi$
$A \rightarrow C$

Proof:
$A \rightarrow B \rightarrow C$
## CNF
Propositional atoms: P, Q, R
Literals, P $\neg P$, Q $\neg Q$, R $\neg R$ 
Disjunctive clauses: $\neg P \lor \neg Q \lor \neg R$
CNF: $(\neg P \lor Q) \land (Q \lor \neg R) \land R$

Find negation of $KB \vDash \varphi$ 
Find CNF of negation
Look for contradiction in CNF
If negation has contradiction, $KB \vDash \varphi$  is always true
https://echo360.org.au/media/2a6b3e3a-1a20-41e7-9557-b8a5eed9d679/public?currentMediaId=65ac1b24-5930-4491-a505-68779016e2c5

## 'The Method'???
https://echo360.org.au/media/d558d73f-3d12-4595-b400-55392dcb53ca/public?currentMediaId=c96f8cf4-c85d-49b2-8b9a-b3902753c8c0&sessionId=b9d76191-70a9-4d35-a283-da38d59f794e
