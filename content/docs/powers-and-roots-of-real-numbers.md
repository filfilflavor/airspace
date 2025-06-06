+++
weight = 2
title = 'Exponentiation of real numbers to real exponents'
date = 2024-01-14T07:07:07+01:00
+++

# Exponentiation of real numbers to real exponents

{{% hint warning %}}
in progress
{{% /hint %}}

## Statement

For zero, if \(n>0\), then \(0^{n}=0\). If \(n<0\), then \(0^{n}\) is undefined.

> [In some contexts (e.g., combinatorics), the expression \(0^{0}\) is defined to be equal to \(1\); in others (e.g., analysis), it is often undefined.](https://en.wikipedia.org/wiki/Exponentiation#Powers_of_zero)

---

For a positive base, exponentiation to a real power cannot make the number negative or introduce any imaginary component to the number.

> [For positive real numbers... The result is always a positive real number, and the identities and properties shown above for integer exponents remain true with these definitions for real exponents.](https://en.wikipedia.org/wiki/Exponentiation)

{{< katex display=true >}}
b^{m}\cdot b^{n}=b^{m+n}
{{< /katex >}}
\[\left(b^{m}\right)^{n}=b^{m\cdot n}\]
\[b^{n}\cdot c^{n}=\left(b\cdot c\right)^{n}\]

This means that [for a rational number \(\frac{p}{q}\)](https://en.wikipedia.org/wiki/Exponentiation#Rational_exponents),

\[x^\frac pq= \left(x^p\right)^\frac 1q=(x^\frac 1q)^p\]

\(x^{\frac{1}{n}}\) or \(\sqrt[n]x\) denotes the unique nonnegative real \(n\)th root of \(x\). Even if there are multiple \(n\)th roots of \(x\), there is only one value of \(x^{\frac{1}{n}}\).

Irrational exponents can be defined using limits of rational exponents (this is intuitive). A [formal description of this](https://en.wikipedia.org/wiki/Exponentiation#Limits_of_rational_exponents) is

\[b^x = \lim_{r (\in \mathbb{Q}) \to x} b^r \quad (b \in \mathbb{R}^+,\, x \in \mathbb{R})\]

\[b^{-n}=\frac{1}{b^{n}}\]

---

For a negative base, exponentiation to a real power can introduce imaginary components.

Exponent rules hold for integer exponents.

\[\left(\left(-1\right)^{\frac{1}{2}}\right)^{2}=-1\]
\[\left(\left(-1\right)^{2}\right)^{\frac{1}{2}}=1\]
\[\left(-1\right)^{2\cdot\frac{1}{2}}=-1\]

\(\left(b^{m}\right)^{n}=b^{m\cdot n}\) does *not* hold. Instead, \(\left(b^{m}\right)^{n}\) must be calculated by first calculating \(b^{m}\), and then taking that result to the \(n\)th power.

\[b^{x}=\left(-b\right)^{x}\left(\cos\left(\pi x\right)+i\sin\left(\pi x\right)\right)\]

\[b^{x}=\left(-b\right)^{x}\left(\cos\left(\pi x+2\pi kx\right)+i\sin\left(\pi x+2\pi kx\right)\right)\]

Since \(-b\) is positive (\(-b=\left|b\right|\)), the rules above can be used for \(\left(-b\right)^{x}\).

Note that \(b\in\mathbb{R}\) if \(x\in\mathbb{Z}\), regardless of the choice of \(k\). \(\pi x+2\pi kx=\left(x+2kx\right)\pi\), and \(\left(x+2kx\right)\in\mathbb{Z}\). Therefore, \(\sin\left(\pi x+2\pi kx\right)=0\). We can reduce the expression to \(b^{x}=\left(-b\right)^{x}\cos\left(\pi x\right)\). This is what you would expect from repeated multiplication.

> [Therefore, exponentiation with a basis that is not a positive real number is generally viewed as a multivalued function.](https://en.wikipedia.org/wiki/Exponentiation)

\(\left(b^{m}\right)^{n}=b^{m\cdot n}\) holds for complex base and real exp?

\(b^{n}\cdot c^{n}=\left(b\cdot c\right)^{n}\) holds for complex base and real exp?

\(b^{m}\cdot b^{n}=b^{m+n}\) does not hold?

principal root = greatest real part, then greatest imaginary if real tied

## References

https://en.wikipedia.org/wiki/Exponentiation

https://math.stackexchange.com/questions/2114774/what-is-1x