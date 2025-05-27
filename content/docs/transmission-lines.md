+++
weight = 1
title = 'Transmission line equations'
date = 2024-01-14T07:07:07+01:00
+++

# A few transmission line equations

<p align="center"><img alt="Figure 8.9: Transmission line of length l connected on one end to a generator circuit and on the other end to a load Z_L. The load is located at z=0 and the generator terminals are at z=l." src="/airspace/img/f2.09.png" /></p>

Figure 8.9: Transmission line of length \(l\) connected on one end to a generator circuit and on the other end to a load \(Z_{L}\). The load is located at \(z=0\) and the generator terminals are at \(z=l\).

source: https://eme2e.eecs.umich.edu/figs/f2.09.pdf (from https://eme2e.eecs.umich.edu/figs/figs8.html)

## Equations

### Complex propagation constant and traveling wave solutions of the wave equations

\[\gamma=\alpha+j\beta\]

where \(\gamma\) is the complex propagation constant of the transmission line, \(\alpha\) is the attenutation constant of the line with units of \(\frac{\text{Np}}{\text{m}}\), \(\beta\) is the phase constant of the line with units of \(\frac{\text{rad}}{\text{m}}\).

The magnitude of the voltage phasor \(\tilde{V}\left(z\right)\) in a transmission line is

### Magnitude of voltage and current phasors

The magnitude of the voltage phasor \(\tilde{V}\left(z\right)\) in a transmission line is

{{< katex display=true >}}
\begin{split}
\left|\tilde{V}\left(z\right)\right|&=\left|V_0^+\right|\left(e^{-2\alpha z}+\left|\Gamma\right|^2e^{2\alpha z}+2\left|\Gamma\right|\cos\left(2\beta z+\theta_r\right)\right)^{\frac{1}{2}}\\
&=\left|V_0^+\right|\sqrt{e^{-2\alpha z}+\left|\Gamma\right|^2e^{2\alpha z}+2\left|\Gamma\right|\cos\left(2\beta z+\theta_r\right)}
\end{split}
{{< /katex >}}

The magnitude of the voltage phasor \(\tilde{V}\left(z\right)\) in a *lossless* transmission line is

\[\begin{split}
\left|\tilde{V}\left(z\right)\right|&=\left|V_0^+\right|\left(1+\left|\Gamma\right|^2+2\left|\Gamma\right|\cos\left(2\beta z+\theta_r\right)\right)^{\frac{1}{2}}\\
&=\left|V_0^+\right|\sqrt{1+\left|\Gamma\right|^2+2\left|\Gamma\right|\cos\left(2\beta z+\theta_r\right)}
\end{split}\]

Note that spatial position \(z=-l\) corresponds to the sending end (generator terminals) and spatial position \(z=0\) corresponds to the location of the load. Coordinate \(d\) is defined as \(d=-z\) and denotes distance from the load. Since cosine is an even function (\(\cos\left(-x\right)=\cos\left(x\right)\)), we also know that

\[
\begin{split}
\left|\tilde{V}\left(d\right)\right|&=\left|V_0^+\right|\left(1+\left|\Gamma\right|^2+2\left|\Gamma\right|\cos\left(2\beta d-\theta_r\right)\right)^{\frac{1}{2}}\\
&=\left|V_0^+\right|\sqrt{1+\left|\Gamma\right|^2+2\left|\Gamma\right|\cos\left(2\beta d-\theta_r\right)}
\end{split}
\]

## Derivation

This can be derived using the formula for the voltage phasor in a lossless (\(\gamma=j\beta\)) transmission line \(\tilde{V}\left(z\right)=V_0^+\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)\). The derivation is as follows.

\[\left|\tilde{V}\left(z\right)\right|=\left(\tilde{V}\left(z\right)\tilde{V}^{*}\left(z\right)\right)^{\frac{1}{2}}\]

