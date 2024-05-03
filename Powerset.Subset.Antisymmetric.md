**Theorem:** The subset ordering of a powerset is antisymmetric.

**Proof:**
```
●	Antisymmetric 𝒫.A ⊆

≡		Definition of Antisymmetry

	∀(X,Y ∈ 𝒫.A • X ⊆ Y ⋀ Y ⊆ X  ⇒  X = Y)

≡		Prove ∀

	●	X ⊆ Y ⋀ Y ⊆ X

	i.	X,Y ∈ 𝒫.A

	≡		Definition of ⊆ twice

		∀(a • a ∈ X ⇒ a ∈ Y) ⋀ ∀(a • a ∈ Y ⇒ a ∈ X)

	≡		∀ distributivity

		∀(a • (a ∈ X ⇒ a ∈ Y) ⋀ (a ∈ Y ⇒ a ∈ X))

	≡		Mutual implication

		∀(a • a ∈ X ≡ a ∈ Y)

	≡		Extensionality

		X = Y

	▢

⋯	∀(X,Y ∈ 𝒫.A • X = Y  ⇒  X = Y)

≡		⇒ reflexive

	true
▢
```

🦃
