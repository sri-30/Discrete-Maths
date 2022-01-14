[[Big Unions and Intersections]]
[[Set]]
[[Powerset axiom]]

Let $\mathcal{F} = \set{S \subseteq \mathbb{R}|(0 \in S) \land (\forall x \in \mathbb{R}. x \in S \implies (x+1)\in S)}$
Then
1. $\mathbb{N} \in \mathcal{F}$
2. $\mathbb{N} \subseteq \bigcap \mathcal{F}$

Hence, $\bigcap \mathcal{F} = \mathbb{N}$

Proof:
RTP: $\bigcap \mathcal{F} = \mathbb{N}$ 
$\iff (\bigcap \mathcal{F} \subseteq \mathbb{N} \land \mathbb{N} \subseteq \bigcap \mathcal{F})$
1. RTP: $\bigcap \mathcal{F} \subseteq \mathbb{N}$
We show $\mathbb{N} \in \mathcal{F}$, which is the case by definition of [[Natural]] numbers.

2. RTP: $\mathbb{N} \subseteq \bigcap \mathcal{F}$
$\iff \forall n \in \mathbb{N}. n \in \bigcap \mathcal{F} \iff \forall n \in \mathbb{N}. \forall S \in \mathcal{F}. n \in S$

We proceed by induction on $n$

We show $\forall n \in \mathbb{N}. P(n)$
where $P(n) = \forall S \in \mathcal{F}. n \in S.$

Base case: $n = 0$

$\forall S \in \mathcal{F}. 0 \in S$ by definition of the family.

Inductive step: Let $n \in \mathbb{N}$
Inductive Hypothesis: $\forall S \in \mathcal{F}. n \in S$
RTP: $\forall S \in \mathcal{F}. (n+1) \in S$

Let $S \in \mathcal{F} \implies \forall x \in \mathbb{R}. x \in S \implies (x+1) \in S$

By the induction hypothesis, $n \in S$, so $(n+1) \in S$

QED.