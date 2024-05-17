# Binary Minimum

This document presents a construction of a program that selects the minimum of two numbers.

```
●	m ≔ a ↓ b

=		< Simple specification >

	m : [m = a ↓ b]

=		< Default precondition >

	m : [true, m = a ↓ b]

=		< ↓ calculus >

	m : [a ↓ b = a  ⋁  a ↓ b = b, m = a ↓ b]

⊑		< Alternation >

	if a ↓ b = a → m ≔ a
	▯ a ↓ b = b → m ≔ b
	fi

=		< ↓ calculus >

	if a ≤ b → m ≔ a
	▯ a ≤ b = b → m ≔ b
	fi

▢
```

Summarising:

```
m ≔ a ↓ b 
⊑	if a ≤ b → m ≔ a
	▯ a ≤ b = b → m ≔ b
	fi  
```

❤️