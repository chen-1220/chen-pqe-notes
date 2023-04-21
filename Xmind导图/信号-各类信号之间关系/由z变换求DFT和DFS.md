# 由Z变换求DFT与DFS

为什么要这么做，因为DFT与DFS在考纲里面是没有的，但是在真题里面却又考了！！！
所以希望利用学过的z变换去规避掉这个问题

## z变换求DFT

这个很简单，只需要令$z=e^{j\Omega}$带入H(z)中即可得到DFT：离散傅里叶变换H(Ω)
$$
F(\Omega)=F(z)|_{z=e^{j\Omega}}
$$


## z变换求DFS

首先对周期信号取他的一个周期波形做z变换，然后令$z=e^{jk\Omega_0}$并且需要乘系数$\frac{1}{N}$
$$
a_k=\frac{1}{N}H(z)|_{z=e^{jk\Omega_0}}
$$


## 几种变换关系如下：

z变换的正反变换式如下：
$$
\begin{align*}
&F(z)=\sum\limits_{n=-\infty}^{+\infty}f[n]z^{-n}\\
&f[n]=\frac{1}{ 2 \pi j}\oint F(z)z^{n-1}dz
\end{align*}
$$
DFT的正反变换式如下：
$$
\begin{align*}
&F(\Omega)=\sum_{n=-\infty}^{\infty}f[n]e^{-j\Omega n}
\\
&f[n]=\frac{1}{2\pi}\int_{2\pi}F(\Omega)e^{j\Omega n}d\Omega
\end{align*}
$$


DFS的正反变换式如下：
$$
\begin{align*}
&f[n]=\sum_{k=<N>}a_ke^{jk\Omega_0n}
\\
&a_k=\frac{1}{N}\sum_{n=<N>}f[n]e^{-jk\Omega_0n}
\\\\
&\sum_{k=<N>}=\sum_{k=-\frac{N}{2}}^{\frac{N}{2}-1}
\end{align*}
$$
