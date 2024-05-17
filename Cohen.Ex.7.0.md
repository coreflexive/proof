# Cohen - Exercise 7.0

An exercise in the construction of assignment statements framed as refinements.

## Part (a)

```
●	n,r : [r = n²]  ⊑  n,r ≔ n+1,E

1.	E = ? // E = n² + 2*n + 1

⊩		< Assignment >

	●	E = (n+1)²

	≡		< Expansion >

		E = n² + 2*n + 1	-- Assumption 1.

	▢

▢
```

## Part (b)

```
●	n,r : [r = n², r = n²]  ⊑  n,r ≔ n+1,E

1.	E = ? // E = r + 2*n + 1

⊩		< Assignment >

	●	(r = n²)  ⊆  (E = (n+1)²)

	≡		< Reduction >

		∀(r,n • r = n²  ⇒ E = (n+1)² )

	≡		< Establish ∀, fixing r, n >

		●	E = (n+1)²

		2.	r = n²

		≡		< Expansion >

			E = n² + 2*n + 1

		≡		< Assumption 2. >

			E = r + 2*n + 1		-- Assumption 1.

		▢

	⋯	∀(r,n • r = n²  ⇒ true )

	≡		< Right zero of ⇒ >

		∀(r,n • true )		-- Vacuous ∀

	▢

▢
```

## Part (c)

```
●	n,r : [r = n² ⋀ s = 2*n, r = n²]  ⊑  n,r ≔ n+1,E

1.	E = ? // E = r + s + 1

⊩		< Assignment >

	●	(r = n² ⋀ s = 2*n)  ⊆  (E = (n+1)²)

	⊩		< Reduction; Establish ∀, fixing r,n, and s >

		●	E = (n+1)²

		2.	r = n²

		3.	s = 2*n

		≡		< Expansion >

			E = n² + 2*n + 1

		≡		< Assumptions 2 and 3 >

			E = r + s + 1		-- Assumption 1.

		▢

	▢

▢
```
