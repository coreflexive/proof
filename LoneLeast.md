The least element of a poset are unique if they exist.

●	$\textbf{Lone} \, (\textbf{Least} \; A \; R \; B)$

$\equiv$		Definition of $\textbf{Lone}$

​	$\forall(z,y \in B : (\textbf{Least} \; A \; R \; B).z \wedge (\textbf{Least} \; A \; R \; B).y : z = y)$

$\Leftarrow$		Antimonotonic $\forall$ range

​	●	$(\textbf{Least} \; A \; R \; B).z \wedge (\textbf{Least} \; A \; R \; B).y$

​	$\equiv$		Definition of $\textbf{Least}$, twice

​		$\forall(x \in B :: z \mathbin{R} x) \wedge \forall(x \in B :: y \mathbin{R} x)$

​	$\Rightarrow$		$\forall$ instantiation, twice

​		$z \mathbin{R} y \wedge y \mathbin{R} z$

​	$\equiv$		$R$ antisymmetric

​		$z = y$​

​	$\square$

$\cdots$	$\forall(z,y \in B : z = y : z = y)$

$\square$
