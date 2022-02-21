>**Theorem**: If $L_1$ and $L_2$ are regular languages over an alphabet $\Sigma$, then their intersection $L_1 \cap L_2 = \set{u \in \Sigma* | u \in L_1 \land u \in L_2}$ is also regular.

**Proof**: Note that $L_1 \cap L_2 = \Sigma* \backslash ((\Sigma* \backslash L_1) \cup (\Sigma* \backslash L_2))$ due to de Morgan's Law

So if $L_1$