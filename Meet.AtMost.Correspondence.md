This one is **Lemma 2.1** from Back's book on the refinement calculus.

**Theorem (Correspondence).** The following properties hold for any `a`, `b` in a poset:

1. `a ⊓ b = a  ≡  a ⊑ b`
2. `a ⊔ b = b  ≡  a ⊑ b`

whenever the meet and join in question exist.

He gives a proof, but I'm going to expand on some of the detail.

**Proof.** By mutual implication.

```
●	a ⊓ b = a  ⇒  a ⊑ b
⊩		Prove ⇒
	●	a ⇒ b
	1.	a ⊓ b = a
	≡		Textual substitution using 1
		a ⊓ b ⇒ b
	⇐		Meet elimination
		true
	▢
```

```
●	a ⊑ b  ⇒  a ⊓ b = a
⊩		Prove ⇒
	●	a ⊓ b = a
	1.	a ⊑ b
	⇐		⊑ Antisymmetric
		a ⊓ b ⊑ a ⋀ a ⊑ a ⊓ b
	⇐		⊓ Elimination
		a ⊑ a ⊓ b
	⇐		⊓ Introduction
		a ⊑ a ⋀ a ⊑ b
	⇐		⊑ Reflexive
		a ⊑ b
	⇐		Assumption 1.
		true
	▢
```

The proof of part 2. is the same, *mutatis mutandis*.

❤️