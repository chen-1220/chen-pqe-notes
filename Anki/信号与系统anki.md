TARGET DECK
信号与系统


系统函数的相角函数 #flashcard 
$$
\begin{align*}
&H(\omega)=Ke^{-j\omega t_{0}}
\\\\
&|H(\omega)|=K \qquad \varphi_{H}(\omega)=-\omega t_{0}
\end{align*}
$$
<!--ID: 1669110257020-->


系统群时延公式 #flashcard 
$$
\tau(\omega)=-\frac{d\varphi_{H}(\omega)}{d\omega}
$$
<!--ID: 1669110257026-->


设计滤波器的时候需要考虑的因素 #flashcard
1.增益；2.通带最高最低频率
<!--ID: 1669110257030-->


时移性质的作用范围 #flashcard
针对信号中所有的t而言
<!--ID: 1669110257034-->


绝对值信号怎么处理 #flashcard
可以考虑u(t)分割信号
<!--ID: 1669110257037-->


周期信号怎么处理 #flashcard 
考虑周期冲激串的卷积性质
<!--ID: 1669110257042-->



常见tan函数 #flashcard
根据复数坐标确定其所在象限并以此限定$\angle H(j\omega)$的范围
1. $tan(\angle H(j\omega))=\omega$
![[Pasted image 20221116124850.png|800]]
2. $tan(\angle H(j\omega))=\frac{1}{\omega}$
![[Pasted image 20221116124249.png|800]]
3. $tan(\angle H(j\omega))=\frac{\omega}{\omega^2-a}$
![[Pasted image 20221116124658.png|800]]
<!--ID: 1669110257046-->




相关函数题怎么做 #flashcard 
 $r(t)=f_1(-t)*f_2(t)$
换元转换为卷积，然后拉斯变换；或者直接带入用数学方法做
<!--ID: 1669108427139-->

卷积公式是什么 #flashcard 
$$
\begin{cases}
f(t)*h(t)=\int_{-\infty}^{+\infty}f(\tau)\cdot h(t-\tau)d\tau=\int_{-\infty}^{+\infty}h(\tau)\cdot h(t-\tau)dt
\\\\
f[n]*h[n]=\sum_{k=-\infty}^{+\infty}f[k]*h[n-k]=\sum_{k=-\infty}^{+\infty}h[k]f[n-k]
\end{cases}
$$
<!--ID: 1669111081929-->



长除法怎么区分左边信号和右边信号 #flashcard 
右边信号降幂排
左边信号升幂排
<!--ID: 1669108427142-->


s域微分性质 #flashcard 
$$-tf(t) \quad \leftrightarrow \quad \frac{dF(s)}{ds}$$
<!--ID: 1669108427147-->


信号的全时域积分 #flashcard 
1.考虑帕斯瓦尔定理；2.转换为傅里叶变换定义
<!--ID: 1669108427150-->


周期信号与非周期信号帕斯瓦尔定理的区别 #flashcard 
周期信号帕斯瓦尔定理计算功率，非周期信号帕斯瓦尔定理计算能量
$$
\begin{align*}
&\frac{1}{T}\int_{T}|f(t)|^2dt=\sum_{k=-\infty}^{+\infty}|a_{k}|^2
\\\\
&\int_{-\infty}^{+\infty}|f(t)|^2dt = \frac{1}{2\pi}\int_{-\infty}^{+\infty}|F(\omega)|^2d\omega
\end{align*}
$$
<!--ID: 1669108427153-->


傅里叶逼近的推导采用什么原则 #flashcard 
均方收敛
<!--ID: 1669108427157-->


采样定理都有哪些 #flashcard 
奈奎斯特采样定理
- 采样频率$\omega_s \ge 2\omega_0$
带通采样定理
-  $\frac{2\omega_M}{m}\le \omega_s \le \frac{2\omega_L}{m-1}\quad m=[\frac{\omega_m}{B}]$,B为频谱带宽,$\omega_L,\omega_M$分别为最低与最高频率
- 当信号最低频率为0时，带通采样定理⇔奈奎斯特采样定理
<!--ID: 1669108427160-->


