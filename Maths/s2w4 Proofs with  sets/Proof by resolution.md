Created: Sep 10 2025
Class: [[Maths]] 
- - -
Used to show [[Satisfiability|unsatisfiability]] of a propositional formula and hence prove [[Entailment]]

Prove $KB \vDash \varphi$, where KB (knowledge base) is a set of formulas known to be true, and $\varphi$ is the formula we want to prove is satisfiable

$$
KB \rightarrow \varphi \space is \space always \space true
$$
$$or$$
$$KB \land \neg \varphi \space is \space always \space false$$
# Method
Rewrite $KB \vDash \varphi$ as $KB \space ' = KB \land \neg \varphi$
Rewrite $KB\space '$ in CNF
Prove $KB \space '$ is not satisfiable
## Inference
$$KB \vDash \varphi$$
$$iff$$
$$all \space models \space of \space KB \space are \space models \space of \space \varphi$$
$$iff$$
$$KB \rightarrow \varphi \space is \space a \space valid$$
$$iff$$
$$KB \land \neg \varphi \space is \space unsatisfiable$$
$\therefore$ If you can prove $KB \land \neg \varphi$ is a contradiction, you prove that $KB \vDash \varphi$

## CNF
Find $KB \land \neg \varphi$
Find CNF of $KB \land \neg \varphi$
Look for contradiction in CNF
If negation has contradiction, $KB \vDash \varphi$  is always true

## Main resolution step
Consider $(P \lor Q)$ and $(\neg P \lor R)$
- If $P$ is true, $(P \lor Q)$ is true and $(\neg P \lor R)$ is just R
- If $P$ is false, $(P \lor Q)$ is Q and $(\neg P \lor R)$ is true
Therefore, $(P \lor Q) \land (\neg P \lor R)$ can be resolved to $(Q \lor R)$

If two clauses of a CNF contain a literal and its negation, the literal can be cancelled out and the remains of each clause can be unioned with each other to form a new clause