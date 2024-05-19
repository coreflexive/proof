# Hoare Triple - Precondition Rule

```
●	(Q ⇒ A) ⋀ {A} S {R} ⇒ {Q} S {R}

⊩		< Prove ⇒ >

	●	(Q ⇒ A) ⋀ {A} S {R}

	≡		< Definition of Hoare Triple >

		(Q ⇒ A) ⋀ (A ⇒ wp.S.R)

	⇒		< ⇒ Transitive >

		Q ⇒ wp.S.R

	≡		< Definition of Hoare Triple >

		{Q} S {R}

	▢

▢
```