框图怎么转换为流图 #flashcard 
- 不要在表达式中出现常数项，如果出现，就将其合并到某一有理式项当中
- 框图转换成流图的方法
	1. 将加法器合并之后画成节点
	2. 小方框都改写成横线箭头，其方框内容重写到箭头上
	3. 反馈支路画成曲线，其它支路画成直线。箭头不再线段尾端而是在线段中间
<!--ID: 1669108427164-->

框图的三种形式 #flashcard 
直接：H(s)直接当做整体画框图
级联：H(s)表示为两个部分相乘，各部分单独画框图，一路相连
并联：H(s)表示为两个部分相加，各部分单独画框图，分出n路，最后汇合为一路
![[Pasted image 20221104172505.png]]
<!--ID: 1669110257050-->



欧拉公式 #flashcard 
$$
\begin{align*}
&e^{j\omega t}=cos(\omega t)+jsin(\omega t)
\\\\
&sin(\omega t) = \frac{1}{2j}(e^{j\omega t}-e^{-j\omega t}) 
\\
&cos(\omega t) = \frac{1}{2}(e^{j\omega t}+e^{-j\omega t}) 
\end{align*}
$$
<!--ID: 1669108738384-->



采样后的频谱有什么特点 #flashcard 
周期倒数被的无穷平移，可能导致频谱混叠
$$
Y(\omega)=\frac{1}{T_{s}}\sum_{k=-\infty}^{+\infty}F(\omega-k\omega_{s})
$$
<!--ID: 1669108427167-->


三角波的频谱 #flashcard 
$$
\begin{align*}
&x(t)=k(\frac{sin\ \omega_c t}{t})^2 \Rightarrow
X(j\omega)=
\begin{cases}
a|\omega|+b,&|\omega|<2\omega_c
\\\\
0,&其他
\end{cases}
\\\\
&a=-\frac{\pi}{2}k \qquad \qquad b=\omega_c\pi k
\\\\
&x(t)=\begin{cases}
a|t|+b, &|t|<2\tau
\\\\
0,&其他
\end{cases}
\Rightarrow X(j\omega)=-4a·\frac{sin^2(\tau\omega)}{\omega^2}
\end{align*}
$$
<!--ID: 1669110445897-->



f[n]的时域展宽性质 #flashcard 
$$
\begin{align*}
&时域展宽特性:f_{1}[n]\leftrightarrow F(z^N)
\\\\&f_1[n]=
\begin{cases}
f[\frac{n}{N}],&n为N的整数倍\\
\\
0,&其他
\end{cases}
\end{align*}
$$
<!--ID: 1669108427170-->




因果系统的逆系统也是因果的吗 #flashcard 
不一定
<!--ID: 1669108427174-->



实数信号的傅里叶变换意义 #flashcard 
F(ω)=F*(-ω)
<!--ID: 1669108427177-->


频谱分析的时候 #flashcard 
务必标记出所有频率分量
<!--ID: 1669110257055-->


f[Mn]的z变换怎么求解 #flashcard 
牢记怎么筛除非整数倍的点
$$
\begin{align*}
&f[m]=f[m]\frac{1}{M}\sum_{k=0}^{M-1}e^{-j\frac{2\pi}{M}mk}
\\\\
&表示只有m=kM  \qquad k=0,\pm1,\cdots的点非零
\end{align*}
$$
<!--ID: 1669108427180-->



电路题目 #flashcard 
转换为s域模型；明确是电流关系or电压关系
![[Pasted image 20221105154319.png]]
![[Pasted image 20221105154336.png]]
<!--ID: 1669108427184-->


网孔电流法 #flashcard 
- 以网孔的电流为待求量
- 电路中独立网孔的数量=方程的数量
- 所有网孔选择同一个方向，同顺时针或同逆时针
自回路电阻×自回路电流-互回路电阻×互回路电流=电压提升值
<!--ID: 1669108427187-->


