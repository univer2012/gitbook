# 一、连续性概念
1.若$$\displaystyle \lim_{x\rightarrow x_0}f(x) = f(x_0)$$，称$$f(x)$$在$$x_0$$连续。
2.若$$\displaystyle\lim_{x\rightarrow x_0^+}f(x) = f(x_0)$$（$$\displaystyle \lim_{x\rightarrow x_0^-}f(x) = f(x_0)$$），称$$f(x)$$在$$x=x_0$$右（左）连续。

（单双侧连续性的关系）$$f(x)$$在$$x_0$$连续 $$\Leftrightarrow f(x)$$在$$x_0$$既左连续又右连续。
3.若$$f(x)$$在$$(a, b)$$内任一点均连续，称$$f(x)$$在$$(a, b)$$内连续。
4.$$若f(x)在(a,b)连续，在x=a右连续，在x=b左连续，称f(x)在[a, b]上连续。$$

# 二、函数连续性的判断
**1.（连续性的size运算法则）**$$设f(x)，g(x)在x_0连续，则f(x)\pm g(x)，f(x)\cdot g(x)，f(x)/g(x)（g(x_0)\neq 0)）在x_0也连续。$$
**2.（复合函数的连续性）**$$设u=\varphi(x)在x=x_0连续，y=f(u)在u=u_0（u_0=\varphi(x_0)）连续，则f(\varphi(x))在x=x_0连续。$$
**3.（反函数的连续性）**设$$y=f(x)$$在区间$$I_x$$上单调且连续，则反函数$$x=\varphi(y)$$也在对应的区间$$I_y = \{y|y=f(x),x\in I_x\}$$上连续且有相同的单调性。


# 三、连续函数的性质
**性质1：**设$$f(x)在x=x_0连续，f(x_0)>0，则\exists\delta > 0，当|x-x_0|< \delta时，f(x)>0。$$
**性质2：（连续函数介值定理（中间值定理））**设$$f(x)$$在$$[a, b]$$上连续，$$f(a)\neq f(b)$$，则对f(a)与f(b)之间的任何数$$\eta$$，则必定$$\exists c(a < c < b)$$，使得$$f(c)=\eta$$。

**性质3：（有界闭区间上连续函数的有界性）**设$$f(x)$$在$$[a, b]$$上连续，则$$f(x)$$在$$[a, b]$$有界，即存在常数$$M>0$$，对任意$$x \in [a, b]$$，使得$$|f(x)| \leqslant M$$。
**性质4：（有界闭区间上连续函数存在最大、最小值）**设$$f(x)$$在$$[a, b]上连续，则在[a, b]上必存在x_1，x_2，使得$$

$$f(x_1)=\displaystyle \max_{x\in[a, b]}f(x)（即\forall x\in [a, b],f(x)\leqslant f(x_1)）,$$
$$f(x_2)=\displaystyle \min_{x\in[a, b]}f(x)（即\forall x\in [a, b],f(x)\geqslant f(x_2)）。$$


