A least element of a poset is unique if it exists.

```
●	Lone (Least A ⊑ B)

≡		Definition of Lone

	∀(z,y ∈ B • (Least A ⊑ B).z ⋀ (Least A ⊑ B).y ⇒ z = y)

⇐		Antimonotonic ∀ range

	●	(Least A ⊑ B).z ⋀ (Least A ⊑ B).y

	≡		Definition of Least, twice

		∀(x ∈ B • z ⊑ x) ⋀ ∀(x ∈ B • y ⊑ x)

	⇒		Instantiation, twice

		z ⊑ y ⋀ y ⊑ z
	
	≡		⊑ Antisymmetric

		z = y

	▢

⋯	∀(z,y ∈ B • z = y ⇒ z = y)

▢
```

💛
