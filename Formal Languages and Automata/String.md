A string of length $n$ (for $n=0,1,2,...$) over an [[alphabet]] $\Sigma$ is just an ordered $n$-tuple of elements of $\Sigma$, written without any punctuation.

$\Sigma^{*}$ denotes the set of all strings over $\Sigma$ of any finite length.

Examples:

- If $\Sigma = {a,b,c}$, then $\epsilon, a, ab, aac,$ and $bbac$ are strings over $\Sigma$ of lengths zero, one, two, three and four respectively.
- If $\Sigma = \set{a}$, then $\Sigma^{*}$ conains $\epsilon, a, aa, aaa, aaaa$ etc.
- If $\Sigma = \emptyset$ , then $\Sigma^{*} = \set{\epsilon}$

There is a unique strong of length zero over $\Sigma$, called the null string (or empty string) and denoted $\epsilon$, no matter which alphabet $\Sigma$ we are talking about.

We make no notational distinction between a symbol $a \in \Sigma$ and the string of length $1$ containing $a$. Thus we regard $\Sigma$ as a subset of $\Sigma^{*}$.

$\emptyset, \set{\epsilon}$ and $\epsilon$ are three different things:
- $\emptyset$ is the (unique) set with no elements
- $\set{\epsilon}$ is a set with one element (the null string)
- $\epsilon$ is the string of length $0$

The length of a string $u \in \Sigma^{*}$ is denoted $|u|$
