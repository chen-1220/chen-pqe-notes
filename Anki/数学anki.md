
TARGET DECK
数学

余子式M，代数余子式A，行列式之间关系 #flashcard 
$$
\begin{align*}
&其中A_{ij}是代数余子式，M_{ij}是余子式，A_{ij}=(-1)^{i+j}M_{ij}
\\\\
&|A|=a_{i1}A_{i1}+a_{i2}A_{i2}+...+a_{in}A_{in}
\\\\
&|A|=a_{1j}A_{1j}+a_{2j}A_{2j}+...+a_{nj}A_{nj}
\end{align*}
$$
<!--ID: 1669125321989-->




在求解函数时，需注意什么 #flashcard 
补充无定义点，写清楚定义域
<!--ID: 1669125321996-->



协方差和相关系数的公式 #flashcard 
$$
\begin{align*}
&Cov(X,Y)=E[(X-EX)(Y-EY)]
\\\\
&公式法:Cov(X,Y)=E(XY)-EX\cdot EY
\\\\
&\rho_{XY}=\frac{Cov(X,Y)}{\sqrt{DX}\cdot \sqrt{DY}}
\begin{cases}
=0 \Leftrightarrow X,Y不线性相关
\\\\
\ne 0 \Leftrightarrow X,Y线性相关
\end{cases}
\end{align*}
$$
<!--ID: 1669125322002-->


洛必达使用需要注意什么 #flashcard 
1.是否函数的导数存在
2.求导的时候认真看清楚，别求错了
<!--ID: 1669125322008-->


遇到不同类型的函数该怎么处理 #flashcard 
分类分类分类！！！
<!--ID: 1669125322015-->


在被积函数无法找到原函数时怎么处理 #flashcard 
1.考虑分部积分！！！！！
2.二重积分交换积分次序
3.无穷级数展开
4.夹逼定理
<!--ID: 1669125322022-->




涉及二阶导数及以上导数时，怎么处理函数？ #flashcard 
泰勒展开
$$
f(x)=\sum_{n=0}^{\infty}\frac{f^{(n)}(x_0)}{n!}(x-x_0)^n
$$
<!--ID: 1669166461306-->




取特殊值或特殊函数需要注意什么？ #flashcard
满足题目所有条件
<!--ID: 1669125322029-->



空间向量之间的位置怎么分析？ #flashcard
转换为非齐次方程组分析
线性无关解个数：n-r(A)+1
$$
\begin{align*}
\newcommand{\overline}{\overset{\mathbf{\_\_}}}
&\begin{cases}
有解r(A)=r(\overline A)
\begin{cases}
r(A)=r(\overline A)=n &唯一解
\\\\
r(A)=r(\overline A)<n &无穷解
\end{cases}
\\\\
无解r(A)+1= r(\overline A)
\end{cases}
\end{align*}
$$
<!--ID: 1669125322036-->



