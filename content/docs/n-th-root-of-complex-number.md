+++
weight = 2
title = 'n-th root of a complex number'
date = 2024-01-14T07:07:07+01:00
+++

# \(n\)<sup>th</sup> root of a complex number

<p align="center"><img alt="" src="/airspace/img/Visualisation_complex_number_roots.svg" /></p>

image from https://commons.wikimedia.org/wiki/File:Visualisation_complex_number_roots.svg

## Statement

Denote by \(z\) a complex number with modulus \(r\) and argument \(\theta\) (\(z=re^{i\theta}\)).

If \(x^{\frac{1}{n}}=z\) where \(n\in\mathbb{R}\), what are all possible solutions for \(x\)?

In general, we can represent all possible solutions for \(x\) as

\[x\in\left\{r^{n}e^{i\left(\theta n+2k\pi n\right)}\mid k\in\mathbb{Z}\right\}\]

If \(x^{n}=z\) where \(n\in\mathbb{R}\), what are all possible solutions for \(x\)?

In general, we can represent all possible solutions for \(x\) as

\[x\in\left\{r^{\frac{1}{n}}e^{i\frac{\theta+2k\pi}{n}}\mid k\in\mathbb{Z}\right\}\]

If \(n\) is an integer, then we can reduce this to

\[x\in\left\{r^{\frac{1}{n}}e^{i\frac{\theta+2k\pi}{n}}\mid k\in\left\{0,1,2,\dots,n-1\right\}\right\}\]

{{< katex display=true >}}
z^{\frac{1}{n}}=\left(e^{i\theta}\right)^{\frac{1}{n}}=e^{i\left(\frac{\theta+2\pi k}{n}\right)}
{{< /katex >}}

where \(k\in\mathbb{Z}\). Not realizing this, many people omit the \(i\frac{2\pi k}{n}\) in the exponent and simply state that \(z^{\frac{1}{n}}=e^{\frac{i\theta}{n}}\). While true (simply set \(k\) to \(0\)), it does not include all possible solutions.

## Proof

\[z=e^{i\theta}=\cos\left(\theta\right)+i\sin\left(\theta\right)=\operatorname{cis}\left(\theta\right)\]

Because \(\cos\left(\theta\right)=\cos\left(\theta+2\pi k\right)\) and \(\sin\left(\theta\right)=\sin\left(\theta+2\pi k\right)\),

\[z=\cos\left(\theta+2\pi k\right)+i\sin\left(\theta+2\pi k\right)=\operatorname{cis}\left(\theta+2\pi k\right)=e^{i\left(\theta+2\pi k\right)}\]

\[z=e^{i\theta}=e^{i\left(\theta+2\pi k\right)}\]

Therefore, \(z^{n}\) is

\[z^{n}=\left(e^{i\left(\theta+2\pi k\right)}\right)^{n}=e^{i\left(\theta n+2\pi kn\right)}\]

Since \(2\pi kn\) is an integer multiple of \(2\pi\) if both \(k\in\mathbb{Z}\) and \(n\in\mathbb{Z}\), it is correct to state the following:

\[z^{n}=e^{i\theta n}=\cos\left(\theta n\right)+i\sin\left(\theta n\right)\]

However, \(z^{\frac{1}{n}}\) is

\[z^{\frac{1}{n}}=\left(e^{i\left(\theta+2\pi k\right)}\right)^{\frac{1}{n}}=e^{i\left(\frac{\theta+2\pi k}{n}\right)}=e^{i\left(\frac{\theta}{n}+2\pi\cdot\frac{k}{n}\right)}\]

When \(n\ne0\) and \(n\ne\pm1\), \(2\pi\cdot\frac{k}{n}\) is not an integer multiple of \(2\pi\) for all \(k\in\mathbb{Z}\) (meaning, there exists at least one value of \(k\in\mathbb{Z}\) for which \(\frac{k}{n}\) is not an integer). Therefore, we do *not* reduce \(z^{\frac{1}{n}}\) to \(e^{\frac{i\theta}{n}}\).

## References