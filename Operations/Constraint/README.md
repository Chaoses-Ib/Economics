# Constraint Satisfaction Problems
[Wikipedia](https://en.wikipedia.org/wiki/Constraint_satisfaction_problem)

**Constraint satisfaction problems (CSPs)** are mathematical questions defined as a set of objects whose state must satisfy a number of constraints or limitations.

A constraint satisfaction problem consists of three components, $Z$, $D$, and $C$:
- $X$ is a set of variables, $\{X_1,\cdots,X_n\}$.
- $D$ is a set of domains, $\{D_1,\cdots,D_n\}$, one for each variable.
- $C$ is a set of constaints that specify allowable combinations of values.

Each constraint $C_j$ consists of a pair $<scope,rel>$, where $scope$ is a tuple of variables that participate in the constraint and $rel$ is a relation that deﬁnes the values that those variables can take on. A relation can be represented as an explicit set of all tuples of values that satisfy the constraint, or as a function that can compute whether a tuple is a member of the relation. For example, if $X_1$ and $X_2$ both have the domain $\{1,2,3\}$, then the constraint saying that $X_1$ must be greater than $X_2$ can be written as $<(X_1,X_2),\{(3,1),(3,2),(2,1)\}>$ or as $<(X_1,X_2),X_1 > X_2>$.

Solving a CSP Partial assignment is an NP-complete problem in general, although there are important subclasses of CSPs that can be solved very efﬁciently.

CSP search algorithms take advantage of the structure of states and use general rather than domain-speciﬁc heuristics to enable the solution of complex problems. The main idea is to eliminate large portions of the search space all at once by identifying variable/value combinations that violate the constraints. CSPs have the additional advantage that the actions and transition model can be deduced from the problem description.[^ai-modern]


[^ai-modern]: Russell, Stuart J. Artificial Intelligence a Modern Approach. Pearson Education, Inc.,