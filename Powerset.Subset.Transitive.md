The subset ordering of a power set is transitive.

```
●	Transitive 𝒫.A ⊆

≡		Definition of transitive

	∀(X,Y,Z ∈ 𝒫.A • X ⊆ Y ⋀ Y ⊆ Z ⇒ X ⊆ Z)

≡		Establish ∀

	●	X ⊆ Y ⋀ Y ⊆ Z

	1.	X,Y,Z ∈ 𝒫.A

	≡		Definition of subset, twice

		∀(a ● a ∈ X ⇒ a ∈ Y) ⋀ ∀(a ● a ∈ Y ⇒ a ∈ Z)
	
	≡		∀ distributive

		∀(a ● a ∈ X ⇒ a ∈ Y ⋀ a ∈ Y ⇒ a ∈ Z)

	≡		⇒ transitive

		∀(a ● a ∈ X ⇒ a ∈ Z)

	≡		Definition of subset

		X ⊆ Z

	▢

⋯	∀(X,Y,Z ∈ 𝒫.A • true)

≡		Trivial

	true

▢
```

🍄
