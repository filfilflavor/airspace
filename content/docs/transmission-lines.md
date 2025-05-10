+++
weight = 1
title = 'Transmission Lines'
date = 2024-01-14T07:07:07+01:00
+++
## Transmission Lines

{{< katex display=true >}}
\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\sqrt{1+\left|\Gamma\right|^2+2\left|\Gamma\right|\cos\left(2\beta z+\theta_r\right)}
{{< /katex >}}

This can be derived from

{{< katex display=true >}}
\tilde{V}\left(z\right)=V_0^+\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)
{{< /katex >}}

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
\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(1+\left|\Gamma\right|e^{-j\theta_r}e^{-j2\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{j2\beta z}+e^{j\beta z}+\left|\Gamma\right|e^{-j\theta_r}e^{-j\beta z}\right)^{\frac{1}{2}}
{{< /katex >}}
