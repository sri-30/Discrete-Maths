![[Pasted image 20220131193150.png]]
![[Pasted image 20220131195533.png]]
1. Every block in part(E) is non-empty
	- Because $a \in [a]_E$
2. $\bigcup part(E) = A$
	- $\subseteq$ is clear
	- $\supseteq$ Every element of $A$ appears in a block.
		- Necessarily the caseas $\forall a \in A. \exists \beta \in part(E) \text{ namely } \beta = [a]_E \text{ such that } a \in \beta$
3. If $\beta_1, \beta_2 \in part(E)$ such that $\beta_1 \cap \beta_2 \neq \emptyset$ then $\beta_1 = \beta_2$
	Let $\beta_1, \beta_2 \in part(E)\text{ such that } \beta_1 \cap \beta_2 \neq \emptyset$
	Then $\beta_1=[a_1]_E$ for some $a_1 \in A$
	$\beta_2=[a_2]_E$ for some $a_2 \in A$
	Also $b \in [a_1]_E$ and $b \in [a_2]_E$ for some $b$
	$b E a_1 \land b E a_2$
	$a_1 E b E a_2$
	Lemma: $a_1 E a_2 \iff [a_1]_E = [a_2]_E$
	