周期冲激串的拉斯变换 #flashcard 
$$
\sum_{k=0}^{\infty}\delta(t-kT) \leftrightarrow  \frac{1}{1-e^{-sT}} \qquad \sigma>0
$$
<!--ID: 1669112072452-->





傅里叶级数定义 #flashcard
$$
\begin{align*}
\begin{cases}
x(t)=\sum_{k=-\infty}^{+\infty}a_ke^{jk\omega_0t}
\\\\
a_k=\frac{1}{T}\int_{T}x(t)e^{-jk\omega_0t}dt
\end{cases}
\end{align*}
$$
<!--ID: 1669111081934-->



离散傅里叶级数DFS定义  #flashcard
$$
\begin{align*} 
&x[n]=\sum_{k=<N>}a_ke^{jk\Omega_0n} 
\\
&a_k=\frac{1}{N}\sum_{n=<N>}x[n]e^{-jk\Omega_0n} 
\\\\ 
&\sum_{k=<N>}:表示一个周期里的累加
\end{align*}  
$$
<!--ID: 1669111081938-->


傅里叶变换FT定义  #flashcard


$$
\begin{align*}
&\begin{cases}
x(t)=\frac{1}{2\pi}\int_{-\infty}^{+\infty}X(j\omega)e^{j\omega t}d\omega
\\\\
X(j\omega)=\int_{-\infty}^{+\infty}x(t)e^{-j\omega t}dt
\end{cases}
\end{align*}
$$
<!--ID: 1669111756136-->


离散傅里叶变换DFT定义  #flashcard
$$
\begin{align*} 
&X(\Omega)=\sum_{n=-\infty}^{\infty}x[n]e^{-j\Omega n} 
\\ 
&x[n]=\frac{1}{2\pi}\int_{2\pi}X(\Omega)e^{j\Omega n}d\Omega 
\end{align*}  
$$
<!--ID: 1669111081942-->






拉普拉斯变换定义 #flashcard
<font color = red>表达式一定要带上收敛域</font>
$$
\begin{align*}
F(s)=&\int_{-\infty}^{+\infty}f(t)e^{-st}dt
\\
\\
f(t)=&\frac{1}{2\pi j}\int_{\sigma-j\infty}^{\sigma+j\infty}F(s)e^{st}ds
\end{align*}
$$
<!--ID: 1669190622409-->



Z变换定义 #flashcard
<font color =red>Z变换表达式由于常写作负幂次，所以要特别注意在零极图原点处可能出现的零点 </font>
$$
\begin{align*}
&F(z)=\sum\limits_{n=-\infty}^{+\infty}f[n]z^{-n}\\
&f[n]=\frac{1}{ 2 \pi j}\oint F(z)z^{n-1}dz
\end{align*}
$$
<!--ID: 1669110445906-->


离散傅里叶级数或变换一定有基波分量吗 #flashcard
未必有基波分量！！！
对于正弦信号求解傅里叶级数，直接用欧拉公式展开
<!--ID: 1669110682712-->



信号震荡频率 #flashcard
  信号频率越靠近奇数倍的$\pi:\pm \pi,\pm 3\pi \cdots$，其震荡频率越高
  信号频率越靠近偶数倍的$\pi:0,\quad \pm 2\pi \cdots$，其震荡频率越低
<!--ID: 1669110682716-->



三角波卷积三角波的图像长什么样子 #flashcard
![[Pasted image 20221103175506.png|700]]
<!--ID: 1669110682721-->


梅森公式 #flashcard
$$
\begin{align*}
&H(s)=\frac{1}{\Delta}\sum_{k=1}^{n}p_k\Delta_k
\\\\
&n:从x(t)\to y(t)的单向路径条数
\\\\
&\Delta=1-\sum L_a+\sum L_bL_c -\sum L_dL_eL_f+\cdots
\\\\
&\sum L_a:所有单独回路增益之和; \quad \sum L_bL_c:两个互不接触的回路增益乘积之和
\\\\
&\sum L_dL_eL_f:三个互不接触的回路增益乘积之和
\\\\
&p_k:第k条从x(t)\to y(t)的单向路径的总增益
\\\\
&\Delta_k=\Delta-(\Delta中与第k条通路有接触的部分)
\end{align*}
$$
<!--ID: 1669110682726-->


