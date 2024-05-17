# Cohen - Exercise 7.1

An exercise in the construction of assignment statements framed as refinements.

## Part (a)

```
●	n,s : [s = Σ(i : 0 ≤ i ⋀ i < n : f.i)]  ⊑  n,s ≔ 0,E

1.	E = ? // E = 0

⊩		< Assignment >

	●	(true)  ⊆  (E = Σ(i : 0 ≤ i ⋀ i < 0 : f.i))

	⊩		< Reduction; Establish ∀, fixing n and s >

		●	E = Σ(i : 0 ≤ i ⋀ i < 0 : f.i)

		≡		< Inequalities >

			E = Σ(i : false : f.i)

		≡		< Σ Empty-range >

			E = 0		-- Assumption 1.

		▢
	▢

▢
```

## Part (b)

```
●	n,s : [s = Σ(i : 0 ≤ i ⋀ i < n : f.i)]  ⊑  n,s ≔ 1,E

1.	E = ? // E = f.0

⊩		< Assignment >

	●	(true)  ⊆  (E = Σ(i : 0 ≤ i ⋀ i < 1 : f.i))

	⊩		< Reduction; Establish ∀, fixing n and s >

		●	E = Σ(i : 0 ≤ i ⋀ i < 1 : f.i)

		≡		< Inequalities >

			E = Σ(i : 0 = i : f.i)

		≡		< Σ One-point >

			E = f.0		-- Assumption 1

		▢
	
	▢

▢
```
