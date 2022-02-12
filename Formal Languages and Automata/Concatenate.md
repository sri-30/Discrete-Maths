The concatenation of two [[string]]s $u$ and $v$ is the string $uv$ obtained by joining the strings end-toend. This generalises to the concatenation of three or more strings.

Examples:

If $\Sigma = \set{a,b,c,...,z}$ and $u,v,w \in \Sigma^{*}$ are $u=ab$, $v=ra$ and $w=cad$, then

$$vu=raab$$
$$uu=abab$$
$$wv=cadra$$
$$uvwuv=abracadabra$$
Concatenation satisifies:

$$u\epsilon=u=\epsilon u$$
$$(uv)w=uvw=u(vw)$$
$$|uv| = |u| + |v|$$
If $u \in \Sigma^{*}$, then $u^n$ denotes $n$ copies of $u$ concatenated together. By convention $u^0 = \epsilon$