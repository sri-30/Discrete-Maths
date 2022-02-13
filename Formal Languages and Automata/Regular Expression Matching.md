 ![[Pasted image 20220213013933.png]]

We can introduce operator precedence and associativity conventions for concrete syntax and cut down the pairs in the ~ relation to make it single-valued (that is, $r \sim R \land r \sim R' \implies R = R'$).
For example, for [[regular expression]]s we decree:
> _* binds more tightly than __, binds more tightly than _|_

So, for example the only parse of $\epsilon|ab^{*}$ is the tree
$$Union(Null,Concat(Sym_a,Star(Sym_b)))$$
We also decree that the binary operations of concatenation and union are left associative, so that for example $abc$ parses as
$$Concat(Concat(Sym_a,Sym_b),Sym_c)$$
(However, the union and concatenation operators for regular expressions will always be given a semantics that is [[associative]], so the left-associativity convention is less important than the operator-precedence convention)