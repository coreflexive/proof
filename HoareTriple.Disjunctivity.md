# Hoare Triple - Disjunctivity

```
●	{Q0} S {R0} ⋀ {Q1} S {R1}  ⇒  {Q0 ⋁ Q1} S {R0 ⋁ R1}

⊩		< Prove ⇒ >

	●	{Q0 ⋁ Q1} S {R0 ⋁ R1}

	1.	{Q0} S {R0}

	2.	{Q1} S {R1}

	≡		< Definition of Hoare Triple >

		(Q0 ⋁ Q1) ⇒ wp.S.(R0 ⋁ R1)

	≡		< ⋁ universal property >

		(Q0 ⇒ wp.S.(R0 ⋁ R1)) ⋀ (Q1 ⇒ wp.S.(R0 ⋁ R1))

	≡		< Definition of Hoare Triple, twice >

		{Q0} S {R0 ⋁ R1} ⋀ {Q1} S {R0 ⋁ R1}

	⇐		< Postcondition Rule, using ⇒ weakening, twice >

		{Q0} S {R0} ⋀ {Q1} S {R1}

	▢

▢
```