系统函数怎么转化为微分方程 #flashcard
- N(s):方程右侧，与输入相应
- D(s):方程左侧，与输出相应
$$
\begin{align*}
&H(s)=\frac{N(s)}{D(s)}
\end{align*}
$$
<!--ID: 1669110682730-->


信号周期性怎么判别 #flashcard
$f(t)=f(T+t)$或$f[n]=f[n+N]$
- 对于T，无特别要求。对于N，要求<font color=red>N是非零正整数</font>
<!--ID: 1669110682735-->


sa函数全时域积分 #flashcard
$$
\begin{align*}
&1.\int_{-\infty}^{+\infty}\frac{sin(\omega_ct)}{t}dt=\pi
\\\\
&2.\int_{-\infty}^{+\infty}\frac{sin^2(\omega_ct)}{t^2}dt=\pi\omega_c
\\\\
&3.\int_{-\infty}^{+\infty}\frac{sin^3(\omega_ct)}{t^3}dt=\frac{3}{4}\pi\omega_c^2
\\\\
&4.\int_{-\infty}^{+\infty}\frac{sin^4(\omega_ct)}{t^4}dt
=\frac{2}{3}\pi\omega_c^3
\end{align*}
$$
<!--ID: 1669111081946-->


方波信号傅里叶变换对 #flashcard
$$
\begin{align*}
&g_{\tau}(t)=
\begin{cases}
1, \quad
 & |t|<{\tau}
 \\
 \\
0, \quad
 & |t|>\tau
\end{cases}
\quad
\leftrightarrow
\quad
2 \frac{Sin(\omega \tau)}{\omega}
\\\\
&g(t)=k\frac{sin\ \omega_c t}{t}
\Rightarrow G(j\omega)=
\begin{cases}
{k\pi},&|\omega|<\omega_c
\\\\
0,&其他
\end{cases}
\end{align*}
$$
<!--ID: 1669111081950-->


内插公式 #flashcard
$$
x(t)=\sum_{l=-\infty}^{\infty}f(lT_{s})sa[\frac{\pi(t-lT_{s})}{T_{s}}]
$$
<!--ID: 1669111081955-->


罗斯-霍维茨准则 #flashcard
$$
\begin{align*}
&1.系统特征多项式:系统函数的分母部分D(s)或D(z),要求正幂次
\\
&2.对于拉斯变换D(s)=a_{n}s^{n}+a_{n-1}s^{n-1}+\cdots+a_0
\\
&3.写出罗斯-霍维茨阵列:
\begin{matrix}
a_n &a_{n-2}&a_{n-4} &\cdots \\
a_{n-1} &a_{n-3}&a_{n-5} &\cdots \\
-\frac{\begin{vmatrix}
a_n &a_{n-2}  \\
a_{n-1} & a_{n-3} \\
\end{vmatrix}}{a_{n-1}}
&-\frac{\begin{vmatrix}
a_n &a_{n-4}  \\
a_{n-1} & a_{n-5} \\
\end{vmatrix}}{a_{n-1}}
&\cdots
\\
\cdots&\cdots&\cdots
\end{matrix}
\\\\
&一共有n+1行,如果第一列元素不变号,则系统稳定
\\\\
&对于Z变换需要多一步,先进行双线性变换z=\frac{\lambda+1}{\lambda-1},剩余相同
\end{align*}
$$
如果第一列出现0,用ε代替该0,且$\varepsilon \to 0^{+}$
<!--ID: 1669111081959-->

