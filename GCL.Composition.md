# GCL - Composition

```
●	{Q} S {H} ⋀ {H} T {R}  ⇒  {Q} S;T {R}

⊩	{Q} S;T {R}

1.	{Q} S {H}

2.	{H} T {R}

a.	Q ⇒ wp.S.H	< Hoare Triple on assumption 1. >

b.	H ⇒ wp.T.R	< Hoare Triple on assumption 2. >

≡		< Definition of Hoare Triple >

	Q ⇒ wp.(S;T).R

≡		< Definition of ; >

	Q ⇒ (wp.S.(wp.T.R))

⇐		< Observation b. >

	Q ⇒ (wp.S.H)

⇐		< Observation a. >

	Q ⇒ Q

▢
```
