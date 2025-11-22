---
tags: []
parent: ""
collections:
    - Note
version: 28153
libraryID: 1
itemKey: S78W9UVP

---
# LiteratureNote-Raha

${\rm{QM}}\ \alpha版本笔记$

\#框架

首先是描述一个系统选定自由度的数学对象 $q$ , 为了描述他的运动我们引入他的运动的对应自由度 $p$ ,称之为共轭动量

然后是导入一个括号乘法 ${\rm{[,]}}$ 和一个加减法, 构成一个代数 ,我们认定 $[q,p]=1$ .

要求莱布尼兹律 , 我们可以形式的写出 $[f(q),p]=\frac{\partial f(q)}{\partial q}$ , 现在我们要求在 $\{q,p\}$ 的相空间里规定演化 , 这应该由一个对象 $\mathcal{H}[q,p]$ 生成 .

$$
   \Omega : q \in \mathcal{A} \rightarrow [\cdot,q] \in vector \ , \       \frac{d}{dt} = \Omega\left(\mathcal{H}[p,q] \right)
$$

这便是我们规定的哈密顿正则方程 $\dot q = [q,\mathcal{H}]\ ,\ \dot p=[p,\mathcal{H}]$ ,

在经典表示下

这样的演化是保相空间体积的 , 其背后其实是我们要求物理体系演化到物理体系,存在一个流守恒的规律.

选定一个研究对象，提取出感兴趣的参量$q$ ，预言能力要求我们得到这些参量关于某个参数 $t$ 的函数 $q(t)$ ，

这个函数可能来自于各种各样的微分方程 $Function(q,\dot q, \ddot q , \dots )=0$ ， 不过，足够一般的，我们可以认为他会被一个一阶微分方程完全确定，

$I(q,\dot q)=0 \rightarrow q(t)$

并且 $I$ 的形式与参数t无关.

即，在以 $\{ q, \dot{q}\}$ 为坐标的空间内的一条曲线将唯一的给定函数 $q(t)$

（认定曲线的某个端点为 $t=0$ ）.

将这个过程一般化，以消除 ${q,\dot{q}}$中关于参数 $t$的冗余（即，当时钟

的尺度被改变时物理描述依然不变 $t \rightarrow \Gamma t$） ，引入新的参量

$p$ ，其与q一样，在将 $t$ 放缩时不变.取而代之的问题是， ${p,q}$ 组成的

相空间内的一条曲线并不足以唯一的确定 $q(t)$的形式，而是还需要 $p,q$的关系.

一般性的，我们需要的 $I(q,\dot{q})=0 \text{与} F(p,q,\dot{q})=0$ ，可以被形变为

$\dot{q}=\partial_{p}{H[p,q]} ,\ \dot{p}=-\partial_{q}{H[p,q]}$

与此相对应的，在求解出2d个方程前，我们并不能严格的确定相空间的初始末尾两端.

得到一个不含时的哈密顿量 $H[p,q]$后，此时可以说，我们构建了一个能量守恒的系统了.

如果一开始的 $I(q,\dot{q})$ 就含时，应该改为 $I(q,\dot{q},t)$ ，则一般来说

我们后面引入的 $F(p,q,\dot q,t)$也会含时，最后的方程变为含时理论：

$\dot{q}=\partial_{p}{H[p,q,t]} ,\ \dot{p}=-\partial_{q}{H[p,q,t]}$

这样的理论在我们的框架下被诠释为能量不守恒的，或者说是开放的系统.

所谓的物理学理论，就是以这套范式为基础工具研究不同系统.

1.

我们来看看这样的范式，是如何在改变时钟标度时用同样的叙述解决问题的：

$$

\dot{p}|_{\Gamma t}= -\partial_{q}{H_{\Gamma t}},\

\dot{q}|_{\Gamma t}= \partial_{p}{H_{\Gamma t}}

$$

运动方程有关系：

$$

\dot{p}|_{\Gamma t}= -\frac{1}{\Gamma }\partial_{q}{H_{ t}},\

\dot{q}|_{\Gamma t}= \frac{1}{\Gamma }\partial_p{H_{ t}}

$$

即，只需要将哈密顿量，也就是系统的能量重新定标一下即可，整个系统在时钟重定标下的

不变性是显化的.

2.

正则方程背后总是对应着某个极值曲线问题.

$S[p,q]= \int^A_B dt \left( p \dot{q}-H[p,q]\right)$

其中 $A,B$  表示确定两端的 $q,p$ 值.

$$
\delta S = \int dt \left( \delta p \left( \dot{q}-\partial_{p} H 
\right)-\delta q \left( \dot{p}+\partial_{q} H  \right)
 \right)   +\int d(p \delta q)
$$

   我们只需要固定两端的 $q$值即可由极值曲线导出正则运动方程.

3\.   当我们追求更精确的预言能力时，将不得不考虑参量是什么类型的数学对象的问题.   为此先将前面的讨论尽力的抽象化为一个代数结构，所谓的量子原理，便是“我们应该 将这些物理对象用某个泛函空间的广义线性变换表示”.   将正则运动方程改写为形式：   $\frac{dx^i}{dt}=\omega^{ij}\partial_jH[x]$   其中 $w^{ij}= \begin{bmatrix}      0 & I \\   -I & 0 \end{bmatrix} =J$     不难想到，正则共轭的结构实际上是在相空间 $\\{p,q\\}$ 上加入一个二形式: $\omega =w_{ij}dx^i \wedge dx^j = \sum_a dp^a\wedge dq^{\bar a}$ $\rightarrow \omega =dp \wedge dq$ $w_{ij}=J^{-1}$   这个二形式定义了一套代数 $[m,n]=w^{ij}\partial_im \partial _jn$   我们可以正式的在相空间的几何的意义上写出正则共轭对应的代数结构：  

$p^\prime =ip,\ [q,p^\prime ]=i,\ p^\prime \rightarrow -i \partial _q$

同样的,
