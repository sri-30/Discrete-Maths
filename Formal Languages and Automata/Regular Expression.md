Concrete syntax: [[string]]s of symbols
![[Pasted image 20220213003927.png]]
Abstract syntax: finite rooted trees
![[Pasted image 20220213003953.png]]

Regular expressions over a given [[alphabet]] $\Sigma$
Let $\Sigma '$ be the 6-element set $\set{\epsilon, \emptyset, |, *, (,)}$ (assumed disjoint from $\Sigma$)

> $U = (\Sigma \cup \Sigma ')$
> axioms: $\frac{}{a}$ $\frac{}{\epsilon}$ $\frac{}{\emptyset}$
> rules: $\frac{r}{(r)}$ $\frac{r\text{   }s}{r|s}$ $\frac{r\text{   }s}{rs}$ $\frac{r}{r^{*}}$
> (where $a \in \Sigma$ and $r, s \in U$)

![[Pasted image 20220213004953.png]]

The 'signature' for regular expression abstract syntax trees (over an alphabet $\Sigma$) consists of
- binary operators Union and Concat
- unary operator Star
- nullary operators (constants) Null, Empty and $\text{Sym}_a$ (one for each $a \in \Sigma$)
![[Pasted image 20220213005431.png]]
![[Pasted image 20220213005456.png]]
### Relating concrete and abstract syntax
![[Pasted image 20220213005524.png]]
