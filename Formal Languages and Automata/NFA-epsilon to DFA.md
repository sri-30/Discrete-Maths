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