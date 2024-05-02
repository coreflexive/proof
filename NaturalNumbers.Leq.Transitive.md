The $\leq$ relation on the natural numbers is transitive.

●	$\textbf{Transitive} \; \N \; \leq$

≡		Definition of transitive

​	$\forall(x,y,z \in \N : x \leq y \wedge y \leq z : x \leq z)$

≡		Establish $\forall$

​	●	$x \leq z$

​	i.	$x,y,z \in \N$

​	ii.	$x \leq y$

​	iii.	$y \leq z$

​	a.	$\exists(k \in \N :: x + k = y)$	{ by definition of $\leq$ on i. }

​	b.	$\exists(k \in \N :: y + k = z)$	{ by definition of $\leq$ on ii. }

​	›	Define $m \in \N$:

​		$x + m = y$

​	›	Define $n \in \N$:

​		$y + n = z$

​	c.	$\exists(k :: x + k = z)$

​		●	$x + k = z$

​		iv.	$k = ?$ // $k = m + n$

​		≡		Definition of $n$

​			$x + k = y + n$

​		≡		Definition of $m$

​			$x + k = x + m + n$

​		≡		Leibniz

​			$k = m + n$

​		≡	Assumption iv.

​			$\text{true}$

​		$\square$

​	$\Vdash$	Goal follows from observation c and the definition of $\leq$

​	$\square$

⋯	$\text{true}$

$\square$