Z变换性质 #flashcard
$$
\begin{align*}\\
&时移性质:f[n-n_{0}] \leftrightarrow z^{-n_0}F(z)\\\\
&z域尺度变换:z_{0}^{n}f[n] \leftrightarrow F(\frac{z}{z_{0}})\\\\
&时域反转特性:f[-n] \leftrightarrow F(\frac{1}{z})\\\\
&时域展宽特性:f_{1}[n]\leftrightarrow F(z^N)
\\\\&f_1[n]=
\begin{cases}
f[\frac{n}{N}],&n为N的整数倍\\
\\
0,&其他
\end{cases}\\
&
\\
&时域卷积特性:f[n]*h[n] \leftrightarrow F(z)H(z)
\\
\\
&时域差分:f[n]-f[n-1]\leftrightarrow (1-z^{-1})F(z)
\\
\\
&时域累加:\sum_{m=-\infty}^{n}f[m] \leftrightarrow 
\frac{1}{1-z^{-1}}F(z)
\\
\\
&z域微分性质:-nf[n] \leftrightarrow z\frac{dF(z)}{dz}
\\
\\
&初值定理:f[n_0]=\lim_{z \to \infty}[z^{n_0}F(z)],\quad f[n]=0,n<n_0
\\
\\
&终值定理:f[\infty]=\lim_{z \to 1}[(1-z^{-1})F(z)],
\quad (1-z^{-1})F(z)收敛域包含单位圆
\end{align*}
$$
<!--ID: 1669111173667-->

傅里叶变换性质 #flashcard
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
共轭对称性:(和FS完全一样)
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
<!--ID: 1669450825585-->




信号变换后最高频率 #flashcard
$$
\begin{align*}
&记信号x(t)和g(t)的最高频率分别为\omega_x,\omega_g
\\\\
&则x(at)的最高频率:\omega=a\omega_x
\\\\
&x(t)\cdot g(t)的最高频率:\omega=\omega_x+\omega_g
\\\\
&x(t)*g(t)的最高频率:\omega=min\{\omega_x,\omega_g\}
\end{align*}
$$
<!--ID: 1669111756145-->



傅里叶常用变换对 #flashcard

![[Pasted image 20221123144447.png]]
![[Pasted image 20221123144504.png]]
<!--ID: 1669190687542-->





拉斯变换的性质 #flashcard
$$
\begin{align*}
时移性质:f(t-t_{0})\quad \leftrightarrow & \quad e^{-st_{0}}F(s)
\\\\
频移性质:f(t)e^{s_{0}t}\quad \leftrightarrow &\quad F(s-s_{0})
\\\\
尺度变换:f(at) \quad \leftrightarrow & \quad \frac{1}{|a|}F(\frac{s}{a})
\\\\
时域卷积:f(t)*h(t) \quad \leftrightarrow &\quad F(s)H(s)
\\\\
时域微分:\frac{df(t)}{dt} \quad \leftrightarrow &\quad sF(s)	\quad 对于双边成立
\\\\
时域积分:\int_{-\infty}^{t}f(\tau)d\tau \quad \leftrightarrow &\quad \frac{1}{s}F(s)	
\\\\
s域微分:-tf(t) \quad \leftrightarrow &\quad \frac{dF(s)}{ds}
\\\\
初值定理:f(0^+)=\lim_{t \to 0^+}f(t)=&\lim_{s\to \infty}sF(s) \quad 0时刻无冲激
\\\\
终值定理:f(\infty)=\lim_{t \to \infty}f(t)=&\lim_{s \to 0}sF(s) \quad sF(s)收敛域包含虚轴
\end{align*}
$$
<!--ID: 1669111297489-->


$sin\omega_0 t\cdot u(t)$和$cos\omega_0t\cdot u(t)$的拉斯变换是什么？ #flashcard 
$$
\begin{align*}
cos{(\omega t)}\cdot u(t) \leftrightarrow \frac{s}{s^2+\omega^2}
\\\\
sin{(\omega t)}\cdot u(t) \leftrightarrow \frac{\omega}{s^2+\omega^2}
\end{align*}
$$
<!--ID: 1669189910472-->



