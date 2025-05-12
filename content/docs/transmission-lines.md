+++
weight = 1
title = 'Transmission line equations'
date = 2024-01-14T07:07:07+01:00
+++
## A few transmission line equations

The magnitude of the voltage phasor
{{< katex >}}
\tilde{V}\left(z\right)
{{< /katex >}}
in a *lossless* transmission line is

{{< katex display=true >}}
\begin{split}
\left|\tilde{V}\left(z\right)\right|&=\left|V_0^+\right|\left(1+\left|\Gamma\right|^2+2\left|\Gamma\right|\cos\left(2\beta z+\theta_r\right)\right)^{\frac{1}{2}}\\
&=\left|V_0^+\right|\sqrt{1+\left|\Gamma\right|^2+2\left|\Gamma\right|\cos\left(2\beta z+\theta_r\right)}
\end{split}
{{< /katex >}}

Note that spatial position
{{< katex >}}
z=-l
{{< /katex >}}
corresponds to the sending end (generator terminals) and spatial position
{{< katex >}}
z=0
{{< /katex >}}
corresponds to the location of the load. Coordinate{{< katex >}}d{{< /katex >}}is defined as
{{< katex >}}
d=-z
{{< /katex >}}
and denotes distance from the load. Since cosine is an even function ({{< katexModified >}}\cos\left(-x\right)=\cos\left(x\right){{< /katexModified >}}), we also know that

{{< katex display=true >}}
\begin{split}
\left|\tilde{V}\left(d\right)\right|&=\left|V_0^+\right|\left(1+\left|\Gamma\right|^2+2\left|\Gamma\right|\cos\left(2\beta d-\theta_r\right)\right)^{\frac{1}{2}}\\
&=\left|V_0^+\right|\sqrt{1+\left|\Gamma\right|^2+2\left|\Gamma\right|\cos\left(2\beta d-\theta_r\right)}
\end{split}
{{< /katex >}}

This can be derived using the formula for the voltage phasor in a lossless ({{< katexModified >}}\gamma=j\beta{{< /katexModified >}}) transmission line
{{< katex >}}
\tilde{V}\left(z\right)=V_0^+\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)
{{< /katex >}}
. The derivation is as follows.

{{< katex display=true >}}
\left|\tilde{V}\left(z\right)\right|=\left(\tilde{V}\left(z\right)\tilde{V}^{*}\left(z\right)\right)^{\frac{1}{2}}
{{< /katex >}}

{{< katex display=true >}}
\left|\tilde{V}\left(z\right)\right|=\left(\left(V_0^+\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)\right)\left(\left(V_0^+\right)^{*}\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)^{*}\right)\right)^{\frac{1}{2}}
{{< /katex >}}

{{< katex display=true >}}
\left|\tilde{V}\left(z\right)\right|=\left(V_0^+\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)\left(V_0^+\right)^{*}\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)^{*}\right)^{\frac{1}{2}}
{{< /katex >}}

{{< katex display=true >}}
\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)^{*}\right)^{\frac{1}{2}}
{{< /katex >}}

{{< katex display=true >}}
\Gamma=\left|\Gamma\right|e^{j\theta_r}
{{< /katex >}}

{{< katex display=true >}}
\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(\left(e^{-j\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{j\beta z}\right)\left(e^{-j\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{j\beta z}\right)^{*}\right)^{\frac{1}{2}}
{{< /katex >}}

{{< katex display=true >}}
\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(\left(e^{-j\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{j\beta z}\right)\left(\left(e^{-j\beta z}\right)^{*}+\left(\left|\Gamma\right|e^{j\theta_r}e^{j\beta z}\right)^{*}\right)\right)^{\frac{1}{2}}
{{< /katex >}}

{{< katex display=true >}}
\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(\left(e^{-j\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{j\beta z}\right)\left(e^{j\beta z}+\left|\Gamma\right|e^{-j\theta_r}e^{-j\beta z}\right)\right)^{\frac{1}{2}}
{{< /katex >}}

{{< katex display=true >}}
\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(1+\left|\Gamma\right|e^{-j\theta_r}e^{-j2\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{j2\beta z}+\left|\Gamma\right|^2\right)^{\frac{1}{2}}
{{< /katex >}}

{{< katex display=true >}}
\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(1+\left|\Gamma\right|^2+\left|\Gamma\right|\left(e^{j\left(2\beta z+\theta_r\right)}+e^{-j\left(2\beta z+\theta_r\right)}\right)\right)^{\frac{1}{2}}
{{< /katex >}}

{{< katex display=true >}}
e^{jx}+e^{-jx}=2\cos\left(x\right)
{{< /katex >}}

{{< katex display=true >}}
\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(1+\left|\Gamma\right|^2+2\left|\Gamma\right|\cos\left(2\beta z+\theta_r\right)\right)^{\frac{1}{2}}
{{< /katex >}}

See page 67 (Section 2-6.2: Standing Waves) of the following text:

Fawwaz T. Ulaby and Umberto Ravaioli. *Fundamentals of Applied Electromagnetics*. Pearson. 8th edition, 2020. ISBN-10 0136681581. ISBN-13 9780136681588.

See page 261 (PDF page 276) (Section 8-5.2: Standing Waves) of the following text: https://www.fulcrum.org/ebooks/0p0969731/download (ISBNs: 9781607859116 (hardcover); 9781607859123 (open access, electronic))

The above link is from https://doi.org/10.3998/mpub.13073174 https://www.fulcrum.org/concern/monographs/r781wk11q
