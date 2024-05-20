# GCL - Abort versus false

```
●	{Q} abort {R}  ≡  Q ≡ false

⊩	{Q} abort {R}

≡		< Definition of Hoare Triple >

	Q ⇒ wp.abort.R

≡		< Definition of abort >

	Q ⇒ false

≡		< bottom >

	Q ⇒ false ⋀ false ⇒ Q

≡		< Mutual implication >

	Q ≡ false

▢
```
