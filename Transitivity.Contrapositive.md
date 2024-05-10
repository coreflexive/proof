Theorem: `[x ⊐ z  ⇒  x ⊐ y  ⋁  x ⊐ z] ≡ Transitive ⊑`

Proof:

```
●	Transitive ⊑

≡		Definition of Transitive

	[x ⊑ y  ⋀  y ⊑ z  ⇒  x ⊑ z]

≡		Contrapositive

	[¬(x ⊑ z) ⇒ ¬(x ⊑ y  ⋀  y ⊑ z)]

≡		DeMorgan

	[¬(x ⊑ z) ⇒ ¬(x ⊑ y)  ⋁  ¬(y ⊑ z)]

≡		Not ⊑ is ⊐, thrice

	[x ⊐ z ⇒ x ⊐ y  ⋁  y ⊐ z]

▢
```

🚡
