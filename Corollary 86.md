[[Powerset axiom]]

Let $U$ be a [[set]] and let $A, B, C \in \mathcal{P}(U)$

1. $C = A \cup B$ 
$\iff$
$[A \subseteq C \land B \subseteq C]$ 
$\land$ 
$[\forall X \in \mathcal{P}(U). (A \subseteq X \land B \subseteq X) \implies C \subseteq X]$

2. $C = A \cap B$ 
$\iff$
$[C \subseteq A \land C \subseteq B]$ 
$\land$ 
$[\forall X \in \mathcal{P}(U). (X \subseteq A \land X \subseteq B) \implies X \subseteq C]$