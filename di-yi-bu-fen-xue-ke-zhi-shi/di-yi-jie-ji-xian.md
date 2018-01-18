### 1.1 一元二次方程$$ax^2+bx+c=0$$的求解

设$$\Delta = b^2-4ac$$,

当$$\Delta &gt; 0$$时，有2个不相等的实数根，$$x_1 = \frac{-b+ \sqrt{b^2-4ac}}{2a},x_2=\frac{-b-\sqrt{b^2-4ac}}{2a}$$;

当$$\Delta = 0$$时，有2个相等的实数根，$$x_1=x_2=\frac{-b}{2a}$$;

当$$\Delta &lt; 0$$时，没有实数根。

有2个实数根时，有$$x_1+x_2=\frac{-b}{a},x_1x_2=\frac{c}{a}$$。

$$x=\frac{-b \pm \sqrt{(b^2-4ac)} } {2a}$$




# 一、实数的完备性
## （一）实数的完备性
### 1.确界
确界：上确界与下确界统称为确界。
（1）上确界：设$$S$$为$$\mathbb{R}$$中的一个数集。若数$$\eta$$满足：对一切$$x\in S$$，都有$$x\leqslant\eta$$即$$\eta$$是$$S$$的上界；对任何$$\alpha < \eta$$，存在$$x_0\in S$$，即$$\eta$$又是$$S$$的最小上界，则称数$$\eta$$为数集$$S$$的上确界，记作$$\eta=\sup S$$。

（2）下确界：设$$S$$为$$\mathbb{R}$$中的一个数集$$\mathbb{R}$$。若数$$\xi$$满足：对一切$$x\in S$$，都有$$x\geqslant\xi$$，即$$\xi$$是$$S$$的下界；对任何$$\beta > \xi$$，存在$$x_0\in S$$，是的$$x_0 > \beta$$，即$$\xi$$又是$$S$$的最大下界，则称$$\xi$$为数集$$S$$的下确界，记作$$\xi=\inf S$$。



### 2.单调数列
单调数列：若数列$$\{a_n\}$$的各项满足关系式$$a_n \leqslant a_{n+1}$$，则$$\{a_n\}$$为递增数列；若数列$$\{a_n\}$$的各项满足关系式$$a_n \geqslant a_{n+1}$$，则$$\{a_n\}$$为递减数列，递增数列和递减数列统称为单调数列。

### 3.区间套
区间套：设闭区间列$$\{[a_n,b_n]\}$$具有如下性质：$$[a_n,b_n] \supset [a_{n+1},b_{n+1}],n=1,2,\cdots;\lim_{n\rightarrow+\infty}(b_n-a_n)=0$$，则$$\{[a_n,b_n]\}$$为闭区间套，或简称区间套。

### 4.聚点
聚点：设$$S$$为数轴上的点集，$$\xi$$为定点（它可是属于$$S$$，也可以不属于$$S$$）。若$$\xi$$的任何邻域内都含有$$S$$中无穷多个点，则称$$\xi$$为点集$$S$$的一个聚点。

### 5.开覆盖
开覆盖：$$S$$为数轴上的点集，$$H$$为开区间的集合，即$$H$$的每一个元素是形如$$(\alpha,\beta)$$的开区间。若$$S$$中任何一点都含有$$H$$中至少一个开区间内，则称$$H$$为$$S$$的一个开覆盖，或称$$H$$覆盖$$S$$。若$$H$$中开区间的个数是无限（有限）的，则称$$H$$为$$S$$的一个无限开覆盖（有限开覆盖）。

## （二）关于实数完备性的六个基本定理
### 1.确界原理
确界原理：设$$S$$为非空数集。若$$S$$有上界，则$$S$$必有上确界；若$$S$$有下界，则$$S$$必有下确界。

### 2.单调有界定理
单调有界定理：在实数系中，有界的单调数列必有极限。

### 3.区间套定理
区间套定理：若$$\{[a_n,b_n]\}$$是一个区间套，则在实数系中存在唯一的一点$$\xi$$，使得$$\xi \in [a_n,b_n],n=1,2,\cdots$$，即$$a_n\leqslant\xi b_n,n=1,2,\cdots$$。

### 4.有限覆盖定理
海涅-博雷尔（Heine-Borel）有限覆盖定理：设$$H$$为闭区间$$[a,b]$$的任一（无限）开覆盖，则从$$H$$中可选出有限个开区间来覆盖$$[a,b]$$。

### 5.聚点定理
魏尔斯特拉斯（Weierstrass）聚点定理：实轴上的任一有界无限点集$$S$$至少有一个聚点。

### 6.柯西收敛准则
柯西（Cauchy）收敛准则：数列$$\{a_n\}$$收敛的冲要条件是：对任一给定$$\varepsilon > 0$$，存在$$N > 0$$，使得当$$n,m > N$$时，有$$|a_n-a_m|< \varepsilon$$成立。

