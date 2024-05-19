# Postcondition Rule

Proof that we can strengthen a postcondition.

```
●	{Q} S {A} ⋀ (A ⇒ R) ⇒ {Q} S {R}

≡		< ⋀ symmetric >

	(A ⇒ R) ⋀ {Q} S {A}  ⇒ {Q} S {R}

≡		< Shunting >

	(A ⇒ R) ⇒ ({Q} S {A}  ⇒ {Q} S {R})

≡		< WP Monotonic >

	true

▢
```