梅森公式中回路就是闭合的框吗？  #flashcard
不是，闭合框中箭头指向一致才是一个回路
<!--ID: 1669189910478-->



幅频特性要怎么计算？ #flashcard 
得到系统函数后，求其模值，复指数使用欧拉公式化简
<!--ID: 1669189910484-->


周期信号怎么求解其傅里叶变换？ #flashcard 
==记住有2Π==
$$
周期信号:f(t)=\sum_{k=-\infty}^{+\infty}a_{k}e^{jk\omega_{0}t}
\  \leftrightarrow  \ 
2\pi\sum_{k=-\infty}^{+\infty}a_{k}\delta(\omega-k\omega_{0})
$$
<!--ID: 1669194027520-->


要想采样出一个信号点，需要怎么做？ #flashcard 
乘上对应冲激之后积分
$$
f(t_0)=\int_{-\infty}^{+\infty}f(t)\delta(t-t_0)dt
$$
<!--ID: 1669194027527-->


帕斯瓦尔定理的证明 #flashcard 
1.用f(t)=f*(t),在使用傅里叶变换表示f*(t)
2.转换为傅里叶变换的定义，求$f^2(t)$的傅里叶变换，频域卷积性质
<!--ID: 1669194027531-->


怎么求解系统函数的模$|H(e^{j\Omega})|$   #flashcard
分子的模/分母的模
<!--ID: 1669280950112-->



对于LTI系统，输出之间的线性微积分关系与什么相同？ #flashcard 
输入之间的线性微积分关系
<!--ID: 1669280925867-->



傅里叶尺度变换性质 #flashcard 
$$
f(at)\leftrightarrow \frac{1}{|a|}F(\frac{j\omega}{a})
$$
<!--ID: 1669280925876-->


周期信号都可以表出为什么形式 #flashcard 
周期性冲激串与非周期信号的卷积
<!--ID: 1669280925883-->


z域尺度变换公式 #flashcard 
$$
z_{0}^{n}f[n] \leftrightarrow F(\frac{z}{z_{0}})
$$
<!--ID: 1669280925888-->


两个方波进行卷积怎么处理？ #flashcard 
将其中一个求导为冲激，和另一个信号卷积之后再积分回来。
<!--ID: 1669280925893-->

补偿滤波器无法补偿零点信息？ #flashcard 
是的，小心
<!--ID: 1669290778004-->


实信号的拉斯变换零极点有什么特点  #flashcard
共轭对称$F(s)=F^*(s^*)$
<!--ID: 1669517119078-->



如下的周期冲激串的傅里叶变换
$$
\begin{align*}
f(t)=\sum_{k=-\infty}^{+\infty}(-1)^{k}\delta(t-kT)
\end{align*}
$$
#flashcard
$$
\begin{align*}
&a_k=\frac{1}{T}\int_{T}f(t)e^{-j\omega t}dt=\frac{1}{T}\{1-(-1)^k\}
\\\\
&f(t)=\sum_{k=-\infty}^{+\infty}a_ke^{j\omega t} 
\\\\
&F(j\omega)=\frac{2\pi}{T}\sum_{k=-\infty}^{+\infty}\{1-(-1)^k\}\delta(\omega-k\frac{2\pi}{T})
\end{align*}
$$
<!--ID: 1669517119082-->




双边拉斯变换/z变换的条件使用条件  #flashcard
因果信号/无初始条件
<!--ID: 1669621931269-->



已知X(z)=1,f[n]=?  #flashcard
δ[n]
<!--ID: 1669621931273-->



实奇函数的拉斯变换零极点有什么特点？  #flashcard
一定有零点s=0，零极点不仅共轭对称而且还偶对称
<!--ID: 1669621931278-->



已知$x(t)*h(t)=y(t)$则，$x(at)*h(at)$等于？  #flashcard
$x(at)*h(at)=\frac{1}{|a|}y(at)$
<!--ID: 1669627986806-->


如果系统的输入信号有阶跃怎么处理  #flashcard
利用卷积的微积分性质将其转为冲激信号
<!--ID: 1670057624230-->