侧面积公式是什么？ #flashcard
绕x轴旋转
$$
\begin{align*}
S_{侧}=
\begin{cases}
2\pi\int_{a}^{b}y\cdot \sqrt{1+y'^2}\ dx
\\\\
2\pi\int_{a}^{b}y(t)\cdot \sqrt{x'(t)^2+y'(t)^2}\ dt
\\\\
2\pi\int_{a}^{b}rsin\ \theta\cdot \sqrt{r^2+r'^2}\ d\theta
\end{cases}
\end{align*}
$$
绕y轴旋转
$$
\begin{align*}
S_{侧}=
\begin{cases}
2\pi\int_{a}^{b}x\cdot \sqrt{1+y'^2}\ dx
\\\\
2\pi\int_{a}^{b}x(t)\cdot \sqrt{x'(t)^2+y'(t)^2}\ dt
\\\\
2\pi\int_{a}^{b}rcos\ \theta\cdot \sqrt{r^2+r'^2}\ d\theta
\end{cases}
\end{align*}
$$
<!--ID: 1669166461311-->



正交矩阵有什么特点 #flashcard
1.|A|=1或-1
2.列向量单位正交
3.$A^T=A^{-1}$
<!--ID: 1669125322042-->



要永远相信什么？ #flashcard
第二问救赎之道就在第一问
<!--ID: 1669125322049-->


已知概率分布求解概率密度需要注意什么？ #flashcard
概率分布函数求导注意复合
<!--ID: 1669125322054-->


分布函数可以和什么紧密联系 #flashcard
事件概率
<!--ID: 1669125322058-->



数列的是否敛散和什么等价？ #flashcard
数列极限是否存在
<!--ID: 1669125322063-->


数列极限的定义是什么？ #flashcard
$$
\begin{align*}
\lim_{n \to \infty}x_n=A \Leftrightarrow \forall \varepsilon>0,\exists  
N>0,当n>N时，有|x_n-A|<\varepsilon
\end{align*}
$$
<!--ID: 1669125322068-->



第二型曲线积分的对称性以及轮换对称性有什么需要注意的？ #flashcard
轮换对称性
$$
\begin{align*}
&如果被积曲线关于y=x对称\Leftrightarrow 交换x,y后曲线方程不变
\\\\
&\Rightarrow \int_{L}f(x,y)dx+f(y,x)dy=0
\end{align*}
$$
普通对称性
$$
\begin{align*}
&1.L关于y轴对称:L_1为L在右半平面的部分
\\\\
&\int_{L}P(x,y)dx=
\begin{cases}
0 &P(x,y)是关于x的奇函数
\\\\
2\int_{L_1}P(x,y)dx &P(x,y)是关于x的偶函数
\end{cases}
\\\\\\
&\int_{L}Q(x,y)dy=
\begin{cases}
2\int_{L_1}Q(x,y)dy &Q(x,y)是关于x的奇函数
\\\\
0 &Q(x,y)是关于x的偶函数
\end{cases}
\\\\\\
&2.L关于x轴对称:L_1为L在上半平面的部分
\\\\
&\int_{L}P(x,y)dx=
\begin{cases}
2\int_{L_1}P(x,y)dx &P(x,y)是关于y的奇函数
\\\\
0 &P(x,y)是关于y的偶函数
\end{cases}
\\\\\\
&\int_{L}Q(x,y)dy=
\begin{cases}
0 &Q(x,y)是关于y的奇函数
\\\\
2\int_{L_1}Q(x,y)dy  &Q(x,y)是关于y的偶函数
\end{cases}
\end{align*}
$$
<!--ID: 1669125322075-->




定积分与二重积分定义公式记得吗？ #flashcard
$$
\begin{align*}
&\lim_{n \to \infty}\sum_{i=1}^{n}f(0+\frac{1-0}{n}i)\frac{1-0}{n}=\int_{0}^{1}f(x)dx
\\\\
&\lim_{n \to \infty}\sum_{i=0}^{n-1}f(0+\frac{1-0}{n}i)\frac{1-0}{n}=\int_{0}^{1}f(x)dx
\end{align*}
$$
$$
\begin{align*}
&\iint_{D}f(x,y)d\sigma=\displaystyle \lim_{n \to \infty}\sum_{i=1}^{n}\sum_{j=1}^{n}f(a+\frac{b-a}{n}i,c+\frac{d-c}{n}j)·\frac{b-a}{n}·\frac{d-c}{n}
\\
\\
&D是长方形区域[a,b]\times[c,d]
\end{align*}
$$
<!--ID: 1669125322082-->


开始积分之前需要考虑什么？ #flashcard 
对称性
<!--ID: 1669125322088-->


减法公式是什么？ #flashcard
$$
\newcommand{\overline}{\overset{\mathbf{\_\_}}}
P(A \overline B)=P(A-B)=P(A)-P(AB)
$$
<!--ID: 1669125322092-->


关于拉格朗日数乘法，需要考虑什么？ #flashcard
怎么可以较好的运用约束方程
有时候并不需要解出具体值
<!--ID: 1669125322097-->


第二型曲面积分需要注意什么？ #flashcard
1.不满足一阶偏导连续时，使用投影法
2.投影有正负之分
3.注意高斯公式是否可以满足，补面或者去点
<!--ID: 1669125322102-->



级数的和函数和级数一定等价意味着什么？ #flashcard
级数系数未知时，可以使用待定系数法
<!--ID: 1669125322106-->


已知矩阵A，怎么将其相似对角化？ #flashcard
写出特征多项式⇒得到特征值⇒求解特征方程组⇒特征向量
<!--ID: 1669125322110-->



据估计当分布的期望为0时怎么办？ #flashcard
考虑二阶矩相等
$$
样本k阶原点矩:A_k=\frac{1}{n}\sum_{i=1}^{n}X_i^k(k=1,2,\cdots)
$$
<!--ID: 1669125322115-->


渐近线有几种怎么求解的？ #flashcard
极坐标下要先转换为直角坐标或参数方程$x=r(\theta)cos\theta;\quad y=r(\theta)sin\theta$
$$
\begin{align*}
&1.铅垂渐近线:x_0来源: ➊ 无定义点 \quad ➋区间端点
\\\\
&若\lim_{x\to x_0^+}f(x)=\infty(或\lim_{x\to x_0^-}f(x)=\infty) \Rightarrow x=x_0为铅垂渐近线
\\\\
&2.水平渐近线:来源: \pm \infty处
\\\\
&若\lim_{x\to +\infty}f(x)=y_1  \Rightarrow y=y_1为水平渐近线
\\
&若\lim_{x\to -\infty}f(x)=y_2  \Rightarrow y=y_2为水平渐近线
\\\\
&3.斜渐近线:来源: \pm \infty处(已经有水平渐近线的方向一定没斜渐近线)
\\\\
&若\lim_{x\to +\infty}\frac{f(x)}{x}=k_1,\lim_{x\to +\infty}[f(x)-k_1x]=b_1  \Rightarrow y=k_1x+b_1为斜渐近线
\\
&若\lim_{x\to -\infty}\frac{f(x)}{x}=k_2,\lim_{x\to -\infty}[f(x)-k_2x]=b_2 \Rightarrow y=k_2x+b_2为斜渐近线
\end{align*}
$$
<!--ID: 1669166936738-->



傅里叶级数？ #flashcard 
$$
\begin{align*}
&f(x)=\frac{a_0}{2}+\sum_{n=1}^{\infty}(a_ncos\frac{n \pi x}{l}+b_nsin\frac{n \pi x}{l})
\\
\\
&其中：a_0=\frac{1}{l}\int_{-l}^{l}f(x)dx \qquad a_n=\frac{1}{l}\int_{-l}^{l}f(x)cos\frac{n \pi x}{l}dx
\\
\\
&b_n=\frac{1}{l}\int_{-l}^{l}f(x)sin\frac{n \pi x}{l}dx
\end{align*}
$$
<!--ID: 1669166936744-->




非齐次方程组线性无关解个数 #flashcard
n-r(A)+1
<!--ID: 1669166936747-->



A伴随矩阵的某一项不为0的项有什么意义 #flashcard
决定A中列向量谁线性无关
<!--ID: 1669166936751-->




正定二次型的定义 #flashcard 
$$
\begin{align*}
&1.特征值\lambda全>0
\\
&2.正惯性指数p=n
\\
&3.顺序主子式全>0
\\
&4.A\simeq E:A=C^TEC其中C可逆
\\
&5.x\ne 0 \Rightarrow 二次型f>0
\end{align*}
$$
<!--ID: 1669166936755-->



数字特征和独立怎么判断 #flashcard 
数字特征判别相关，分布判定独立
<!--ID: 1669166936759-->



怎么去除绝对值 #flashcard 
通过划分区域
<!--ID: 1669166936764-->


二维正态分布 #flashcard 
$$
\begin{align*}
& (X,Y)\sim N(\mu_1,\mu_2;\sigma_1^2,\sigma_2^2;\rho) \quad 注意顺序
\\\\
&\large f(x,y)=\frac{1}{2\pi \sigma_1\sigma_2\sqrt{1-\rho^2}}
e^{-\frac{1}{2(1-\rho^2)}[(\frac{x-\mu_1}{\sigma_1})^2-2\rho\frac{(x-\mu_1)(y-\mu_2)}{\sigma_1\sigma_2}+(\frac{y-\mu_2}{\sigma_2})^2]}
\end{align*}
$$
<!--ID: 1669166936768-->


二阶可降阶微分方程怎么处理 #flashcard 
- 缺y形
$$
形如:y''=f(x,y')
\\ 
令y'=z,y''=z'即可
$$
- 缺x形 $$
形如:y''=f(y,y')
\\ 
令y'=z,y''=zz'即可
$$
<!--ID: 1669168770462-->






级数和函数收敛域出现未定义点 #flashcard 
补充定义
<!--ID: 1669166936777-->




证明极限存在 #flashcard
1.单调有界
2.极限定义
3.夹逼定理+放缩
<!--ID: 1669166936782-->


斯托克斯公式怎么选取转哪一种曲面积分？ #flashcard
对于平面⇒第一型曲面积分，对于曲面⇒第二型曲面积分 
<!--ID: 1669166936786-->


极坐标不好处理，又难以转换为直角坐标时怎么办？ #flashcard
转换为参数方程
<!--ID: 1669168590832-->


第一型曲面积分和第二型曲面积分的共同特点是什么？ #flashcard
投影不能重叠
<!--ID: 1669168590836-->


求导可分为哪两类？ #flashcard
1.公式法
2.具体点的定义法
<!--ID: 1669168590841-->



级数收敛的必要条件 #flashcard
$$\lim_{n\to \infty}u_n=0$$
<!--ID: 1669168590845-->


级数收敛的判断方法有哪些 #flashcard
1.前n项和单调增加有上界
2.比值，根值，比较
3.交错级数莱布尼茨
<!--ID: 1669168590849-->


偏微分方程怎么处理？ #flashcard
对于一阶偏微分方程可以直接偏积分，二阶需要转为一元处理
<!--ID: 1669168590853-->


实对称矩阵不同特征值对应的特征向量有什么关系？ #flashcard
一定正交
<!--ID: 1669169756581-->



转动惯量的公式记得吗？ #flashcard
需要乘密度函数
$$
\begin{align*}
&I_{x}=\iint_{D}y^2\rho(x,y)d\sigma \qquad I_{y}=\iint_{D}x^2\rho(x,y)d\sigma
\\
&I_{o}=\iint_{D}(x^2+y^2)\rho(x,y)d\sigma
\end{align*}
$$
<!--ID: 1669169756585-->


矩阵的迹怎么求？ #flashcard
特征值之和
<!--ID: 1669169756589-->


最大似然估计怎么求解 #flashcard 
取观测值⇒求概率乘积或概率密度乘积⇒取对数⇒求驻点
<!--ID: 1669169756593-->



无穷级数与微分方程怎么联系？ #flashcard 
1.微分方程的解是无穷级数的和函数
2.无穷级数构建微分方程
<!--ID: 1669169756596-->


点到平面的距离公式？ #flashcard 
$$
d=\frac{|Ax_0+By_0+Cz_0+D|}{\sqrt{A^2+B^2+C^2}}
$$
矩阵相似的性质 #flashcard 
矩阵相似⇔特征值相同且都可以相似对角阵
$$
\begin{align*}
&1.|A|=|B|
\\\\
&2.r(A)=r(B)
\\\\
&3.|\lambda E-A|=|\lambda E-B| \Rightarrow特征值相同
\\\\
&4.\sum a_{ii}=\sum b_{ii}
\\\\
&5.A+kE\sim B+kE 
\\\\
&6.相似的传递性:A\sim \Lambda,B\sim \Lambda \Rightarrow A\sim B 
\\\\
&7.A^n\sim B^n,借助对角阵可解决n阶矩阵问题
\\\\
&8.A\sim B \Rightarrow A,B具有相同的特征值
\end{align*}
$$
<!--ID: 1669169756601-->



有哪些方式可以将$A_{ij}$与$a_{ij}$联系起来？ #flashcard 
展开式or$A^*A=|A|E$
<!--ID: 1669169756605-->


随机样本独立同分布于哪一种分布时，样本方差和样本均值独立？ #flashcard 
正态分布
<!--ID: 1669169756608-->



如果随机变量$X_i^2$的均值依概率收敛于$E(X^2)$
样本方差S依概率收敛于方差σ


物体沿某温度场上升速度最快方向移动意味着什么？ #flashcard 
物体沿其梯度方向前进
<!--ID: 1669177554718-->




格林-斯托克斯-高斯的使用均有什么条件？ #flashcard 
一阶连续偏导的条件！！！
<!--ID: 1669177554726-->


飞机追踪如何列方程 #flashcard 
斜率+弧长列方程
<!--ID: 1669177554732-->



置信区间的定义 #flashcard 
参数落在置信区间的概率=置信度
<!--ID: 1669177554739-->



提取物体做功的公式，以及要求是什么？ #flashcard 
以水面为坐标起点，向下为x轴正方向
$$
W=\rho g\int_{a}^{b}xA(x)dx \quad \rho为物体密度\quad g为重力加速度
$$
<!--ID: 1669177554747-->




静水压力的公式，以及要求是什么？ #flashcard 
以水面为坐标起点，向下为x轴正方向
$$
P=\rho g\int_{a}^{b}x[f(x)-h(x)]dx
$$
<!--ID: 1669177554752-->


如果积分区间两端，被积函数都发散怎么处理  #flashcard 
将积分区间划分为两段，务必保证只有单边发散
<!--ID: 1669207139234-->


怎么判断无穷积分是否收敛 #flashcard 
利用比较判别法转换为已知的几种无穷积分
<!--ID: 1669207139244-->


有哪些无穷积分的敛散性是已知的 #flashcard 
$$
\begin{align*}
&\int_{a}^{b}\frac{1}{(x-a)^q}dx\quad (a<b)
\begin{cases}
q<1,&收敛
\\\\
q\ge1,&发散
\end{cases}
\\\\
&\int_{a}^{+\infty}\frac{1}{x^p}dx\quad (a>0)
\begin{cases}
p>1,&收敛
\\\\
p\le1,&发散
\end{cases}
\end{align*}
$$
<!--ID: 1669207139252-->


$AB=E_n$意味着什么？ #flashcard
$$
n=r(AB)\le min\{r(A)+r(B)\}
$$
<!--ID: 1669207139258-->



关于$AA^{T}=E$举出一个特例 #flashcard
$$
\begin{align*}
&AA^{T}=E
\\\\
&取A=
\begin{bmatrix}
1 &0  &0  \\
0 &  1& 0 \\
\end{bmatrix}
\qquad
A^T=
\begin{bmatrix}
1 &0 \\
0 &1\\
0&0\\
\end{bmatrix}
\end{align*}
$$
<!--ID: 1669207275603-->

傅里叶级数的题目一定要由公式求解出$a_n$与$b_n$吗？  #flashcard 
不一定，左右式的恒等
<!--ID: 1669263279917-->



函数的傅里叶级数展开值一定和原函数点相等吗? #flashcard 
连续点处是的，但是间断点是左右极限和的一半
<!--ID: 1669263279923-->



“实对称矩阵”和“A有3个相互正交的特征向量”之间是什么关系？ #flashcard
充分必要
<!--ID: 1669263279928-->


切比雪夫不等式是什么 #flashcard
$$
\begin{align*}
P\{|X-EX|\ge \varepsilon\}\le \frac{DX}{\varepsilon^2}
\end{align*}
$$
<!--ID: 1669263279932-->


二阶常系数微分方程的通解形式  #flashcard
$$
\begin{align*}
单根:y_n=&C_{1}e^{\lambda_{1}x}+C_{2}e^{\lambda_{2}x}
\\
\\
重根:y_n=&(C_{1}+C_{2}x)e^{\lambda x}
\\
\\
复数根(\lambda=\alpha \pm \beta j);y=&e^{\alpha x}{(C_{1}cos\beta x+C_{2}sin\beta x)}
\end{align*}
$$
<!--ID: 1669263279936-->

二阶常系数微分方程的特解形式  #flashcard
$$
\begin{align*}
1.f(x)=&e^{\alpha x}P_{n}(x)时  
\\\\
设为:y_p=&e^{\alpha x}Q_{n}(x)x^k \quad 
k=
\begin{cases}
0 &\alpha\ne \lambda_1,\alpha\ne \lambda_2
\\\\
1 &\alpha=\lambda_1或\alpha=\lambda_2
\\\\
2 &\alpha=\lambda_1=\lambda_2
\end{cases}
\\
\\
2.f(x)=&e^{\alpha x}[P_{m}(x)cos{\beta x}+P_{n}(x)sin{\beta x}]时
\\\\
设为:y_p=&e^{\alpha x}[Q_{l}^{(1)}(x)cos{\beta x}+Q_{l}^{(2)}(x)sin{\beta x}]x^k \quad 
k=
\begin{cases}
0 &\alpha\ne \lambda
\\\\
1 &\alpha=\lambda
\end{cases}
\end{align*}
$$
<!--ID: 1669342979116-->



四阶常系数微分方程的重复数根通解形式 #flashcard 
$$
y=e^{\alpha x}{[(C_{1}+C_{2}x)cos\beta x+(C_{3}+C_{4}x)sin\beta x]}
$$
<!--ID: 1669263279940-->


随机变量和差的方差公式  #flashcard 
$$
D(X\pm Y)=DX+DY\pm2Cov(X,Y)
$$
<!--ID: 1669263279944-->


可微条件下方向导数的计算公式  #flashcard 
$$
\begin{align*}
\frac{\partial u}{\partial \overrightarrow l}=u_x'cos\alpha+u_y'cos\beta+u_z'cos\gamma
\end{align*}
$$
<!--ID: 1669263279949-->


已知$P_0(x_0,y_0)$指向$P_1(x_1,y_1)$的方向导数为a，怎么表出？ #flashcard 
$$
\begin{align*}
u_x(x_0,y_0)\cdot \frac{x_1-x_0}{\sqrt{(x_1-x_0)^2+(y_1-y_0)^2}}+u_x(x_0,y_0)\cdot \frac{y_1-y_0}{\sqrt{(x_1-x_0)^2+(y_1-y_0)^2}}=a
\end{align*}
$$
<!--ID: 1669263279953-->


矩阵秩的性质有哪些？ #flashcard 
$$
\begin{align*}
&\color {red}4.r(A+B)\leq r(A)+r(B)
\\\\
&\color {red}5.r(AB)\leq min(r(A),r(B))
\\\\
&A,B为n阶矩阵\quad r(AB)\ge r(A)+r(B)-n
\\\\
&\color {red}6.A可逆，则r(AB)=r(B),r(BA)=r(B)
\\\\
&\color {red}7.若A_{m×n},B_{n×s}且AB=0\Rightarrow r(A)+r(B)\leq n
\end{align*}
$$
<!--ID: 1669517119070-->





八大分布的期望与方差公式  #flashcard 
$$
\begin{align*}
\begin{array}{c|c|c}
\hline
\\
分布 & 期望EX &方差DX
\\
\hline
0-1分布&p &p(1-p)
\\\hline
X\sim B(n,p)&np&np(1-p)
\\\hline
X\sim P(\lambda)&\lambda&\lambda
\\\hline
X\sim G(p)&\frac{1}{p}&\frac{1-p}{p^2}
\\\hline
X\sim U(a,b) &\frac{a+b}{2} &\frac{(b-a)^2}{12}
\\\hline
X\sim E(\lambda)&\frac{1}{\lambda}&\frac{1}{\lambda^2}
\\\hline
X\sim N(\mu,\sigma^2)&\mu&\sigma^2
\\\hline
X\sim \chi^2(n)&n&2n
\\\hline
\end{array}
\end{align*}
$$
<!--ID: 1669273396951-->




转置矩阵和原矩阵秩的联系 #flashcard 
$$
A-n阶矩阵:\color {red}r(A^{*})=
\begin{cases}
n,&r(A)=n
\\
1,&r(A)=n-1
\\
0,&r(A)<n-1
\end{cases}
$$
<!--ID: 1669273396958-->



二阶矩阵的逆矩阵怎么求解 #flashcard 
$$
\begin{align*}
&A=\begin{bmatrix}
a &b\\
c &d\\
\end{bmatrix}
&
A^{-1}=\frac{1}{|A|}\begin{bmatrix}
d &-b\\
-c &a\\
\end{bmatrix}
\end{align*}
$$
<!--ID: 1669273396962-->


平面第二型曲线积分有哪些解题思路？ #flashcard 
直接代换、格林公式、对称性
闭合曲线优先格林公式
<!--ID: 1669290777994-->



格林公式的使用需要注意什么？ #flashcard 
是否满足一阶偏导连续
是否是曲线正方向
曲线所围住空间是否含无定义点
<!--ID: 1669290778000-->


如果矩阵A可以相似对角化，则其特征值与秩的关系是什么？ #flashcard 
r(A)=非零特征值个数
<!--ID: 1669291930936-->



实对称矩阵的非零特征值个数等于其秩，对吗？ #flashcard 
是的！！！
<!--ID: 1669291930942-->


方程组基础解系的解向量个数和秩之间的关系？ #flashcard 
解向量个数=n-r(A)
<!--ID: 1669291930946-->


 反函数导数公式？ #flashcard 
 $$
x'=\frac{1}{y'}  \qquad x''=-\frac{y''}{(y')^3}
$$
<!--ID: 1669342979123-->


曲率公式与曲率半径？   #flashcard 
$$
\begin{align*}
&k=\frac{|y''|}{(1+y'^2)^{\frac{3}{2}}}
&R=\frac{1}{k}
\end{align*}
$$
<!--ID: 1669344808122-->




二元函数的导数定义  #flashcard 
$$
\begin{align*}
&f_{x}'(x_0,y_0)=\lim_{x\to x_0}\frac{f(x,y_0)-f(x_0,y_0)}{x-x_0}
\\\\
&f_{y}'(x_0,y_0)=\lim_{x\to x_0}\frac{f(x_0,y)-f(x_0,y_0)}{y-y_0}
\end{align*}
$$
<!--ID: 1669342979136-->



积分比大小怎么处理？  #flashcard
极限保号性、对称性，相同区间比函数，相同函数比区间，不同区间函数化为相同
<!--ID: 1669344694267-->



水中提取物体做功的密度ρ指代什么？ #flashcard
物体密度-水密度
<!--ID: 1669344694274-->



静水压力中的密度指代什么？   #flashcard
水密度
<!--ID: 1669344694279-->



三重积分的几种积分方式？   #flashcard
先一后二、先二后一、柱坐标、球坐标
<!--ID: 1669344694285-->




球坐标公式  #flashcard
$$
\iiint_{\Omega}f(x,y,z)dxdydz=\iiint_{\Omega}f(rsin\varphi cos\theta,rsin\varphi sin\theta,rcos\varphi)r^2sin\varphi d\theta d\varphi dr
$$
<!--ID: 1669344694290-->



第一型曲面积分公式   #flashcard
$$
\begin{align*}
&曲面\sum:z=g(x,y) 
\\\\
&\iint_{\sum}f(x,y,z)dS=\iint_{D_{xy}}f(x,y,g(x,y))\cdot
\sqrt{1+(\frac{\partial z}{\partial x})^2+(\frac{\partial z}{\partial y})^2}\ \ dxdy
\end{align*}
$$
<!--ID: 1669344694296-->



第一型曲面积分需要注意什么  #flashcard
1.投影不能重叠
2.要明确被消变量的正负
<!--ID: 1669344694302-->




格林公式是什么  #flashcard
$$
\oint_LP(x,y)dx+Q(x,y)dy=\iint_D(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y})d\sigma
$$
<!--ID: 1669344694306-->



格林公式的使用条件  #flashcard
- 有界闭区域D由分段光滑曲线L围成
- P(x,y)、Q(x,y)在D上具有一阶连续偏导数-<font color=red>如果只是函数连续,则不可使用格林公式</font>
- L取正方向-人沿着这个方向走的时候，左手始终在L所围的D内部
<!--ID: 1669344694311-->



斯托克斯公式是什么  #flashcard
$$
\begin{align*}
\oint_{\Gamma}P(x,y,z)dx+Q(x,y,z)dy+R(x,y,z)dz
=&\iint_{\sum}\begin{vmatrix}
 dydz&dzdx &dxdy \\
\frac{\partial }{\partial x} & \frac{\partial }{\partial y} &\frac{\partial }{\partial z}  \\
P &  Q& R \\
\end{vmatrix}
\\\\
=&\iint_{\sum}\begin{vmatrix}
 cos\alpha&cos\beta &cos\gamma \\
\frac{\partial }{\partial x} & \frac{\partial }{\partial y} &\frac{\partial }{\partial z}  \\
P &  Q& R \\
\end{vmatrix}dS
\\\\
其中\overrightarrow{n}=(cos\alpha,cos\beta,cos\gamma)为\sum的&单位外法线向量
\end{align*}
$$
<!--ID: 1669344694317-->



斯托克斯公式的使用条件  #flashcard
- Γ与$\sum$的法向量成右手系
- P，Q，R在Ω内具有连续的一阶偏导数-<font color=red>如果只是函数连续,则不可使用斯托克斯公式</font>
- <font color=red>使用斯托克斯公式之后-积分区域变化，原来函数关系不再成立</font>
- <mark>对于平面⇒第一型曲面积分，对于曲面⇒第二型曲面积分</mark>
<!--ID: 1669344694322-->



第二型曲面积分的解题方法有？  #flashcard
1.投影换元-转换投影法
2.高斯公式
<!--ID: 1669344694325-->



转换投影法是什么  #flashcard
$$
\begin{align*}
&\iint_{\sum}P(x,y,z)dydz+Q(x,y,z)dzdx+R(x,y,z)dxdy
\\\\
=&\pm \iint_{D_{xy}}P[x,y,z(x,y)](-\frac{\partial z}{\partial x})
+Q[x,y,z(x,y)](-\frac{\partial z}{\partial y})+Q[x,y,z(x,y)]dxdy
\end{align*}
$$
<!--ID: 1669344694331-->


转换投影法的要求是什么  #flashcard
- 1.其投影面不能有任何重叠部分，如果有重叠的话，要分割处理投影
- 2.其中当“<font color = "red">曲面的法向量</font>”和“<font color = "blue">被消变量的正轴方向夹锐角时取+</font>”
<!--ID: 1669344694335-->




高斯公式是什么？   #flashcard
$$
\newcommand{\oiint}{\subset\kern{-3pt}\supset\kern{-16.5pt}\iint}
\oiint_{\sum} Pdydz+Qdzdx+Rdxdy=\iiint_{\Omega}(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z})dv
$$
<!--ID: 1669344760977-->




高斯公式的要求是什么？  #flashcard
- 1.空间有界闭区域Ω由有向分片光滑曲面$\sum$围成
- 2.P(x,y,z)、Q(x,y,z)、R(x,y,z)在Ω上具有一阶连续偏导数
- 3.其中$\sum$取外侧
- <font color=red>使用高斯公式之后-积分区域变化，原来函数关系不再成立</font>
<!--ID: 1669344694345-->



一阶微分方程的处理方法有哪些？  #flashcard
换元-公式-伯努利
<!--ID: 1669344694350-->



二阶微分方程的公式有哪些？  #flashcard
二阶可降阶-二阶常系数-欧拉方程
<!--ID: 1669344694355-->




一阶微分方程的公式法？  #flashcard
$$
\begin{align*}
形如:y'+p(x)y=&q(x)
\\
\\
y=e^{-\int p(x)dx}
\{
\int e^{\int p(x)dx}\cdot &q(x)\ dx+C
\}
\end{align*}
$$
<!--ID: 1669344694359-->


伯努利方程是什么  #flashcard
$$
\begin{align*}
y'+p(x)y&=q(x)y^n
\\\\
令z=y^{1-n}\quad 则有:&\frac{1}{1-n}z'+p(x)z=q(x),再代公式
\end{align*}
$$
<!--ID: 1669344694364-->



欧拉方程是什么  #flashcard
$$
\begin{align*}
&形如:x^2y''+pxy'+qy=f(x)
\\
\\
&换元成如下形式:
\\ &
\begin{cases}
y''+(p-1)y'+qy=f(e^t) &x>0 \quad x=e^t
\\
\\
\\
y''+(p-1)y'+qy=f(-e^t) &x<0 \quad x=-e^t
\end{cases}
\end{align*}
$$
<!--ID: 1669344694368-->



绝对收敛，条件收敛于原级数收敛的关系  #flashcard
绝对收敛⇒原级数必收敛 
条件收敛前提是原级数收敛
<!--ID: 1669344694372-->



幂级数收敛域于收敛中心的关系  #flashcard
幂级数的收敛域关于收敛中心对称
<!--ID: 1669344694377-->



常用参考级数都有哪些？  #flashcard
$$
\begin{align*}
&➊ 等比级数\sum_{n=1}^{\infty}aq^{n-1}
\begin{cases}
 \frac{a}{1-q} &|q|<1
\\
\\
发散    &|q|>1
\end{cases}
\\\\
&➋p级数\sum_{n=1}^{\infty}\frac{1}{n^p}
\begin{cases}
收敛 &p>1
\\
\\
发散    &p \leq 1
\end{cases}
\\
\\
&➌广义p级数\sum_{n=2}^{\infty}\frac{1}{n(lnn)^p}
\begin{cases}
收敛 &p>1
\\
\\
发散    &p \leq 1
\end{cases}
\\
\\
&➍交错p级数\sum_{n=1}^{\infty}(-1)^{n-1}\frac{1}{n^p}
\begin{cases}
绝对收敛 &p>1
\\
\\
条件收敛    &0<p \leq 1
\end{cases}
\\
\end{align*}
$$
<!--ID: 1669344694382-->



阿贝尔定理  #flashcard
$$
\begin{align*}
&1.当幂级数\sum_{n=0}^{\infty}a_nx^n在点x=x_1处收敛时
\\
&\Rightarrow 对于|x|<|x_1|,幂级数绝对收敛
\\\\
&2.当幂级数\sum_{n=0}^{\infty}a_nx^n在点x=x_1处发散时
\\
&\Rightarrow 对于|x|>|x_1|,幂级数发散
\end{align*}
$$
<!--ID: 1669424707714-->




空间曲线的切向量怎么求解  #flashcard
$$
\begin{align*}
&参数方程:
\begin{cases}
x=x(t)
\\
y=y(t)
\\
z=z(t)
\end{cases}
\quad
\Rightarrow \quad
\overrightarrow\tau=(x'(t_0),y'(t_0),z'(t_0))
\\\\\\
&方程组:
\begin{cases}
F(x,y,z)
\\\\
G(x,y,z)
\end{cases}
\qquad 
\Rightarrow \quad 
\overrightarrow\tau=
\begin{vmatrix}
 \overrightarrow i&  \overrightarrow j &  \overrightarrow k\\
 F'_x&F'_y  &F'_z  \\
 G'_x&G'_y  &G'_z  \\
\end{vmatrix}_P
\end{align*}
$$
<!--ID: 1669344694390-->



空间曲面的法向量怎么求解  #flashcard
$$
\begin{align*}
&隐式方程:F(x,y,z)=0
\\\\
& \Rightarrow \overrightarrow {n}=(F'_x,F'_y,F'_z)|_p
\\\\
&显式方程:z=f(x,y)
\quad 
令F(x,y,z)=f(x,y)-z
\\\\
&\Rightarrow \overrightarrow {n}=(f'_x(x,y),f'_y(x,y),-1)|_p
\\\\
&参数方程:
\begin{cases}
x=x(u,v)
\\
y=y(u,v)
\\
z=z(u,v)
\end{cases}
\Rightarrow
\overrightarrow n=
\begin{vmatrix}
 \overrightarrow i&  \overrightarrow j &  \overrightarrow k\\
 x'_u&y'_u  &z'_u  \\
 x'_v&y'_v  &z'_v  \\
\end{vmatrix}_P
\end{align*}
$$
<!--ID: 1669344694397-->



曲线绕坐标轴旋转产生的曲面表达式  #flashcard
$$
\begin{align*}
&从直线方程中解出:x=\varphi(z),y=\psi(z)
\\\\
&旋转曲面方程:x^2+y^2=\varphi^2(z)+\psi^2(z)
\end{align*}
$$
<!--ID: 1669344694401-->


方向导数与偏导数关系  #flashcard
- 方向导数：函数在某一个方向上的导数
- 偏导数：只要求x，y方向。但是要求x，y方向的双侧！
- 方向导数只要求一侧有值即可，偏导数要求x，y双侧有值且相等
- 两者互相不能推出
<!--ID: 1669344694405-->



散度公式  #flashcard
$$
散度:div\ \mathbf{A}=\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}
+\frac{\partial R}{\partial z}
$$
<!--ID: 1669344694409-->



旋度公式  #flashcard
$$
旋度:\mathbf{rot \ A}=
\begin{vmatrix}
 \mathbf{i}&\mathbf{j} &\mathbf{k} \\
\frac{\partial }{\partial x} & \frac{\partial }{\partial y} &\frac{\partial }{\partial z}  \\
P &  Q& R \\
\end{vmatrix}
$$
<!--ID: 1669344694414-->



求解行列式的几种方法  #flashcard
- 消出一行或一列出现单0，然后按单0展开。展开时注意存在符号问题！
- 爪型、三对角线型、拉普拉斯(符号问题)、范德蒙、上下三角(符号问题)
- 技巧：逐行相加、全加到第一行、对角线消元素
<!--ID: 1669379440264-->



初等矩阵的逆阵与n次方  #flashcard
$$
\begin{align*}
&E_{ij}^{-1}(k)=E_{ij}(-k);\quad E_{ij}^{-1}=E_{ij};\quad E_{i}^{-1}(k)=E_{i}(\frac{1}{k});\quad
\\\\
&E_{ij}^{n}(k)=E_{ij}(nk);\quad E_{ij}^{n}=
\begin{cases}
E_{ij}, &n=2k
\\\\
E,&n=2k-1
\end{cases}
\\\\
&E_{i}^{n}(k)=E_{i}(k^{n});\quad
\end{align*}
$$
<!--ID: 1669424645781-->




向量线性相关的定义  #flashcard
$$
\begin{align*}
&对于n维向量\alpha_1,\alpha_2...\alpha_s,存在不全为0的k_i,使得
\\
&k_1\alpha_1+k_2\alpha_2+...+k_s\alpha_s=0
\\
&则称向量\alpha_1,\alpha_2...\alpha_s线性相关
\end{align*}
$$
<!--ID: 1669379440274-->



线性相关的四个充要条件  #flashcard
$$
\begin{align*}
&1.[\alpha_1,\alpha_2,...,\alpha_s]x=0有非零解
\\\\
&2.r(\alpha_1,\alpha_2,...,\alpha_s)<s\Leftrightarrow方程组的个数小于未知数的个数
\\\\
&3.某\alpha_i可以由\alpha_1,...,\alpha_{i},...,\alpha_s线性表出
\\\\
&4.n个n维向量线性相关的充分必要条件是行列式为0，克拉默法则
\end{align*}
$$
<!--ID: 1669379440281-->


线性相关的三个充分条件  #flashcard
$$
\begin{align*}
&1.n+1个n维向量一定线性相关
\\\\
&2.多数向量能用少数向量表示
\\\\
&3.存在零向量
\end{align*}
$$
<!--ID: 1669379440285-->



线性无关的定义  #flashcard
$$
\begin{align*}
&对于n维向量\alpha_1,\alpha_2...\alpha_s,只有当k_i全部为0时才有:
\\
&k_1\alpha_1+k_2\alpha_2+...+k_s\alpha_s=0
\\
&则称向量\alpha_1,\alpha_2...\alpha_s线性无关
\end{align*}
$$
<!--ID: 1669379440290-->


线性无关证明题常用方法  #flashcard
1.假设存在一组k，证明其全为0
2.重组方程组，转变为已知的线性无关组
3.用秩
<!--ID: 1669379440295-->




线性表出的定义  #flashcard
$$
\begin{align*}
&对于n维向量\alpha_1,\alpha_2...\alpha_s和\beta,存在k_i,使得
\\
&k_1\alpha_1+k_2\alpha_2+...+k_s\alpha_s=\beta
\\
&则称向量\beta可以由 \alpha_1,\alpha_2...\alpha_s线性表出
\end{align*}
$$
<!--ID: 1669379440300-->


基础解系的定义  #flashcard
- 齐次方程组解的极大无关组
- 是解、极大(n-r(A))、无关
<!--ID: 1669379440303-->




齐次方程组线性无关解向量个数  #flashcard
n-r(A)
<!--ID: 1669379440309-->



非齐次方程组线性无关解向量个数  #flashcard
n-r(A)+1
<!--ID: 1669379440314-->



几种矩阵之间特征值的联系  #flashcard
$$
\begin{align*}
\begin{array}{c| c c c c c c}
A& kA+E& A+kE&A^{-1} &A^*&A^n&P^{-1}AP
\\\hline
\lambda&k\lambda+1&\lambda+k &\frac{1}{\lambda}&\frac{|A|}{\lambda}&\lambda^n &\lambda
\\\hline
\alpha&\alpha&\alpha &\alpha&\alpha&\alpha&P^{-1}\alpha
\end{array}
\end{align*}
$$
<!--ID: 1669379440318-->



$\alpha \alpha^T$相似于什么矩阵  #flashcard
$\alpha \alpha^T$是秩为1的实对称矩阵，相似于diag$(\alpha^T\alpha,0,\cdots,0)$
<!--ID: 1669379440323-->



正交变换是什么  #flashcard
正交变换$Q^TAQ=\Lambda \Rightarrow x^TAx \ \overset{x=Qy}{=\!=\!=} \ y^T \Lambda y$
<!--ID: 1669379440327-->



将二次型化为标准型有哪些方法  #flashcard
正交变换
配方法
<!--ID: 1669379440332-->



微积分方程怎么处理  #flashcard
求导化为微分方程
<!--ID: 1669379440336-->



周期函数的积分特性  #flashcard
$$
\begin{align*}
&\int_{0}^{nT}f(x)dx=n\int_{0}^{T}f(x)dx
\\\\
&\int_{0}^{T}f(x)dx=\int_{a}^{a+T}f(x)dx
\end{align*}
$$
<!--ID: 1669379440341-->



在使用常用级数的和函数时，需要特别注意什么？  #flashcard
n的起始值
<!--ID: 1669379440347-->



斯托克斯公式转为曲面积分的曲面要怎么选择？  #flashcard
只要是以那条空间曲线为边界的均可
<!--ID: 1669379440350-->




线性无关有哪些证明方式？ #flashcard
1. 将待证的向量矩阵写作已知线性无关的向量矩阵与系数阵的乘积
2. 假设存在一组k使得与β的线性组合为0，证明其k均为0
<!--ID: 1669379460019-->



如果似然函数为那怎么求最大似然估计  #flashcard
此时最大似然估计为使得似然函数非0的一个范围
<!--ID: 1669379460024-->



随机变量最值的概率分布  #flashcard
$Y=min\{X_1,X_2,\cdots,X_n\}$
$Z=max\{X_1,X_2,\cdots,X_n\}$
$$
\begin{align*}
&F_Y(y)=1-[1-F(y)]^n
\\\\
&f_Y(y)=n[1-F(y)]^{n-1}f(y)
\\\\
&X_i \overset{iid}\sim U(0,\theta) \Rightarrow\frac{\theta}{n+1}
\end{align*}
$$
$$
\begin{align*}
&F_Z(z)=[F(z)]^n
\\\\
&f_Z(z)=n[F(z)]^{n-1}f(z)
\\\\
&X_i \overset{iid}\sim U(0,\theta) \Rightarrow\frac{n\theta}{n+1}
\end{align*}
$$
<!--ID: 1669379460027-->




$(1+x)^a$的等价无穷小  #flashcard
$$(1+x)^a=1+ax+\frac{\alpha(\alpha-1)}{2}x^2+o(x^2)(a\neq0)$$
<!--ID: 1669517119074-->



计算极限的几种方法？  #flashcard
直接计算法
等价无穷小
夹逼定理
<!--ID: 1669531468442-->



间断点类型都有哪些  #flashcard
$$
\begin{cases}
第一类间断点
\begin{cases}
可去间断点\quad \lim_{x\to x_0^-}f(x)=\lim_{x\to x_0^+}f(x)\neq f(x)
\\\\
跳跃间断点\quad \lim_{x\to x_0^-}f(x)\neq\lim_{x\to x_0^+}f(x)
\end{cases}
\\\\\\
第二类间断点
\begin{cases}
无穷间断点\quad  \lim_{x\to x_0^-}f(x)=\infty 或者 \lim_{x\to x_0^+}f(x)=\infty
\\\\
震荡间断点\quad  \lim_{x\to x_0^-}f(x)=振荡不存在or \lim_{x\to x_0^+}f(x)振荡不存在
\end{cases}
\end{cases}
$$
<!--ID: 1669531468450-->



导数为0的点一定是极值点吗？  #flashcard
不一定如$y=x^3$
<!--ID: 1669531468453-->



多元函数偏导数几种方式求解？  #flashcard
链式求导、隐函数法、全微分形式不变
<!--ID: 1669531468457-->



常用的基本不等式有哪些？  #flashcard
$$
\begin{align*}
&\frac{2}{\frac{1}{x}+\frac{1}{y}}\leq \sqrt{xy} \leq\frac{{x+y}}{2}\leq \sqrt{\frac{x^2+y^2}{2}}
\\\\
&e^x-1 \geq x  \qquad ln(x+1) \leq x
\\\\
&tanx>x>\frac{x}{x^2+1}
\end{align*}
$$
<!--ID: 1669531468462-->



比较判别法的极限形式？  #flashcard
$$
\begin{align*}
\lim_{n \to \infty}\frac{u_{n}}{v_{n}} =
\begin{cases}
0  
\\
+\infty
\\
A   &同敛散
\end{cases}
\end{align*}
$$
<!--ID: 1669531468465-->


交错级数的莱布尼茨判别法  #flashcard
$$
\begin{align*}
&\sum_{n=1}^{\infty}(-1)^{n-1}u_{n}满足如下两个条件收敛
\\
&➊ \lim_{n \to \infty}u_{n}=0 \quad 任何级数收敛的必要条件
\\
&➋ 存在某个k   \qquad 当n \geq k;u_{n} \geq u_{n+1}
\end{align*}
$$
<!--ID: 1669531468469-->




事件概率之和为0说明什么？  #flashcard
每个事件的概率都是0
<!--ID: 1669531468473-->




二阶常系数微分方程需要怎么预处理  #flashcard
划分为“齐次”与“非齐次”
<!--ID: 1669531468477-->



写函数表达式的时候需要注意什么  #flashcard
<font color = red>一定要带上定义域</font>
<!--ID: 1669531468481-->




曲线绕坐标轴旋转公式  #flashcard
$v=\int_{a}^{b}\pi f^2(x) dx\quad v=\int_{a}^{b}2\pi xf|(x)|dx$
<!--ID: 1669531468485-->


怎么求解曲面面积？ #flashcard
$$S=\iint_{\sum}1 dS$$
<!--ID: 1669542029100-->


椭圆面积公式？  #flashcard
$$
\begin{align*}
&S=\pi ab
\\\\
&a,b分别为椭圆的长半轴与短半轴的长度
\end{align*}
$$
<!--ID: 1669542155281-->



随机变量映射后的变量概率怎么求解？  #flashcard
将其转换为原随机变量等价的事件
<!--ID: 1669621812337-->


已知Z=g(X,Y)，怎么求解Z的期望EZ  #flashcard
$$ EZ=\int_{-\infty}^{+\infty}\int_{-\infty}^{+\infty}g(x,y)f(x,y)dxdy$$
<!--ID: 1669621812340-->




两个随机变量独立的时候才可以卸磨杀驴，不独立的怎么做？  #flashcard
全集分解，转化为等价事件概率；不可以在不独立的条件下，直接消掉条件！！！
<!--ID: 1669621812343-->



样本方差的计算公式？  #flashcard
$$
S^2=\frac{1}{n-1}\sum_{i=1}^{n}(X_i-\overline X)^2=\frac{1}{n-1}(\sum_{i=1}^{n}X_i^2-n\overline X^2)
$$
<!--ID: 1669636999806-->


圆锥面方程与抛物面方程区别？ #flashcard
圆锥面：$z=\sqrt{x^2+y^2}\quad z^2=x^2+y^2$
抛物面：$z=x^2+y^2$
<!--ID: 1669637017746-->



二维随机变量-卷积公式法  #flashcard
1. 积谁不换谁,换完求偏导
2. 偏导加绝对,还要换区域
3. 从-扫到+,分组求积分
常用四种卷积公式:
$$
\begin{align*}
➊Z=&X+Y
\\\\
f_Z(z)=&\int_{-\infty}^{+\infty}f(x,z-x)dx
\overset{\underset{\mathrm{X,Y独立}}{}}{=}\int_{-\infty}^{+\infty}f_X(x)\cdot f_Y(z-x)dx
\\\\
➋Z=&X-Y
\\\\
f_Z(z)=&\int_{-\infty}^{+\infty}f(x,x-z)dx
\overset{\underset{\mathrm{X,Y独立}}{}}{=}\int_{-\infty}^{+\infty}f_X(x)\cdot f_Y(x-z)dx
\\\\
➌Z=&XY
\\\\
f_Z(z)=&\int_{-\infty}^{+\infty}\frac{1}{|x|}f(x,\frac{z}{x})dx
\overset{\underset{\mathrm{X,Y独立}}{}}{=}\int_{-\infty}^{+\infty}\frac{1}{|x|}f_X(x)\cdot f_Y(\frac{z}{x})dx
\\\\
➍Z=&\frac{X}{Y}
\\\\
f_Z(z)=&\int_{-\infty}^{+\infty}|y|f(zy,y)dy
\overset{\underset{\mathrm{X,Y独立}}{}}{=}\int_{-\infty}^{+\infty}|y|f_X(zy)\cdot f_Y(y)dy
\end{align*}
$$
<!--ID: 1669782012829-->



$A^T$与$A$特征值之间的关系？  #flashcard
相同：$|\lambda E-A^T|=|(\lambda E-A^T)^T|$
<!--ID: 1669782012833-->



二重积分的极限题怎么求解  #flashcard
1. 二重积分的中值定理
2. 直接解出二重积分
3. 化为可洛必达的形式：被积函数应当只有<font color=red>一元</font>变量
<!--ID: 1669782012837-->




范德蒙行列式  #flashcard
$$
\begin{align*}
\begin{vmatrix}
 1&1&\cdots&1  \\
 x_1&x_2&\cdots&x_n  \\
 x_1^2&x_2^2&\cdots&x_n^2  \\
\vdots&\vdots& &\vdots  \\
 x_1^{n-1}&x_2^{n-1}&\cdots&x_n^{n-1}  \\
\end{vmatrix}=\prod_{1\leq j<i\leq n}(x_i-x_j)
\end{align*}
$$
<!--ID: 1669782012840-->


随机变量和差的期望  #flashcard
$$
D(X\pm Y)=D(X)+D(Y)\pm 2cov(X,Y)
$$
<!--ID: 1669782012844-->



怎么求解级数收敛域  #flashcard
$$
\begin{align*}
&对于\sum u_n f(x_n)
\\\\
&\lim_{n\to \infty}|\frac{u_n f(x_n)}{u_{n-1} f(x_{n-1})}|<1
\end{align*}
$$
<!--ID: 1669812941285-->




Ax=0与Bx=0同解的充要条件  #flashcard
$$
r(A)=r\begin{pmatrix}
A \\B
\end{pmatrix}=r(B)
$$
<!--ID: 1669812941291-->



Ax=0的解是Bx=0的解的充要条件  #flashcard
$$
r(A)=r\begin{pmatrix}
A\\B
\end{pmatrix}
$$
<!--ID: 1669812941296-->



二重积分换元法有什么需要注意的  #flashcard
不要忘记<font color=red>雅可比行列式</font>
$$
\begin{align*}
&x=x(u,v)\qquad y=y(u,v)
\\\\
&dxdy \to 
\begin{vmatrix}
\frac{\partial (x,y)}{\partial (u,v)} 
\end{vmatrix}
dudv
\\\\
&\frac{\partial (x,y)}{\partial (u,v)}
=
\begin{vmatrix}
\frac{\partial x}{\partial u} & \frac{\partial x}{\partial v}
\\
\frac{\partial y}{\partial u} & \frac{\partial y}{\partial v}
\end{vmatrix}
\end{align*}
$$
<!--ID: 1669812941300-->



存在二阶导数且涉及到定积分的时候怎么处理?  #flashcard
在定积分的区间中点位置展开
<!--ID: 1669812941305-->


求解期望的时候，要明确什么？  #flashcard
哪个是固定常数，哪个又是随机变量
<!--ID: 1669885498475-->



定积分区间对称考虑什么?  #flashcard
对称性
区间再现公式
<!--ID: 1669885498483-->




一个表达式与某一个参数的取值无关等价于什么？  #flashcard
相对于那个参数，此表达式为常数
即对该参数求导，导数为0
<!--ID: 1669885498490-->




数列极限大题
1. 已知$a_n$具体的表达式
2. 已知$a_n$抽象的关系等式
  #flashcard
1. 单调有界准则
2. 放缩夹逼
<!--ID: 1669885498497-->



讨论某个向量α和其余向量之间关系时，怎么处理  #flashcard
将α表出为已知向量的线性表出
<!--ID: 1669885498504-->



对于三阶矩阵，若α1、α2、α3分别是λ1=λ2、λ3对应的特征向量
怎么证明如果α垂直α3，α就是对应λ1=λ2的特征向量
  #flashcard
  将α用α1、α2、α3表出
<!--ID: 1669885498510-->


两个矩阵合同的充要条件？  #flashcard
正负惯性指数相等$Q^TAQ=B$
<!--ID: 1670156897317-->



如果已知一个矩阵A是正定矩阵，怎么证明另一个矩阵B也是正定矩阵？  #flashcard
证明A、B合同，$Q^TAQ=B$
<!--ID: 1670156897325-->



如果事件A的概率P(A)=0/1，那它有什么性质？  #flashcard
A与任何事件之间都相互独立
<!--ID: 1670156897330-->



三个事件之间相互独立的等价条件  #flashcard
$$
\begin{align*}
&A、B、C相互独立 \Leftrightarrow
\begin{cases}
P(AB)=P(A)\cdot P(B)
\\\\
P(BC)=P(B)\cdot P(C)
\\\\
P(AC)=P(A)\cdot P(C)
\\\\
P(ABC)=P(A)\cdot P(B)\cdot P(C)
\end{cases}
\end{align*}
$$
<!--ID: 1670156897338-->



在某点处的高阶导数怎么求解？  #flashcard
1. 泰勒展开
2. 莱布尼茨公式，组合函数的n阶导数
<!--ID: 1670156897343-->



如果已知A，则$x^TAx=0$可以通过解方程求得x,那如果是矩阵呢$B_{m×n}^TAB_{m×n}$  #flashcard
可以将$B_{m×n}$表示为n个关于x的方程组，求解后合并为矩阵B
<!--ID: 1670156897347-->



tr(A)、tr(A*)、|A|和矩阵特征多项式的关系  #flashcard
$$
\begin{align*}
|\lambda E-A|&=\lambda^3-(a_{11}+a_{22}+a_{33})\lambda^2+(A_{11}+A_{22}+A_{33})\lambda-|A|
\\\\
&=(\lambda-\lambda_1)\cdot (\lambda-\lambda_2)\cdot (\lambda-\lambda_3)
\end{align*}
$$
<!--ID: 1670156897351-->


如果矩阵A是实对称矩阵，那么A* 是实对称矩阵吗？  #flashcard
是的
<!--ID: 1670156897355-->


已知α、β、γ分别是$A^T,A^*,A^2$的特征向量，那他们是A的特征向量吗？
不一定

$P(A\cup B \cup C)=$?  #flashcard
$P(A\cup B \cup C)=P(A)+P(B)+P(C)-P(AB)-P(AC)-P(BC)+P(ABC)$
<!--ID: 1670156897359-->



P(A)+P(B)与P(AB)的关系？  #flashcard
$P(A)+P(B)\ge 2P(AB)$
<!--ID: 1670156897362-->



前n项的平方和公式  #flashcard
$\frac{1}{6}n(n+1)(2n+1)$
<!--ID: 1670156897366-->



合工大2-平面与曲面相交之后的上侧，投影时需要注意什么？  #flashcard
此时实际投影应该是交线的投影，而不再是原曲面的投影
<!--ID: 1670156897370-->



中值定理的证明题怎么考虑第一步？  #flashcard
将待证明的等式移项，构成某个新的函数的导数
<!--ID: 1670156897373-->



正定矩阵的对角线元素都为正对吗？  #flashcard
是的
<!--ID: 1670156897377-->



求z的概率密度函数，应该怎么做？  #flashcard
按z的情况分类讨论
<!--ID: 1670156897380-->


齐次方程组有非零公共解的充要条件  #flashcard
$$
\begin{align*}
n阶矩阵A、B,Ax=0与Bx=0有非零公共解\Leftrightarrow r\begin{pmatrix}
A\\B
\end{pmatrix}<n
\end{align*}
$$
<!--ID: 1670307437091-->


若r(A)=1，则A的特征值有哪些？ #flashcard
(n-1)个0，以及tr(A)
<!--ID: 1670307437097-->



如果某个矩阵的主对角元素都有相同的参数，可以怎么处理？ #flashcard
将其拆分，使参数全到单位阵上
<!--ID: 1670307437101-->



如果已知数列递推关系，可以选择怎么求解数列 #flashcard
带值，找规律，数学归纳法
<!--ID: 1670307437105-->



如果矩阵A满足:$A^2+A-2E=0$,说明矩阵A的特征值有什么特点？ #flashcard
矩阵A的特征值一定为1或者-2
<!--ID: 1670410671331-->



$1-\frac{1}{2}+\frac{1}{3}-\frac{1}{4}\cdots$等于多少 #flashcard
$\sum_{n=1}^{+\infty}(-1)^{n-1}\frac{x^n}{n}=ln(1+x)|_{x=1}=ln2$
<!--ID: 1670410671343-->

	

处理极限的时候，相同架构的函数差值，怎么处理？ #flashcard
拉格朗日中值定理
<!--ID: 1670410671349-->



$|(-1)A|=$? #flashcard
$(-1)^n|A|$
<!--ID: 1670484773077-->



二项分布、卡方分布的最大似然估计与据估计有什么联系？ #flashcard
两者相等
<!--ID: 1670484773084-->


判断级数的敛散性时，使用等价无穷小的条件是什么？ #flashcard
得是正项级数
<!--ID: 1670730365384-->



判断级数得收敛性，可以使用什么公式将其转换为幂级数和得敛散性？ #flashcard
泰勒展开
<!--ID: 1670730365390-->




线性表出、线性相关、不相关都有哪些思路？ #flashcard
1. 定义法
2. 将待证向量组表示为已知向量组与某矩阵的乘积
<!--ID: 1670914929390-->



利用二次型矩阵A研究二次型的性质（正定、合同...）时，对A有什么要求 #flashcard
A必须是实对称矩阵
<!--ID: 1670914929404-->


两个矩阵合同的充要条件 #flashcard
正负惯性指数相等+两个矩阵都是对称矩阵
<!--ID: 1670914929411-->



若$A=C^TC$，是否可说明矩阵A正定？ #flashcard
不可以！！！未知C是否可逆
<!--ID: 1670914929417-->


在求具体点的偏导数时候，可以怎么处理？ #flashcard
将非求导变量的值导入表达式，化简为一元
<!--ID: 1670986350080-->



已知$|Q|\ne0,Q^{-1}AQ=B$,求A  #flashcard
$A=QBQ^{-1}$
只有通过逆阵才能实现矩阵的相消
<!--ID: 1670986350087-->



对于一阶微分方程积分成对数时候需要注意什么？  #flashcard
此时去掉对数，常数项应当与函数部分相乘积
<!--ID: 1670986350091-->



矩阵组合的行列式求解思路  #flashcard
1. 表示为矩阵的乘积，然后拆开各自求解
2. 求出组合矩阵的特征值
<!--ID: 1670986350096-->


伴随矩阵中$A_{ij}$与$a_{ij}$的关系？  #flashcard
没有任何关系！！！
<!--ID: 1671249238474-->



对于形如$(x-1)^2+(y-1)^2\le 1$的积分区域，可以怎么做  #flashcard
令$\begin{cases}x=u+1\\ y=v+1 \end{cases}$，但是换元的时候要记得会引入雅可比行列式
换元的目的是为了更好的使用其对称性
<!--ID: 1671249238485-->



拉格朗日与泰勒的变体 #flashcard
令$\theta=\frac{\xi-a}{b-a}$，实际上就是约束到(0,1)的单值映射
<!--ID: 1671249238490-->




$\sum_{n=1}^{+\infty}\frac{1}{4n+1}x^n$怎么处理？ #flashcard
令$x=t^4$
<!--ID: 1671249238495-->



$a_{ij}=A_{ij}$意味着什么 #flashcard
$A^{*}=A^{T}$
<!--ID: 1671249238500-->



如果A,B正定，则AB正定的充要条件是 #flashcard
AB=BA
<!--ID: 1671450251075-->



如果A正定且A是正交矩阵，有什么结论 #flashcard
A=E
<!--ID: 1671450251079-->


P(AB)、P(A)、P(A+B)的关系 #flashcard
$P(AB)\le P(A)\le P(A+B)$
<!--ID: 1671450251083-->

