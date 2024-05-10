Theorem (Raising the Lower Side): `[(x ⊑ z  ⇐  y ⊑ z)  ⇐  x ⊑ y] ≡ Transitive ⊑`

Proof:

```
●	[(x ⊑ z  ⇐  y ⊑ z)  ⇐  x ⊑ y]

≡		Definition of ⇐

	[x ⊑ y  ⇒  (x ⊑ z  ⇐  y ⊑ z)]

≡		Definition of ⇐

	[x ⊑ y  ⇒  y ⊑ z  ⇒  x ⊑ z]

≡		Shunting

	[x ⊑ y  ⋀  y ⊑ z  ⇒  x ⊑ z]

≡		Definition of Transitive

	Transitive ⊑

▢
```

🚡
