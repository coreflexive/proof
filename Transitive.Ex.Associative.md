An associative binary operator gives rise to a transitive relation.

```
●	Transitive ⊑

1.	x ⊑ y  ≡  x ⊓ y = x

2.	Associative ⊓

≡		Definition of Transitive

	∀(x,y,z ∈ A • x ⊑ y ⋀ y ⊑ z ⇒ x ⊑ z)

≡		Establish ∀

	●	x ⊑ z

	3.	x ⊑ y

	4.	y ⊑ z

	a.	x ⊓ y = x

	b.	y ⊓ z = y

	c.	x ⊓ z = x

		●	x ⊓ z

		=		Observation a.

			(x ⊓ y) ⊓ z

		=		Assumption 2.

			x ⊓ (y ⊓ z)

		=		Observation b.

			x ⊓ y

		=		Observation a.

			x

		▢

	⊩		Goal follows from observation c. by the defintion of ⊑

	▢

⋯	true

▢
```