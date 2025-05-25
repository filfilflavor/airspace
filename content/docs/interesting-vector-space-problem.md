+++
weight = 3
title = 'An interesting vector space problem'
date = 2024-01-14T07:07:07+01:00
+++

# An interesting vector space problem with \(\mathbb{R}_{+}\)

## Statement

Denote by the set \(\mathbb{R}_{+}\) as the [strictly positive real numbers](https://proofwiki.org/wiki/Definition:Strictly_Positive/Real_Number).

{{< katex display=true >}}
\mathbb{R}_{+}=\left\{x\in\mathbb{R}\mid x>0\right\}
{{< /katex >}}

Vector addition in \(\mathbb{R}_{+}\) is defined in the following manner (\(\mathbf{u},\mathbf{v}\in\mathbb{R}^{+}\)):

\[\mathbf{u}\oplus\mathbf{v}=\mathbf{u}\mathbf{v}\]

Scalar multiplication in \(\mathbb{R}_{+}\) is defined in the following manner (\(\mathbf{u}\in\mathbb{R}^{+}\) and \(c\in\mathbb{R}\)):

\[c\odot\mathbf{u}=\mathbf{u}^{c}\]

Prove that \(\mathbb{R}_{+}\) is a vector space.

## Proof

\[c=\log_{\mathbf{u}}\left(c\odot\mathbf{u}\right)\]

\[\mathbf{u}=\mathbf{v}^{\log_{\mathbf{v}}\left(\mathbf{u}\oplus\mathbf{v}\right)-1}\]

## References

https://math.stackexchange.com/questions/1332747/proof-that-mathbbr-is-a-vector-space

https://math.stackexchange.com/questions/1361445/proving-that-v-is-a-vector-space-if-ab-ab-and-a-b-ab

https://www.stat.uchicago.edu/~lekheng/courses/110f07/math110-hw1sol.pdf

https://www.math.stonybrook.edu/~scott/mat310.spr05/docs/LogAsIsomorphism.pdf

https://sites.lafayette.edu/thompsmc/files/2015/12/HW7_2_Key.pdf

http://matematika.reseneulohy.cz/2504/the-space-of-positive-real-numbers

https://proofwiki.org/wiki/Definition:Strictly_Positive/Real_Number