>**Theorem**: If $L_1$ and $L_2$ are regular languages over an alphabet $\Sigma$, then their intersection $L_1 \cap L_2 = \set{u \in \Sigma* | u \in L_1 \land u \in L_2}$ is also regular.

**Proof**: Note that $L_1 \cap L_2 = \Sigma* \backslash ((\Sigma* \backslash L_1) \cup (\Sigma* \backslash L_2))$ due to de Morgan's Law

So if $L_1 = L(M_1)$ and $L_2 = L(M_2)$ for DFAs $M_1$ and $M_2$, then $L_1 \cap L_2 = L(Not(PM))$ where $M$ is the NFA$^{\varepsilon}$ $Union(Not(M_1),Not(M_2))$.
![[Pasted image 20220221031700.png]]
