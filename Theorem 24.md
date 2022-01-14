For all integers $l$, $m$, $n$, if $l|m$ and $m|n$ then $l|n$.

Proof: Let $l$, $m$, $n$ be arbitrary integers.
Assume $l|m$ and $m|n$

By definition
$l|m \iff \exists i. l \cdot i = m$ (1)
and 
$m|n \iff \exists j. m \cdot j = n$ (2)

RTP $l|n$ or by definition $\exists k. l \cdot k = n$

From (1), we have an integer $i_0$ with the property $l \cdot i_0 = m$

From (2), we have an integer $j_0$ with the property $m \cdot j_0 = n$

Then $n = m \cdot j_0 = l \cdot (i_0 \cdot j_0)$ so $l|n$ as or witness $k = i_0 \cdot j_0$.
QED.