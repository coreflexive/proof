# Postcondition Rule

Proof that we can strengthen a postcondition.

```
●	{Q} S {A} ⋀ (A ⇒ R) ⇒ {Q} S {R}

⊩		< Prove ⇒ >

	●	{Q} S {A}

	1.	A ⇒ R

	≡		< Definition of Hoare Triple >

		Q ⇒ wp.S.A

	⇒		< WP Monotonic, using assumption 1. >

		Q ⇒ wp.S.R

	≡		< Definition of Hoare Triple >

		{Q} S {R}

	▢

▢
```
