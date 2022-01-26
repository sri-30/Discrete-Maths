A relation $R : A \rightarrow B$    is said to be functional and called a partial function, whenever it is such that

$$\forall a \in A, \forall b_1, b_2 \in B. a R b_1 \land a R b_2 \implies b_1 = b_2$$
Every element in the source is related to at most one in the target.

![[Pasted image 20220126194430.png]]

Def: $R: A \rightarrow B$

R is functional at $a \in A$ whenever $a$ is related to at most one element of $B$.

$$\forall b_1, b_2 \in B. a R b_1 \land a R b_2 \implies b_1 = b_2$$
NB: $S \subseteq R: A \rightarrow B$
If $R$ is functional at $a$, then so is $S$.

$f : A \rightharpoonup B$: $f$ is a partial function from $A$ to $B$

Given $a \in A$, we have either

1. There is no $b \in B$ such athat $a f b$
or
2. There is a unique $b \in B$ such that $afb$

In case
1. $f(a) \uparrow$ $f$ is undefined at $a$
2. $f(a) \downarrow$ $f$ is defined at $a$

Moreover, $f(a)$ denotes the unique element of $B$ such that $(a, f(a))$ is in $f$.

### Domain of definition
For $f: A \rightharpoonup B$,

dom($f$) $\subseteq A = \set{a \in A | f(a) \downarrow} = \set{a \in A | \exists b \in B. afb}$

Example:

pred: $\mathbb{N} \rightharpoonup \mathbb{N} = \set{(n+1, n) \in \mathbb{N} \times \mathbb{N}|n \in \mathbb{N}} = \set{(x, y) \in \mathbb{N} \times \mathbb{N} | x \geq 1 \land x = y + 1}$ 
$pred(0) \uparrow$
$pred(m) \downarrow$ for $m$ a positive integer
$pred(m) = m - 1$

dom(pred) is the set of positive integers

### Defining Partial Functions
![[Pasted image 20220126200037.png]]

Example: $pred: \mathbb{N} \rightharpoonup \mathbb{N}$

$pred: n \in \mathbb{N} \mapsto max k < n. k \in \mathbb{N}$
as a relation:
pred = $\set{(n,m) \in \mathbb{N} \times \mathbb{N} | m = max k < n. k \in \mathbb{N}}$
For all $n \in \mathbb{N}$ there is at most one element equal to $max_{k \in \mathbb{N}}$. For $n = 0$ there is no such element, for $n \geq 1$ that element is $n-1$.

as