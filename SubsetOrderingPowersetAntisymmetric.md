The subset ordering of a powerset is antisymmetric.

●	$\textbf{Antisymmetric} \; \mathcal{P}.A \; \subseteq_A$

≡		Definition of antisymmetric

​	$\forall(X,Y \in \mathcal{P} :: X \subseteq_A Y \wedge Y \subseteq X \Rightarrow X = Y)$

≡		Prove $\forall$

​	●	$X \subseteq_A Y \wedge Y \subseteq X$

​	✓	$X, Y \in \mathcal{P}.A$

​	≡		Definition of subset, twice

​		$\forall(a :: a \in X \Rightarrow a \in Y) \wedge \forall(a :: a \in Y \Rightarrow a \in X)$

​	≡		Distributivity

​		$\forall(a :: (a \in X \Rightarrow a \in Y) \wedge (a \in Y \Rightarrow a \in X))$

​	≡		Mutual implication

​		$\forall(a :: a \in X \equiv a \in Y)$

​	≡		Set equality

​		$X = Y$

​	$\square$

⋯	$\forall(X,Y \in \mathcal{P} :: X = Y \Rightarrow X = Y)$

≡		⇒ Reflexive

​	$\text{true}$

$\square$

