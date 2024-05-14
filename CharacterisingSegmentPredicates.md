# Characterising Predicates over Segments

Here we present the definitions of three characterisations of predicates over segments:

1. Holds for empty range
2. Is prefix-closed
3. Is postfix closed

We'll then see a couple of (very detailed) proofs.

## The Definitions

In each of following definitions, we assume the following about `A`:

```
A ∈ (p: ℕ) → (q: ℕ) → 𝔹
```

Strictly speaking, `A` should have another parameter `N: ℕ`, but let's just treat it as implicit, for now.

### Holds for Empty Range

```
●	A "holds for empty range"

⊩		< Definition of "holds for empty range" >

	●	∀(n : 0 ≤ n ≤ N : A.n.n)
```

### Prefix-Closed

```
●	A "is prefix-closed"

⊩		< Definition of "is prefix-closed" >

	●	∀(p,q ∈ ℕ : 0 ≤ p ≤ q ≤ N : A.p.q  ⇒  ∀(i : p ≤ i ≤ q : A.p.i ))
```

### Postfix-Closed

```
●	A is "postfix-closed"

⊩		< Definition of is "postfix-closed" >

	●	∀(p,q ∈ ℕ : 0 ≤ p ≤ q ≤ N : A.p.q  ⇒  ∀(i : p ≤ i ≤ q : A.i.q ))
```

## The Example Proofs

### Establishing Empty Range

```
●	A "holds for empty range"

1.	A = (p,q ∈ ℕ : 0 ≤ p ≤ q ≤ N : ∀(i : p ≤ i < q : X.i = 0))

2.	X ∈ [0..N) → ℕ

≡		< Definition of "holds for empty range" >

	∀(n ∈ ℕ : 0 ≤ n ≤ N : A.n.n)

≡		< Assumption 1. >

	∀(n ∈ ℕ : 0 ≤ n ≤ N : (p,q ∈ ℕ : 0 ≤ p ≤ q ≤ N : ∀(i : p ≤ i < q : X.i = 0)).n.n)

≡		< β-reduction >

	∀(n ∈ ℕ : 0 ≤ n ≤ N : 0 ≤ n ≤ n ≤ N ⋀ ∀(i : n ≤ i < n : X.i = 0))

≡		< Inequalities >

	∀(n ∈ ℕ : 0 ≤ n ≤ N : 0 ≤ n ≤ N ⋀ ∀(i : false : X.i = 0))

≡		< Substitution >

	∀(n ∈ ℕ : 0 ≤ n ≤ N : ∀(i : false : X.i = 0))

≡		< ∀ empty-range >

	∀(n ∈ ℕ : 0 ≤ n ≤ N : true)

≡		< Trivial >

	true

▢
```

### Establishing Prefix-Closed

```
●	A "is prefix-closed"

1.	A = (p,q ∈ ℕ : 0 ≤ p ≤ q ≤ N : ∀(i : p ≤ i < q : X.p ≤ X.i))

2.	X ∈ [0..n) → Int

≡		< Definition of "is prefix-closed">

	∀(p,q ∈ ℕ : 0 ≤ p ≤ q ≤ N : A.p.q  ⇒  ∀(i ∈ ℕ : p ≤ i ≤ q : A.p.i))

≡		< Establish ∀ >

	●	∀(i ∈ ℕ : p ≤ i ≤ q : A.p.i)

	3.	0 ≤ p ≤ q ≤ N

	4.	∀(i : p ≤ i < q : X.p ≤ X.i)

	≡		< Assumption 1.; β-reduction >

		∀(i ∈ ℕ : p ≤ i ≤ q : 0 ≤ p ≤ i ≤ N ⋀ ∀(j : p ≤ j < i : X.p ≤ X.j))

	≡		< ∀ Distributive >

		∀(i ∈ ℕ : p ≤ i ≤ q : 0 ≤ p ≤ i ≤ N) ⋀
		∀(i ∈ ℕ : p ≤ i ≤ q : ∀(j : p ≤ j < i : X.p ≤ X.j))

	≡		< Establish ⋀ >

		●	∀(i ∈ ℕ : p ≤ i ≤ q : 0 ≤ p ≤ i ≤ N)

		≡		< Assumption 3. i.e. q ≤ N >

			∀(i ∈ ℕ : 0 ≤ p ≤ i ≤ q ≤ N : 0 ≤ p ≤ i ≤ N)

		⇐		< Antimonotonic ∀ range, using ≤ transitive >

			∀(i ∈ ℕ : 0 ≤ p ≤ i ≤ N : 0 ≤ p ≤ i ≤ N)

		≡		< Reflexivity >

			true

		▢

		●	∀(i ∈ ℕ : p ≤ i ≤ q : ∀(j : p ≤ j < i : X.p ≤ X.j))

		≡		< Substitution: i ≤ q ≡ true >

			∀(i ∈ ℕ : p ≤ i ≤ q : ∀(j : p ≤ j < i ≤ q : X.p ≤ X.j))

		⇐		< Antimonotonic ∀ range, using ≤ transitive >

			∀(i ∈ ℕ : p ≤ i ≤ q : ∀(j : p ≤ j < q : X.p ≤ X.j))

		≡		< Assumption 4. >

			∀(i ∈ ℕ : p ≤ i ≤ q : true)

		≡		< Trivial >

			true

		▢

	⋯	true

	▢

⋯	true

▢
```

🍊
