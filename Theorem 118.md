[[Preorders]]

For $R \subseteq A \times A$, let

$$\mathcal{F}_R = \set{Q \subseteq A \times A | R \subseteq Q \land Q \text{is a preorder}}$$
Then (i) $R^{\circ *} \in \mathcal{F}_R$ and (ii) $R^{\circ *} \subseteq \bigcap \mathcal{F}_R$. Hence $R^{\circ *} = \bigcap \mathcal{F}_R$

Proof:

> $R \circ *$ is the least preorder that contains $R$

$R^{\circ *} \in \mathcal{F}_R \implies \bigcap \mathcal{F}_R \subseteq R^{\circ *}$

# i
RTP: $R^{\circ *} \in \mathcal{F}_R \iff R \subseteq R^{\circ *}$ and $R^{\circ *}$ is a preorder

[[Unfinished]]

# ii
RTP: $R^{\circ *} \subseteq \bigcap \mathcal{F}_R \iff \bigcap_{n \in \mathbb{N}} R^{\circ(n)} \subseteq \bigcap \mathcal{F}_R$
$\iff \forall n \in \mathbb{N}. R^{\circ (n)} \subseteq \bigcap \mathcal{F}_R$
$\iff \forall n \in \mathbb{N}. \forall Q \in \mathcal{F}_R. R^{\circ (n)} \subseteq Q$

Proof by induction on $n \in \mathbb{N}$

Base case ($n = 0$)

$id \subseteq Q$ because $Q$ is [[reflexive]]

Inductive step:

IH: $\forall Q \in \mathcal{F}_R. R^{\circ(n)} \subseteq Q$
RTP: $\forall Q \in \mathcal{F}_R. R^{\circ (n+1)} \subseteq Q.$

Let $Q \in \mathcal{F}_R$

$R^{\circ (n+1)} = R^{\circ (n)} \circ R \subseteq Q \circ Q \subseteq Q$ by [[Transitivity]]