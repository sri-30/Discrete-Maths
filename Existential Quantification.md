An existential [[Statement]] is of the form
>There exists an individual x in the universe of discourse for which the property P(x) holds

or, in other words,
>For some individual x in the universe of discourse, the property P(x) holds

or, in symbols,
>$\exists x. P(x)$

**Proof Strategy**:
To prove a goal of the form 

$\exists x. P(x)$

find a witness for the existential statement; that is, a value of $x$, say $w$, for which you think P(x) will be true, and show that indeed $P(w)$, ie the predicate $P(x)$ instantiated with the value $w$, holds.


**Proof Pattern**

In order to prove

$\exists x. P(x)$

1. Write Let $w =$... the witness you decided on
2. Provide a proof of $P(w)$

**The use of existential statements**
To use an assumption of the form $\exists x. P(x)$, introduce a new variable $x_0$ into the proof to stand for some individual for which the property $P(x)$ holds. This means that you can now assume $P(x_0)$ is true.

Examples:
[[The Pigeonhole Principle]]
[[Proposition 22]]
[[Theorem 24]]