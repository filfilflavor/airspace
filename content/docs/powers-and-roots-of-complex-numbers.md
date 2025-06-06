+++
weight = 2
title = 'Powers and roots of complex numbers'
date = 2025-05-24T04:00:00+00:00
+++

# Powers and roots of complex numbers

{{% hint warning %}}
in progress

need to fix circularity

principal root is the one with the largest real component
{{% /hint %}}

<p align="center"><img alt="Geometric representation of the 2nd to 6th roots of a complex number z, in polar form re^{iφ} where r = |z| and φ = arg z. If z is real, φ = 0 or π. Principal roots are shown in black." src="/airspace/img/Visualisation_complex_number_roots.svg" width="400" /></p>

Geometric representation of the 2nd to 6th roots of a complex number \(z\), in polar form \(re^{i\varphi}\) where \(r=\left|z\right|\) and \(\varphi=\arg z\). If \(z\) is real, \(\varphi=0\) or \(\pi\). Principal roots are shown in black.

image from https://commons.wikimedia.org/wiki/File:Visualisation_complex_number_roots.svg. caption from https://en.wikipedia.org/wiki/Nth_root#nth_roots

## Statement

Denote by \(z\) a complex number with modulus \(r\) and argument \(\theta\) (\(z=re^{i\theta}\)).

### Powers of \(z\)

If \(x^{\frac{1}{n}}=z\) where \(n\in\mathbb{R}\) and \(n\ne0\), what are all possible solutions for \(x\)?

In general, we can represent all possible solutions for \(x\) as

{{< katex display=true >}}
x\in\left\{r^{n}e^{i\left(\theta n+2\pi nk\right)}\mid k\in\mathbb{Z}\right\}
{{< /katex >}}

If \(n\) is an integer, then we can reduce this to

\[x=r^{n}e^{i\theta n}\]

### Roots of \(z\)

If \(x^{n}=z\) where \(n\in\mathbb{R}\) and \(n\ne0\), what are all possible solutions for \(x\)? (This means that out of all possible powers of \(x\), at least one of them is \(z\).)

In general, we can represent all possible solutions for \(x\) as

\[x\in\left\{r^{\frac{1}{n}}e^{i\frac{\theta+2\pi k}{n}}\mid k\in\mathbb{Z}\right\}\]

If \(n\) is an integer, then we can reduce this to

\[x\in\left\{r^{\frac{1}{n}}e^{i\frac{\theta+2\pi k}{n}}\mid k\in\left\{0,1,2,\dots,\left|n\right|-1\right\}\right\}\]

Not realizing this, many people omit the addend \(i\frac{2\pi k}{n}\) in the exponent of \(e\) and simply state that \(x=e^{i\frac{\theta}{n}}\). While \(e^{i\frac{\theta}{n}}\) is a possible solution for \(x\) (we can obtain this principal root from the above formula by simply setting \(k\) to \(0\)), it does not include all possible solutions for \(x\).

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

https://math.stackexchange.com/questions/322481/principal-nth-root-of-a-complex-number

https://www.reddit.com/r/askmath/comments/17sztny/principal_square_root_of_complex_numbers/