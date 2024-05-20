# Hoare Triple - Conjunctivity

```
●	{Q0} S {R0} ⋀ {Q1} S {R1}  ⇒  {Q0 ⋀ Q1} S {R0 ⋀ R1}

⊩		< Prove ⇒ >

	●	{Q0 ⋀ Q1} S {R0 ⋀ R1}

	1.	{Q0} S {R0}

	2.	{Q1} S {R1}

	≡		< Definition of Hoare Triple >

		Q0 ⋀ Q1 ⇒ wp.S.(R0 ⋀ R1)

	≡		< WP Conjunctivity >

		(Q0 ⋀ Q1 ⇒ wp.S.R0) ⋀ (Q0 ⋀ Q1 ⇒ wp.S.R1)

	⇐		< Antimonotonic antecedent, twice >

		(Q0 ⇒ wp.S.R0) ⋀ (Q1 ⇒ wp.S.R1)

	≡		< Definition of Hoare Triple, twice >

		{Q0} S {R0} ⋀ {Q1} S {R1}

	▢

▢
```
