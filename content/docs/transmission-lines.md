+++
weight = 1
title = 'Transmission Lines'
date = 2024-01-14T07:07:07+01:00
+++
## Transmission Lines

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
and denotes distance from the load.

This can be derived using the formula for the voltage phasor in a lossless transmission line ({{< katex >}}\gamma=j\beta{{< /katex >}})
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
