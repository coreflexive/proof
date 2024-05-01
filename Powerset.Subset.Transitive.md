The subset ordering of a power set is transitive.

●	$\textbf{Transitive} \; \mathcal{P}.A \; \subseteq_A$

≡		Definition of transitive

​	$\forall(X,Y,Z \in \mathcal{P}.A : X \subseteq_A Y \wedge Y \subseteq_A Z : X \subseteq_A Z)$

≡		Prove $\forall$

​	●	$X \subseteq_A Y \wedge Y \subseteq_A Z$​

​	✓	$X,Y,Z \in \mathcal{P}.A$

​	≡		Definition of subset, twice

​		$\forall(a :: a \in X \Rightarrow a \in Y) \wedge \forall(a :: a \in Y \Rightarrow a \in Z)$

​	≡		Distributivity

​		$\forall(a :: (a \in X \Rightarrow a \in Y) \wedge (a \in Y \Rightarrow a \in Z))$

​	≡		⇒ Transitive

​		$\forall(a :: a \in X  \Rightarrow a \in Z)$

​	≡		Definition of subset

​		$X \subseteq_A Z$

​	$\square$

⋯	$\forall(X,Y,Z \in \mathcal{P}.A : X \subseteq_A Z : X \subseteq_A Z)$

≡		Reflexivity

​	$\text{true}$

$\square$

