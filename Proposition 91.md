[[Set]]
[[Powerset axiom]]
[[Big Unions and Intersections]]
[[Associative]]

For all $\mathcal{F} \in \mathcal{P}(\mathcal{P}(\mathcal{P}(U)))$,

$\bigcup(\bigcup \mathcal{F}) = \bigcup \set{\bigcup \mathcal{A} \in \mathcal{P}(U) | \mathcal{A} \in \mathcal{F}} \in \mathcal{P}(U)$

Proof:

RTP: $\forall x. x \in \bigcup(\bigcup(\mathcal{F})) \iff x \in \bigcup(\set{\bigcup \mathcal{A} \in \mathcal{P}(U)|\mathcal{A} \in \mathcal{F}})$

$x \in \bigcup(\bigcup(\mathcal{F})) \iff \exists S \in \bigcup(\mathcal{F}). x \in S$

$\iff \exists S. S \in \bigcup(\mathcal{F}) \land x \in S$

$\iff \exists S. \exists \mathcal{A} \in \mathcal{F}. S \in \mathcal{A} \land x \in S$

$x \in \bigcup(\set{\bigcup \mathcal{A} \in \mathcal{P}(U)|\mathcal{A} \in \mathcal{F}})$ 
$\iff \exists \mathcal{A} \in \mathcal{F}. x \in \bigcup(\mathcal{A})$
$\iff \exists \mathcal{A} \in \mathcal{F}. \exists S \in \mathcal{A}. x \in S$

QED.

![[Pasted image 20211217120259.png]]