$y''(t)$与$y'(t)$的单边拉普拉斯变换  #flashcard
$$
\begin{align*}
&y''(t)\leftrightarrow s^2Y(s)-sy(0^-)-y'(0^-)
\\\\
&y'(t)\leftrightarrow sY(s)-y(0^-)
\end{align*}
$$
<!--ID: 1670057624235-->


在作图题中，由两个输入之间关系，得到输出之间关系时要注意什么？  #flashcard
映射关系只能有“==权重叠加==”、“==时移==”;<font color=red>不能有伸缩</font>
<!--ID: 1670057624241-->



由于写作负幂次信号，则画离散系统的零极图的时候需要注意什么？  #flashcard
不要漏掉z=0这个零点
<!--ID: 1670057624246-->


怎么求解相频特性表达式  #flashcard
分子相频表达式-分母表达式
<font color=red>注意，分子分母的表达式都要由ω所决定的象限确定</font>
<!--ID: 1670057624251-->



频域梯形变换对  #flashcard
$$
\begin{align*}
&f(t)=k\frac{sin(\omega_1 t)sin(\omega_2 t)}{t^2} \qquad 其中:\omega_1>\omega_2
\\\\
&F(j\omega)=
\begin{cases}
k\pi \omega_2 &|\omega|\le \omega_1-\omega_2
\\\\
-\frac{k\pi}{2}|\omega|+\frac{k\pi (\omega_1+\omega_2)}{2} &\omega_1-\omega_2<|\omega|<\omega_1+\omega_2
\\\\
0&其他
\end{cases}
\end{align*}
$$
<!--ID: 1670410671402-->


对有跳跃的信号求导数，需注意什么  #flashcard
导数信号有冲激
<!--ID: 1670730365423-->



求采样周期范围需要注意什么？  #flashcard
记得写上单位s
<!--ID: 1670730365426-->


正弦信号通过的频域分析口诀  #flashcard
幅度乘幅度、相角加相角
<!--ID: 1670751361256-->


$\frac{1}{1-z^{-1}}\quad |z|<1$的时域表达式  #flashcard
$-u[-n-1]$
<!--ID: 1670751361265-->


如果系统的t时刻的输出只与系统t时刻之后的输入有关系，那么这个系统有无记忆？ #flashcard
有记忆性
仅当系统的t时刻的输出只与t时刻的输入有关时，系统才是无记忆系统
<!--ID: 1671249238515-->



$\delta(\omega-\omega_0)+\delta(\omega+\omega_0)$的时域表达式 #flashcard
$\frac{1}{\pi}cos\omega_0 t$
<!--ID: 1671249238520-->



由多个子系统构成的系统中，如果整体系统的频率响应不好求怎么处理？ #flashcard
可以分成几个部分分析系统是如何影响输出的
<!--ID: 1671249238525-->



$\frac{1}{({1-az^{-1}})^2} \quad |z|>a$的时域表达式 #flashcard
$(n+1)a^{n}u[n]$
<!--ID: 1671249238530-->


劳斯-赫尔维茨定理使用的前提 #flashcard
特征多项式的各个幂次系数都大于0
<!--ID: 1671450042490-->




---



怎么得到正确的F(jω)
![[Pasted image 20221123145606.png]] #flashcard 

![[Pasted image 20221123145647.png]]
<!--ID: 1669186620589-->



![[Pasted image 20221123150140.png]] 
#flashcard 
![[Pasted image 20221123150215.png]]
<!--ID: 1669189910492-->



想好怎么处理$e^{-j\omega t_0}$
![[Pasted image 20221123152331.png]]
#flashcard 
![[Pasted image 20221123152436.png]]
<!--ID: 1669189910498-->



想好怎么使用梅森公式，怎么求解幅频特性
![[Pasted image 20221123154914.png]]
#flashcard
![[Pasted image 20221123155141.png]]
<!--ID: 1669189910504-->

