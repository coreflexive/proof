Theorem (Join Monotonic): `[a ⊑ a'  ⋀  b ⊑ b'  ⇒  a ⊔ b ⊑ a' ⊔ b']`

Proof:

```
●	[a ⊑ a'  ⋀  b ⊑ b'  ⇒  a ⊔ b ⊑ a' ⊔ b']

⊩		Prove ⇒

	●	a ⊔ b ⊑ a' ⊔ b'

	1.	a ⊑ a'

	2.	b ⊑ b'

	≡		Universal property of ⊔
	
		a ⊑ a' ⊔ b'  ⋀  a ⊔ b ⊑ b'

	⇐		⊑ Transitive, twice, using ⊔ introduction

		a ⊑ a'  ⋀  b ⊑ b'

	▢

▢
```

☢️

