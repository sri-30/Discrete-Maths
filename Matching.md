Each [[regular expression]] $r$ over an alphabet $\Sigma$ determines a language $L(r) \subseteq \Sigma^{*}$. The [[string]]s $u$ in $L(r)$ are by definition the ones that match $r$, where
- $u$ matches the regular expression $a$ (where $a \in \Sigma \iff u = a$)
- $u$ matches the regular expression $\epsilon$ iff $u$ is the null string $\epsilon$
- no string matches the regular expression $\emptyset$
- $u$ matches $r|s$ iff it either matches $r$, or it matches $s$
- $u$ matches $rs$ iff it can be expressed as the concatenation of two strings, $u=vw$, with $v$ matching $r$ and $w$ matching $s$
- $u$ matches $r^{*}$ iff either $u=\epsilon$, oe $u$ matches $r$, or $u$ can be expressed as the concatenation of two or more strings, each of which matches $r$.

# [[Inductive definition]] of matching
![[Pasted image 20220213020018.png]]
![[Pasted image 20220213020209.png]]
![[Pasted image 20220213021049.png]]