\[\left|\tilde{V}\left(z\right)\right|=\left(\left(V_0^+\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)\right)\left(\left(V_0^+\right)^{*}\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)^{*}\right)\right)^{\frac{1}{2}}\]

\[\left|\tilde{V}\left(z\right)\right|=\left(V_0^+\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)\left(V_0^+\right)^{*}\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)^{*}\right)^{\frac{1}{2}}\]

\[\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)\left(e^{-j\beta z}+\Gamma e^{j\beta z}\right)^{*}\right)^{\frac{1}{2}}\]

\[\Gamma=\left|\Gamma\right|e^{j\theta_r}\]

\[\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(\left(e^{-j\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{j\beta z}\right)\left(e^{-j\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{j\beta z}\right)^{*}\right)^{\frac{1}{2}}\]

\[\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(\left(e^{-j\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{j\beta z}\right)\left(\left(e^{-j\beta z}\right)^{*}+\left(\left|\Gamma\right|e^{j\theta_r}e^{j\beta z}\right)^{*}\right)\right)^{\frac{1}{2}}\]

\[\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(\left(e^{-j\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{j\beta z}\right)\left(e^{j\beta z}+\left|\Gamma\right|e^{-j\theta_r}e^{-j\beta z}\right)\right)^{\frac{1}{2}}\]

\[\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(1+\left|\Gamma\right|e^{-j\theta_r}e^{-j2\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{j2\beta z}+\left|\Gamma\right|^2\right)^{\frac{1}{2}}\]

\[\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(1+\left|\Gamma\right|^2+\left|\Gamma\right|\left(e^{j\left(2\beta z+\theta_r\right)}+e^{-j\left(2\beta z+\theta_r\right)}\right)\right)^{\frac{1}{2}}\]

\[e^{jx}+e^{-jx}=2\cos\left(x\right)\]

\[\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(1+\left|\Gamma\right|^2+2\left|\Gamma\right|\cos\left(2\beta z+\theta_r\right)\right)^{\frac{1}{2}}\]

Note that in the lossy case (\(\gamma=\alpha+j\beta\)), the result is

\[\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(\left(e^{-\alpha z-j\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{\alpha z+j\beta z}\right)\left(e^{-\alpha z-j\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{\alpha z+j\beta z}\right)^{*}\right)^{\frac{1}{2}}\]

\[\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(\left(e^{-\alpha z}e^{-j\beta z}+\left|\Gamma\right|e^{\alpha z}e^{j\theta_r}e^{j\beta z}\right)\left(e^{-\alpha z}e^{j\beta z}+\left|\Gamma\right|e^{\alpha z}e^{-j\theta_r}e^{-j\beta z}\right)\right)^{\frac{1}{2}}\]

\[\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(e^{-2\alpha z}+\left|\Gamma\right|e^{-j\theta_r}e^{-j2\beta z}+\left|\Gamma\right|e^{j\theta_r}e^{j2\beta z}+\left|\Gamma\right|^2e^{2\alpha z}\right)^{\frac{1}{2}}\]

\[\left|\tilde{V}\left(z\right)\right|=\left|V_0^+\right|\left(e^{-2\alpha z}+\left|\Gamma\right|^2e^{2\alpha z}+2\left|\Gamma\right|\cos\left(2\beta z+\theta_r\right)\right)^{\frac{1}{2}}\]

## References

See page 67 (Section 2-6.2: Standing Waves) of the following text:

Fawwaz Tayssir Ulaby and Umberto Ravaioli. *Fundamentals of Applied Electromagnetics*. Pearson. 8th edition, 2020. ISBN-10 0136681581. ISBN-13 9780136681588.

See page 261 (PDF page 276) (Section 8-5.2: Standing Waves) of the following text: https://www.fulcrum.org/ebooks/0p0969731/download (ISBNs: 9781607859116 (hardcover); 9781607859123 (open access, electronic))

The above link is from https://doi.org/10.3998/mpub.13073174 https://www.fulcrum.org/concern/monographs/r781wk11q