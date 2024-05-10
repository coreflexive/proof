Theorem (Meet Monotonic): `[a ⊑ a'  ⋀  b ⊑ b'  ⇒  a ⊓ b ⊑ a' ⊓ b']`

Proof:

```
●	[a ⊑ a'  ⋀  b ⊑ b'  ⇒  a ⊓ b ⊑ a' ⊓ b']

⊩		Prove ⇒

	●	a ⊓ b ⊑ a' ⊓ b

	1.	a ⊑ a'

	2.	b ⊑ b'

	≡		Universal Property of ⊓

		a ⊓ b ⊑ a'  ⋀  a ⊓ b ⊑ b'

	⇐		Raising the Lower Side, twice, using ⊓ elimination

		a ⊑ a'  ⋀  b ⊑ b'

	≡		Assumptions 1 and 2; ⋀ Idempotent

		true

	▢

▢
```

☢️
