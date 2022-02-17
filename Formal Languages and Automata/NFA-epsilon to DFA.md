[[Finite Automata]]
![[Pasted image 20220216192913.png]]

NFA- $M- (Q (\text{set of states}), \Sigma (\text{Set of input values}), \Delta \subseteq Q \times \Sigma \times Q(\text{Relations between states}), s \in Q \text{Starting state}, F \subseteq Q (\text{Accepting States}), T \subseteq Q \times Q(\text{Epsilon transitions}))$
For DFA: $\delta: Q \times \Sigma \rightarrow Q$, and no $T$

For PM $Q' = \mathcal{P}(Q)$

In state $q_0$ there is a state transition $q_0 \xRightarrow{\epsilon b} q_2$

$\delta(S, a) = \set{q' \in Q | \exists q \in S. (q, a, q') \in \Delta}$

$s' = \set{q_0, q_1, q_2} = \set{q' \in Q| (s, q') \in T}$

The accepting states are states that contain at least one accepting state.

$F' = \set{s \in Q'| S \cap F \neq \emptyset}$

> **Theorem**: For each $NFA^{\epsilon}$ $M=(Q, \Sigma, \Delta, s, F, T)$ there is a DFA $PM = (\mathcal{P}(Q), \Sigma, \delta, s', F')$ accepting exactly the same strings as $M$, i.e. with $L(PM) = L(M)$.

Definition of $PM$:
- set of states is the powerset $\mathcal{P}(Q) = \set{S|S \subseteq Q}$ of the set $Q$ of states of $M$
- same input alphabet $\Sigma$ as for $M$
- next-state function maps each $(S,a) \in \mathcal{P}(Q) \times \Sigma$ to $\delta(S,a) \triangleq \set{q' \in Q | \exists q \in S. q \xRightarrow{a} q' \text{ in } M}$
- start state is $s' \triangleq \set{q' \in Q | s \xRightarrow{\epsilon} q'}$
- subset of accepting states is $F' \triangleq \set{S \in \mathcal{P}(Q) | S \cap F \neq \emptyset}$

## Proving that $P$ is equivalent to $PM$
RTP:
$L(M) \subseteq L(PM)$
$L(PM) \subseteq L(M)$
![[Pasted image 20220217230507.png]]
![[Pasted image 20220217232401.png]]
