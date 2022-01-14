For all statements $P$ and $Q$,

$(P \implies Q) \implies (\neg Q \implies \neg P)$

Proof:

Let $P$ and $Q$ be statements,

Assume (1) $P \implies Q$

RTP: $\neg Q \implies \neg P$

Proof strategy: [[Proof by Contradiction]]

1. Assume (2) $\neg Q$
	1. RTP: $\neg P$
		1. Assume (3) $P$
			1. RTP: false

From (1) and (3) we have (4) $Q$. From (2) and (4) we have false.
QED.