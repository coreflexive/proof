Theorem (Lowering the Upper Side): `[(x ⊑ z  ⇐  x ⊑ y)  ⇐  y ⊑ z] ≡ Transitive ⊑`

Proof:

```
●	[(x ⊑ z  ⇐  x ⊑ y)  ⇐  y ⊑ z]

≡		Definiton of ⇐

	[y ⊑ z  ⇒  (x ⊑ z  ⇐  x ⊑ y)]

≡		Definition of ⇐

	[y ⊑ z  ⇒  x ⊑ y  ⇒  x ⊑ z]

≡		Shunting

	[y ⊑ z  ⋀  x ⊑ y  ⇒  x ⊑ z]

≡		⋀ Symmetric

	[x ⊑ y  ⋀  y ⊑ z  ⇒  x ⊑ z]

≡		Definition of Transitive

	Transitive ⊑

▢
```

🚡
