# 拉斯变换与傅里叶变换

傅里叶变换是拉斯变换在虚轴上的特例！！！
所以如果信号的傅里叶变换存在的话$\Rightarrow$其拉斯变换的收敛域一定包含$\sigma=0$ 

拉斯变换存在收敛域问题，而傅里叶变换没有，因为傅里叶变换实质只是拉斯变换的收敛域中某一点的状态。记拉斯变换写清楚收敛域

在大多数情况下，用s代替jω或则用jω代替s则可以实现拉斯变换和傅里叶变换的转换

对于信号的变换域求解，用拉斯变换。频谱分析用傅里叶变换

对于复指数信号经过LTI系统，计算如下：
$$
\begin{align*}
x(t)=e^{at} \Rightarrow y(t)=H(a)e^{at}  \quad 要求s=a要在H(s)的收敛域中
\end{align*}
$$

---

## 傅里叶变换性质：

$$
\begin{align*}

线性:a_{1}f_{1}(t)+a_{2}f_{2}(t) \leftrightarrow &a_{1}F_{1}(\omega)+a_{2}F_{2}(\omega)
\\
\\
时移特性:f(t-t_{0}) \leftrightarrow &e^{-j\omega t_{0}}F(j\omega)
\\
\\
频移特性:e^{j\omega_{0}t}f(t) \leftrightarrow &F(\omega-\omega_{0})
\\
\\
尺度变换:	f(at) \leftrightarrow &\frac{1}{|a|}F(\frac{\omega}{a})
\\
\\
共轭对称性:（和FS完全一样）
\\
f(t)是实信号: F(\omega)=F^*(-\omega) &\quad F(-\omega)=F^*(\omega)
\\
\\
f(t)是实偶信号:F(\omega)=F(-\omega)=&F^*(\omega) \quad F(\omega)实偶
\\
\\
f(t)是实奇信号:F(\omega)=-F(-\omega)=&-F^*(\omega) \quad F(\omega)虚奇
\\
\\
实信号f(t)的偶部:& Re\{F{(\omega)}\}
\\
\\
实信号f(t)的奇部: & jIm\{F{(\omega)}\}
\\
\\
对偶性:F(t) \leftrightarrow & 2\pi f(-\omega)
\\
\\
时域卷积:f(t)*h(t) \leftrightarrow & F(\omega)H(\omega)
\\
\\
时域微分:\frac{d^nf(t)}{dt^n} \leftrightarrow & (j\omega)^nF(\omega)
\\
\\
时域积分:\int_{-\infty}^{t}f(\tau)d\tau \leftrightarrow & \frac{F(\omega)}{j\omega}+\pi F(0)\delta(\omega)
\\
\\
帕斯瓦尔定理:\int_{-\infty}^{+\infty}|f(t)|^2dt =& \frac{1}{2\pi}\int_{-\infty}^{+\infty}|F(\omega)|^2d\omega
\\
\\
幅度调制特性:f_{1}(t)f_{2}(t) \leftrightarrow & \frac{1}{2\pi}F_{1}(\omega)*F_{2}(\omega)
\\
\\
频域微分:(-jt)^nf(t) \leftrightarrow & \frac{d^nF(\omega)}{d\omega^n}
\\
\\
频域积分:\frac{f(t)}{-jt}+\pi f(0)\delta(t) \leftrightarrow & \int_{-\infty}^{\omega}F(\theta)d\theta

\end{align*}
$$

## 拉斯变换的性质

$$
\begin{align*}
时移性质：f(t-t_{0})\quad \leftrightarrow & \quad e^{-st_{0}}F(s)
\\\\
频移性质：f(t)e^{s_{0}t}\quad \leftrightarrow &\quad F(s-s_{0})
\\\\
尺度变换：f(at) \quad \leftrightarrow & \quad \frac{1}{|a|}F(\frac{s}{a})
\\\\
时域卷积：f(t)*h(t) \quad \leftrightarrow &\quad F(s)H(s)
\\\\
时域微分：\frac{df(t)}{dt} \quad \leftrightarrow &\quad sF(s)	\quad 对于双边成立
\\\\
时域积分：\int_{-\infty}^{t}f(\tau)d\tau \quad \leftrightarrow &\quad \frac{1}{s}F(s)	\quad 对于因果信号成立
\\\\
s域微分：-tf(t) \quad \leftrightarrow &\quad \frac{dF(s)}{ds}
\\\\
初值定理：f(0^+)=\lim_{t \to 0^+}f(t)=&\lim_{s\to \infty}sF(s) \quad 0时刻无冲激
\\\\
终值定理：f(\infty)=\lim_{t \to \infty}f(t)=&\lim_{s \to 0}sF(s) \quad sF(s)收敛域包含虚轴
\end{align*}
$$

