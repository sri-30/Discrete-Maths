[[Powerset axiom]]

Let $U$ be a [[Set]] and let $A, B \in \mathcal{P}(U).$

1. $\forall X \in \mathcal{P}(U). A \cup B \subseteq X \iff (A \subseteq X \land B \subseteq X)$
2.  $\forall X \in \mathcal{P}(U). X \subseteq A \cup B \iff (X \subseteq A \land X \subseteq B)$

Proof:

Let $A,B,X \in \mathcal{P}(U)$

RTP: $A \cup B \subseteq X \iff (A \subseteq X \land B \subseteq X)$

1. Assume $A \cup B \subseteq X$
RTP: $A \subseteq X \land B \subseteq X$
Equivalently we are proving $\forall a \in A. a \in X \land \forall b \in B. b \in X$
	
	Assume $a \in A$
	$a \in A \land A \cup B \subseteq X \implies a \in X$
	
	Assume $b \in B$
	$b \in B \land A \cup B \subseteq X \implies b \in X$

2. Assume $A \subseteq X \land B \subseteq X$
RTP: $A \cup B \subseteq X$
Let $x \in A \cup B$
Equivalently $x \in A \lor x \in B$
	
	Case $x \in A$:
	By the assumption, $x \in A \land A \subseteq X \implies x \in X$
	
	Case $x \in B$:
	By the assumption, $x \in B \land B \subseteq X \implies x \in X$

QED.