# 二、极限
## （一）极限的定义
**定义1**：$$\lim_{n\rightarrow\infty}x_n=A：\forall\varepsilon > 0，\exists$$正整数$$N$$，当$$n > N$$时，有$$|x_n-A| < \varepsilon$$。
若$$x_n$$存在极限（有限数），又称$$\{x_n\}$$收敛，否则称$$\{x_n\}$$发散。

**定义2**：$$\lim_{x\rightarrow\infty}f(x)=A：\forall\varepsilon > 0，\exists$$正整数$$X$$，当$$|x| > X$$时，有$$|f(x)-A| < \varepsilon$$。
类似可定义：$$\lim_{x\rightarrow +\infty}f(x)=A，\lim_{x\rightarrow -\infty}f(x)=A$$。

**定义3**：$$\lim_{x\rightarrow x_0}f(x)=A：\forall\varepsilon > 0，\exists$$正整数$$\delta$$，当$$0 < |x-x_0| > \delta$$时，有$$|f(x)-A| < \varepsilon$$。
类似可定义$$f(x)$$当$$x \rightarrow x_0$$时右极限与左极限：
$$f(x_0+0) = \lim_{x\rightarrow x_0}f(x) = A，f(x_0-0) = \lim_{x\rightarrow x_0}f(x) = A$$。


## （二）极限的基本性质与两个重要极限
### 1.数列极限的基本性质
**性质1：（极限的不等式性质）**设$$\lim_{n\rightarrow+\infty}x_n = a，lim_{n\rightarrow+\infty}y_n = b$$，若$$a > b$$，则$$\exists N$$，当$$n > N$$时，$$x_n > y_n$$；若$$n > N$$时，$$x_n \geqslant y_n$$，则$$a \geqslant b$$。
**性质2：（收敛数列的有界性）**设$$x_n$$收敛，则$$x_n$$有界（即$$\exists$$常数$$M > 0,|x_n|\geqslant M,n=1,2,\cdots$$）。


### 2.函数极限的基本性质
**性质1：（极限的不等式性质）**设$$\lim_{x\rightarrow x_0}f(x) = A，\lim_{x\rightarrow x_0}g(x) = B$$，
若$$A > B$$，则$$\exists \delta$$，当$$0< |x-x_0|< \delta$$时，$$f(x)>g(x)$$；
若$$f(x) \geqslant g(x)$$（$$0 < |x-x_0| < \delta$$），则$$A \geqslant B$$。
**【推论】（极限的局部保号性）**设$$\lim_{x\rightarrow x_0}f(x) = A$$，则$$f(x)$$在$$x_0$$的某空心邻域$$ U_0(x_0, \delta) = |x| 0< |x-x_0| < \delta|$$内有界，即$$\exists \delta > 0,M > 0$$，使得$$0 < |x-x_0| < \delta$$时，$$|f(x)|\leqslant M$$。



### 3.两个重要极限
$$\lim_{x\rightarrow 0}\frac{\sin x}{x} = 1，\lim_{x\rightarrow 0}(1+ \frac 1x)^x = e $$
$$(\lim_{x\rightarrow 0}(1+x)^{\frac 1x} = e，\lim_{x\rightarrow 0}\frac{\ln(1+x)}{x} = 1 )$$

## （三）求极限的方法
求极限的方法很多，一下结合立体介绍几种常用的、简单的求极限的方法。
### 1.利用变量替换法与两个重要极限

### 2.利用灯姐无穷小因子替换
若$$x\rightarrow a$$时，无穷$$小\alpha (x)~\alpha^*(x)$$，$$\beta  (x)~\beta^*(x)，（即\lim_{x\rightarrow a} \frac{\alpha(x)}{\alpha^*(x)} = 1，\lim_{x\rightarrow a}\frac{\beta(x)}{\beta^*(x)} = 1$$），则$$\lim_{x\rightarrow a}\frac{\alpha(x)u(x)}{\beta(x)v(x)} = \lim_{x\rightarrow a}\frac{\alpha^*(x)u(x)}{\beta^*(x)v(x)}。$$
（等式两边其中之一极限存在或为$$\infty$$，则另一边也是且相等。）

### 3.利用洛必达法则

### 4.分别求左右极限的函数极限

### 5.利用夹逼法
用夹逼定理求极限$$\lim_{n\rightarrow \infty}x_n$$，就是要将数列$$\{x_n\}$$放大与缩小成：$$z_n \geqslant x_n \geqslant y_n$$，要想成功，必须是极限$$\lim_{n\rightarrow \infty}y_n$$与$$\lim_{n\rightarrow \infty} z_n$$会求且相等。

dd




















