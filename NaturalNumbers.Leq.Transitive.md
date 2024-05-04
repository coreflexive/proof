The ≤ relation on the natural numbers is transitive.

```
●	Transitive ℕ ≤

≡		Definition of Transitive

	∀(x,y,z ∈ ℕ • x ≤ y ⋀ y ≤ z ⇒ x ≤ z)

≡		Establish ∀

	●	x ≤ z

	1.	x,y,z ∈ ℕ

	2.	x ≤ y

	3.	y ≤ z

	a.	∃(k ∈ ℕ • x + k = y)	{ by definition of ≤ on 1. }

	b.	∃(k ∈ ℕ • y + k = z)	{ by definition of ≤ on 2. }

	+	Define m ∈ ℕ:

		x + m = y

	+	Define n ∈ ℕ:

		y + n = z
	
	c.	∃(k ∈ ℕ • x + k z)

		{ Non-linear proof }

		●	x + k = z

		4.	k = ? // k = m + n 

		≡		Definition of n

			x + k = y + n

		≡		Definition of m

			x + k = x + m + n

		⇐		Leibniz

			k = m + n

		=		Assumption 4.

			true

		▢

	⊩	Goal follolws from observation c. and the definition of ≤

	▢

⋯	true

▢
```

👹