怎么转换这个绝对和的条件
![[Pasted image 20221128155250.png]]
#flashcard 
D
<!--ID: 1669885622460-->



怎么求一个系统的H(jω)
![[Pasted image 20221126165148.png]]
#flashcard
<!--ID: 1669517119087-->








![[Pasted image 20221128155424.png]] #flashcard 
![[Pasted image 20221128155447.png]]
<!--ID: 1669622200185-->



如下信号的图像如何画？
![[Pasted image 20221128155541.png]]
#flashcard 
![[Pasted image 20221128155612.png]]
<!--ID: 1669622200189-->


![[Pasted image 20221128173359.png]]
#flashcard 
$$
\begin{align*}
x_1[0]=&\frac{1}{2}就是X_1(z)常数项的系数为\frac{1}{2}\Rightarrow L_1=\frac{1}{2}
\\\\
X_1(z)=&L_1\frac{z^2-\frac{3}{4}\sqrt{2}z+\frac{9}{16}}
{z^2+\frac{3}{4}\sqrt{2}z+\frac{9}{16}}
=L_1\frac{1-\frac{3}{4}\sqrt{2}z^{-1}+\frac{9}{16}z^{-2}}
{1+\frac{3}{4}\sqrt{2}z^{-1}+\frac{9}{16}z^{-2}}
\\\\
=&L_1
\begin{pmatrix}
1-\frac{\frac{3}{2}\sqrt{2}z^{-1}}{{1+\frac{3}{4}\sqrt{2}z^{-1}+\frac{9}{16}z^{-2}}}
\end{pmatrix}
=L_1
\begin{pmatrix}
1-4\cdot \frac{\frac{\sqrt{2}}{2}(\frac{3}{4}z^{-1})}{{1+\sqrt{2}(\frac{3}{4}z^{-1})+(\frac{3}{4}z^{-1})^{2}}}
\end{pmatrix}
\\\\
\Rightarrow x_1[n]=&L_1
\begin{Bmatrix}
\delta[n]-4\cdot (\frac{3}{4})^nsin(\frac{3}{4}\pi n)u[n]
\end{Bmatrix}
\\\\
同理:x_2[n]=&L_2
\begin{Bmatrix}
\delta[n]+4\cdot (\frac{1}{2})^nsin(\frac{1}{4}\pi n)u[n]
\end{Bmatrix}
\\\\
x_3[n]=&\frac{x_2[n]}{x_1[n]}=\frac{L_2}{L_1}(-\frac{2}{3})^nu[n]
\\\\
\sum_{n=-\infty}^{+\infty}|x_3[n]|=&\sum_{n=0}^{+\infty}
\begin{vmatrix}
\frac{L_2}{L_1}
\end{vmatrix}
(\frac{2}{3})^n=6 \Rightarrow \begin{vmatrix}
\frac{L_2}{L_1}
\end{vmatrix}=2
\\\\
\Rightarrow |L_2|=&1
\end{align*}
$$
<!--ID: 1669628090815-->


![[Pasted image 20221130160125.png]]
#flashcard 
![[Pasted image 20221130160203.png]]
<!--ID: 1669812941281-->



![[Pasted image 20221206170346.png|500]]
#flashcard 
![[Pasted image 20221206170447.png]]
<!--ID: 1670410671408-->



![[Pasted image 20221209195445.png]]
#flashcard 
![[Pasted image 20221209195518.png]]
<!--ID: 1670730365431-->



![[Pasted image 20221211165706.png]]
#flashcard 
![[Pasted image 20221211165729.png]]
<!--ID: 1670751361269-->




![[Pasted image 20221214172118.png]]
#flashcard 
![[Pasted image 20221214172214.png]]
<!--ID: 1671249238536-->



![[Pasted image 20221219184455.png]]
#flashcard 
![[Pasted image 20221219184533.png]]
<!--ID: 1671450042493-->





![[Pasted image 20221219184559.png]]
#flashcard 
![[Pasted image 20221219184632.png]]
<!--ID: 1671450042497-->




