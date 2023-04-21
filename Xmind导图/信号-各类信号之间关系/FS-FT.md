# 傅里叶级数与傅里叶变换

## 区别

傅里叶级数：FS
要求：
	1.信号具有周期性
	2.周期绝对可积
	3.周期有限个最值
	4.周期有限个非无穷间断点

傅里叶变换：FT
要求：
	1.都可以，就是不论周期信号还是非周期信号都可以存在傅里叶变换
	2.FT无穷区间绝对可积
	3.FT无穷区间有限个最值
	4.FT无穷区间有限个非无穷间断点



## 联系

对于周期信号x(t)
傅里叶级数表示如下：
$$
\begin{align*}
f(t)=&\sum_{k=-\infty}^{+\infty}a_{k}e^{jk\omega_{0} t}
\\
a_{k}=&\frac{1}{T}\int_{t_{1}}^{t_{1}+T}f(t)e^{-jk\omega_{0}t}dt
\end{align*}
$$
傅里叶变换表示如下：
$$
F(j\omega)=2\pi\sum_{k=-\infty}^{+\infty}a_{k}\delta(\omega-k\frac{2\pi}{T})
$$


