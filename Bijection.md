[[Function]]s which are invertible or reversible.

$f: A \rightarrow B$ is bijective iff 
$\exists g: B \rightarrow A. g \circ f = id_A$
$\land$
$\exists h: B \rightarrow A. f \circ h = id_B$
**NB**: If $f$ is bijective and $g \circ f = id_A$ and $f \circ h = id_B$ then $h=g$

$g \circ f \circ h$: $g \circ f$ is the identity so $g \circ f \circ h = id \circ h = h$
$g \circ f \circ h = g \circ id = g$

# Definition
A function $f : A \rightarrow B$ is said to be bijective or a bijection whenever there exists a (necesserily unique) function $g : B \rightarrow A$ (referred to as the inverse of $f$) such that:

1. $g$ is a retraction (or left inverse) for $f$:
	- $g \circ f = id_A$
2. $g$ is a section (or right inverse) for $f$:
	- $f \circ g = id_B$
![[Pasted image 20220129155928.png]]
![[Pasted image 20220129160040.png]]
![[Pasted image 20220129160213.png]]
Whenever there is an element in the target of a function which is not hit by the function, the function is not bijective as it cannot be reverse to hit the element.
![[Pasted image 20220129160436.png]]
Proposition: A function $f: A \rightarrow B$ is a bijection iff
$$\forall b \in B. \exists! a \in A. f(a) = b.$$
(unique a)
Hence $f$ is bijective as the unique $a$ that maps to $b$ is the inverse of $f$ applied to $B$.


