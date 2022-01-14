For all positive integers $p$ and natural numbers $m$, if $m=0$ or $m=p$ then ${p \choose m} \cong 1 \mod {p}$

Proof:
Let $p$ be an arbitrary positive integer and $m$ an arbitrary natural number.

Assume $m = 0 \lor m = p$

${p \choose m} = \frac {p!}{m!(p-m)!}$

RTP $p|(\frac {p!}{m!(p-m)!} - 1)$

Proof strategy: [[Disjunction]]

1. Case 1: $m = 0$
${p \choose 0} = 1 \cong 1 \mod {p}$
QED.

2. Case 2: $m = p$
${p \choose p}  = 1 \cong 1 \mod {p}$
QED.

QED by (1) and (2).