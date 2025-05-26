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

For any \(\vec{\mathbf{w}}\in\left(0,1\right)\cup\left(1,\infty\right)\) and any \(\vec{\mathbf{x}}\in\mathbb{R}_{+}\), we can find a scalar \(c\) such that \(c\odot\vec{\mathbf{w}}=\vec{\mathbf{x}}\). Therefore, \(c\odot\vec{\mathbf{w}}\) spans \(\mathbb{R}_{+}\). Since there is \(1\) basis vector, the dimension of the vector space is \(1\).

Define the transformation (or function or mapping) \(T\colon\mathbb{R}^{+}\to\mathbb{R}\) as \(T\left(\vec{\mathbf{u}}\right)=\log_{\vec{\mathbf{w}}}\left(\vec{\mathbf{u}}\right)\). isomorphism

To prove that \(T\) is one-to-one (injective), we can prove that if \(T\left(\vec{\mathbf{u}}\right)=T\left(\vec{\mathbf{v}}\right)\), then \(\vec{\mathbf{u}}=\vec{\mathbf{v}}\).

\[T\left(\vec{\mathbf{u}}\right)=T\left(\vec{\mathbf{v}}\right)=\log_{\vec{\textbf{w}}}\left(\vec{\mathbf{u}}\right)=\log_{\vec{\textbf{w}}}\left(\vec{\mathbf{v}}\right)\]

\[\vec{\textbf{w}}^{\log_{\vec{\textbf{w}}}\left(\vec{\mathbf{u}}\right)}=\log_{\vec{\textbf{w}}}\left(\vec{\mathbf{u}}\right)=\vec{\textbf{w}}^{\log_{\vec{\textbf{w}}}\left(\vec{\mathbf{v}}\right)}\Rightarrow\]

onto (surjective)

To prove that \(T\) is linear, we can prove that \(T\left(\vec{\mathbf{u}}\oplus\vec{\mathbf{v}}\right)=T\left(\vec{\mathbf{u}}\right)+T\left(\vec{\mathbf{v}}\right)\).

\[T\left(\vec{\mathbf{u}}\oplus\vec{\mathbf{v}}\right)=\log_{\vec{\textbf{w}}}\left(\vec{\mathbf{u}}\oplus\vec{\mathbf{v}}\right)=\log_{\vec{\textbf{w}}}\left(\vec{\mathbf{u}}\vec{\mathbf{v}}\right)=\log_{\vec{\textbf{w}}}\left(\vec{\mathbf{u}}\right)+\log_{\vec{\textbf{w}}}\left(\vec{\mathbf{v}}\right)=T\left(\vec{\mathbf{u}}\right)+T\left(\vec{\mathbf{v}}\right)\]

Therefore, \(T\) is an isomorphism from \(\mathbb{R}^{+}\) onto \(\mathbb{R}\).

## References

https://math.stackexchange.com/questions/1332747/proof-that-mathbbr-is-a-vector-space

https://math.stackexchange.com/questions/1361445/proving-that-v-is-a-vector-space-if-ab-ab-and-a-b-ab

https://www.stat.uchicago.edu/~lekheng/courses/110f07/math110-hw1sol.pdf

https://www.math.stonybrook.edu/~scott/mat310.spr05/docs/LogAsIsomorphism.pdf

https://sites.lafayette.edu/thompsmc/files/2015/12/HW7_2_Key.pdf

http://matematika.reseneulohy.cz/2504/the-space-of-positive-real-numbers

https://proofwiki.org/wiki/Definition:Strictly_Positive/Real_Number