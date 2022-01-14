A negation is a [[Statement]] of the form

> not $P$

or in other words

> $P$ leads to a contradiction

or in symbols

> $\neg P$

**Proof Strategy**
If possible, reexpress the negation in an equivalent form and use instead this other statement.

$\neg(P \implies Q) \iff P \land \neg Q$
$\neg(P \iff Q) \iff P \iff \neg Q$
$\neg (\forall x.P(x)) \iff \exists x. \neg P(x)$
$\neg (P \land Q) \iff (\neg P) \lor (\neg Q)$
$\neg (\exists x. P(x)) \iff \forall x. \neg P(x)$
$\neg (P \lor Q) \iff (\neg P) \land (\neg Q)$
$\neg(\neg P) \iff P$
$\neg P \iff (P \implies false)$

Examples:
[[Theorem 37]]