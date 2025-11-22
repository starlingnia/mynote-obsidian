##note 威腾23年##

##### The Reeh-Schlieder 定理

1.考虑一个D维闵可夫斯基时空 $M_D$ 下的量子场论，时空的坐标用 $x^\mu=(t,\vec{x})$ ，度规选择为$ds^2=-dt^2+d\vec{x}^2$.我们用$\Omega$表示真空态，用$H_0$表示从该基态用场算符产生的所有态构成的希尔伯特空间.注意到$H_0$并不是理论的所有态构成的那个希尔伯特空间$H$,比如理论可能允许不同的基态从而需要做一个超选择.

为了简化，首先考虑厄米标量场算符 $\phi(x^\mu)$,这里的场是不是基本粒子不会影响接下来的讨论，我们可以将场算符做一个光滑的求和，$\int{\rm d}^Dxf(x)\phi(x)$记作场算符$\phi_f(x)$,$f$可以为任意光滑的函数.则，生成$H_0$的充分的场算符的形式为  $|\Phi_\vec{f}>=\phi_{f_1}\phi_{f_2}...\phi_{f_n}|\Omega>$.任意的$H_0$中的态都可以表示为 $|\Phi_\vec{f}>$ 的线性组合。

reeh-schlieder定理说明，为了生成$H_0$，我们并不需要整个时空流形作为定义域的函数的集合{$f$}，甚至不需要以某个类空的超曲面为定义域。

对于时空流形上的波函数，我们总是可以对它做一个傅里叶变换，在时间平移对称性满足的情况下，傅里叶变换中$t$的共轭动量便是一个良好定义的哈密顿量H，H总是以某种形式被等时面上的物理信息给定，然后系统又按照H进行演化。即便一般流形情形下平移对称性可能不存在，但是傅里叶变换后$t$的共轭动量，我们依然认为它会被某个类空超曲面给定并决定系统接下来的演化。因此我们认为只需要靠定义在流形的某个完备的类空超曲面$\Sigma$的函数 $f_i$ 构造出生成 $H_0$ 的态。在严谨的数学语言中，这意味着$f_i$在$\Sigma$的每个邻域$U_i$内都已确定。

而Reeh-Schlieder定理给了更加强力的限制，我们只需要在时空流形的某个同维子空间上的函数$f_i$的集合，就足够充分地生成$H_o$，用严谨点的语言与前面的图像来说，就是我们只需要一个任意的很小的开集 V $\subset\Sigma$ ,以及一个V的很小的邻域 $U_V$.在 $U_V$上的函数 $f_i$ 便足够充分的生成希尔伯特空间$H_0$了.

2.想要证明RS定理，只需要思考它的反例。即，存在一些非零态 $\ket\chi$,他正交于所有用邻域$U_V$的函数$f_i$构造的态。即有：
$$
<\chi|\Psi_{\vec{f}}>=0 \Leftrightarrow <\chi|\phi(x_1)\phi(x_2)\cdot\cdot\cdot\cdot\cdot\cdot\phi(x_n)|\Omega>=0
$$

接下来证明 $\phi(x_1,x_2,...,x_n)=\bra\chi\phi(x_1)\phi(x_2)...\phi(x_n)\ket\Omega$ 如果在 $U_V$ 上为0，则最终对于闵可夫斯基时空来说，它在整个流形上任意取点的值为0.通过定义函数 $g(u)=\bra\chi\phi(x_1)\phi(x_2)\cdot\cdot\cdot\cdot\cdot\cdot\phi(x_n+ut)|\Omega>$ ,$t$ 为时间的方向单位矢量。

从$g(u)=\bra\chi\phi(x_1)\phi(x_2)\cdot\cdot\cdot\cdot\cdot\cdot exp(iHu)\phi(x_n)|\Omega>$ 的全纯形式得到 $g(u)$ 为0（？）.

依此类推，$x_i$ 也可以做一样的拖动，只需要影响第i个场算符时把其余场算符（i到n）一同拖动，从而出现全纯的算符 $exp(iHu)$ ,由于任何坐标变换总可以分解成同时对某些点做拖动，所以我们可以让 $\phi(x_1,x_2,...,x_n)$ 的变量{$x$}遍布闵可夫斯基时空流形.如此一来，整个流形上能满足条件的 $\ket\chi$ 就只剩下0，因为他与所有态的内积都为0.

2.3.有界的能动张量的矢量

定义算符 $\hat a$,在一个 $V$ 的邻域 $U_V$上.物理上，他和另一个类空隔离的时空区域 $\tilde V$的场算符不能够有物理量层面的关联，即他们的对易子都为0. $[\phi(x),a]=0,x\in U_\tilde V$ .反过来，即 $[\phi(x),\tilde a]=0,x \in U_V$.

一个惊奇的结论是，由于 $\hat a$与场算符对易，如果  $\hat a$ 湮没了基态，他也会湮没态  $\phi(x_1)\phi(x_2)\cdot\cdot\cdot\cdot\cdot\cdot\phi(x_n)\ket \Omega$ ，而由RS定理，这种算符将等价于0.因为左乘任何非零的态，振幅最后都是0，而 $U_V$可以是流形中任意的小邻域，我们可以说 $\hat a$湮没了所有的态，等价于0.

注意到产生湮没算符并不是这种情况，因为他们并不与场算符对易. 

从wightman函数来看，上述结论在闵可夫斯基时空的成立应该是可以接受的.因为任意两个坐标本征态的点的波函数之间，他们有着不为0的内积 $\bra\Omega\phi(x_1)\phi(x_2)\ket\Omega=\int\frac{{\rm d}^{D-1}k}{2 \omega_k}e^{ik(x_1-x_2)}$ ，因此这些本征态之间并不正交.

2.5中的一些重点： $\hat a\ket\Omega$ 在某个开集 $\tilde V$ 包含“月”，而 $\hat a$ 为邻域 $U_V$ 的算符.我们定义判断算符M，他是“月” 的个数的算符.则有 $\bra \Omega\hat M\ket\Omega=0,\bra\Omega\hat a^\dagger\hat M\hat a\ket\Omega\approx1$ ，我们可以让M在邻域 $U_{\tilde V}$ 上，则由于两个分隔邻域的算符必须对易，有 $\bra\Omega\hat M\hat a^\dagger\hat a\ket\Omega\approx1$ ，所以 $\hat a$ 必定不能是幺正算符.

由此，类空间隔的邻域上的幺正算符不会改变可观测物理量，这让系统是自洽的.同时，我们看到存在量子关联 $\bra\Omega\hat M\hat a^\dagger\hat a\ket\Omega\approx1\neq$ $\bra\Omega\hat M\ket\Omega\bra\Omega\hat a^\dagger\hat a\ket\Omega$ .不同区域的算符关联纠缠在一次但是没有可观测量的关联.

定义：对于希尔伯特空间 $H_0$ 的矢量 $\Psi$ ，若满足对于任意算符  $\hat a\in A_U$ ， $a\ket \Psi=0$ 等价于 $\hat a=0$ ,其中A表示在闵可夫斯基时空的同维子空间U上的算符的代数集合，则称态 $\Psi$ 和代数 $A_U$ 是分离的；若对于任意算符 $\hat a\in A_U$ ，态 $a\ket \Psi$ 的集合在 $H_0$ 上是稠密的，则称态 $\Psi$ 是一个 cyclic 矢量.注意到基态对于所有代数都是既分离又cyclic的，同时一个态对一个代数来说是 cyclic 的意味着它与其他分隔的邻域的代数是分离的.

一个结论（？）：平移群变换是全纯的作用的态矢量对于两个邻域的代数来说都是既分离又cyclic的.       ？ ${\rm exp}iPc$ 对于c来说是全纯的（解析的）.

加入费米型算符后，定义 $\psi_f=\int {\rm d}^Dxf(x)\psi(x)$ ， $\psi$ 是复数型费米子，所以又 $\psi_f\psi_f=0$ .对于费米子算符来说所有 $\psi_f \chi$ 的态都会被 $\psi_f$ 湮没.对于费米子构成的玻色型算符 $O_{f,g}=\psi_f\psi_g$ ，同样，他会湮没所有 $O_{f,g}\chi$ 形式的态.我们有：对于定义在U邻域的算符 $\psi_f,O_{f,g}$ ，有，态 $\psi_f\chi,O_{f,g}\chi$ 都不与代数 $A_U$ 分离（总有不为0的算符湮没掉态），也不对另一个邻域的代数 $A_\tilde U$  来说cyclic.

一个结论，若U与 $U’$ 为类空间隔下完备的，即他们的并是整个类空区域.则，他们的代数就是与对方代数对易的最大的集合.称为Haag对偶.

##### RT算符

Tomita算符定义：对于态 $\Psi$ (与代数 $A_U、A_\tilde U$ 分离且cyclic）的反线性Tomita算符 $\hat S_\Psi$ ，定义为 $\hat S_\Psi\hat a\ket\Psi=\hat a^\dagger\ket\Psi, a\in A_U$ .

Tomita算符是无界的，因为上述定义式要在任意趋近于湮没算符 $\hat a$ 的算符 $\hat a+\delta$ 下成立，此时其共轭将任意趋近于产生算符，所以 $\hat S_\Psi$ 是无界的.无界算符并不能在希尔伯特空间的所有态上良好定义.                              

拓展Tomita算符的定义：若存在序列 $\hat a_n\in A_U$ ，其极限 $x=\lim\limits_{n\rightarrow\infty}\hat a_n\ket\Psi、y=\lim\limits_{n\rightarrow\infty}\hat a^\dagger\ket\Psi$ 存在，则定义的Tomita算符满足 $S_\Psi x=y$  ，显然， $S_\Psi^2=1$.

对于反线性算符的共轭定义为 $\bra\chi\ket {S^\dagger\gamma}\equiv\bra\gamma\ket{S\chi}$ .Tomita算符的共轭正是与 $A_U$ 对易的代数 $A_{\tilde U}$ 定义的Tomita算符 $S’_\Psi$ .

$$
\bra{S’_\Psi a’\Psi}\ket{a\Psi}=\bra{a’^\dagger\Psi}\ket{a\Psi}=\bra\Psi\ket{a’a\Psi}=\bra\Psi\ket{aa’\Psi}=\bra{a^\dagger\Psi}\ket{a’\Psi}=\bra{S_\Psi^\dagger a’\Psi}\ket{a\Psi}
$$
我们可以对 $S_\Psi$ 做唯一的径向分解 $S_\Psi=J_\Psi\Delta_\Psi^{1/2}$ .

$J_\Psi$ 是反幺正的，叫模共轭，而 $\Delta_\Psi$ 是厄密且正定的.我们有 $\Delta_\Psi=S_\Psi^\dagger S_\Psi$ ，叫模算符.

对于 $\Psi$ 来说，模算符作用相当于1， $f(\Delta_\Psi)\ket\Psi\equiv f(1)\ket\Psi$ .

注意到, $S_\Psi^2=1\leftrightarrow J_\Psi\Delta_\Psi^{1/2}J_\Psi\Delta_\Psi^{1/2}=1$ ,即 $\Delta_\Psi^{-1/2}=J_\Psi\Delta_\Psi^{1/2}J_\Psi$ . 又 $J^2_\Psi(J^{-1}_\Psi\Delta_\Psi^{1/2}J_\Psi)=1\cdot\Delta_\Psi^{-1/2}$ ,由于 $J^{-1}_\Psi\Delta_\Psi^{1/2}J_\Psi$ 也是 $\Delta_\Psi^{-1/2}$ 一种正定的分解，我们要求两种分解相等，即模共轭与Tomita算符一样是自身的逆.

$S’_\Psi=S^\dagger_\Psi=\Delta_\Psi^{1/2}J_\Psi=J_\Psi\Delta_\Psi^{-1/2}=J’_\Psi\Delta_\Psi’^{1/2}$ ,因此模算符互相为逆，而模共轭对于不同代数是相等的.

$J_\Psi\Delta_\Psi J_\Psi =J_\Psi\Delta_\Psi^{1/2}J_\Psi J_\Psi^{-1}\Delta^{1/2}_\Psi J_\Psi=\Delta^{-1}_\Psi$ .

RT算符（相对性Tomita算符）定义为: $S_{\Psi|\Phi}a\ket\Psi=a\ket\Phi$ ,第二个态 $\Phi$ 可以是任意态，但是只有其实分离且cyclic时才存在逆变换 $S_{\Phi|\Psi}$ .

$S_{\Phi|\Psi}S_{\Psi|\Phi}=1$ .所有态都是取归一化到内积为1的.

T算符的许多性质都继承到RT算符中：$S’_{\Psi|\Phi}=S^\dagger_{\Psi|\Phi}、S_{\Psi|\Phi}=J_{\Psi|\Phi}\Delta_{\Psi|\Phi}^{1/2}、\Delta_{\Psi|\Phi}=S^\dagger_{\Psi|\Phi}S_{\Psi|\Phi}$ .

注意到：对于幺正的算符 $\hat a’$ , $S_{\Psi|\hat a’\Phi}\hat a\Psi=\hat a^\dagger\hat a’\Phi=\hat a’\hat a^\dagger\Phi\rightarrow S_{\Psi|\hat a’\Phi}=\hat a’S_{\Psi|\Phi}$ （不需要幺正） $\Delta_{\Psi|a’\Phi}=\Delta_{\Psi|\Phi}$ （需要幺正）.

$\bra{\hat a^\dagger\Psi}\Delta_{\Psi|\Phi}\ket{\hat b\Psi}=\bra{\hat b^\dagger\Phi}\ket{\hat a\Phi}$ .

RT算符要特别注意定义的代数是哪个，可以通过下标邻域区分.

###### 相对熵：

某个区域U的两个态间的相对熵，定义为 $S_{\Psi|\Phi}(U)=-\bra\Psi \log\Delta_{\Psi|\Phi}\ket\Psi$ .即负的对这区域的代数的相对模算符做log求迹.如果说 $\Phi$ 与代数不分离，则RT模算符会有为0的本征值，从而得到无穷大的相对熵.如果态 $\Phi=a’\Psi$ ，差一个其他区域的幺正变换，则相对熵会为0，因为RT模作用在第一个态 $\Psi$ 上会为1( $\Delta_{\Psi|a’\Psi}=\Delta_{\Psi|\Psi}=\Delta_\Psi$ ).或者说相对熵此时为0的性质要求RT模延续之前在第一态上为1的性质.

非负性：$S_{\Psi|\Phi}(U)>\bra\Psi(1-\Delta_{\Psi|\Phi})\ket\Psi=\bra\Psi\ket{\Psi}-\bra\Phi\ket{\Phi}=1-1=0$ .

注意到由：$\bra\chi\ket{\Delta_{\Psi|\Phi}\Psi}=\bra\chi\ket{\Psi}$ , $\bra{a\Psi}\ket{\Delta_{\Psi|\Phi}\Psi}=\bra\Phi\ket{S_{\Psi|\Phi}a\Psi}=\bra\Phi\ket{a^\dagger\Phi}=\bra{a\Psi}\ket{\Psi}=\bra{a\Phi}\ket{\Phi}$ .

意味着 $\bra{a\Psi}\ket{b\Psi}=\bra{a\Phi}\ket{b\Phi}$ ,这种性质相当于两个态间差别一个其他代数的幺正变换 $\Phi=a’\Psi$ .这与前面相对熵为0的情形相符.

######  相对熵的单调性

$\tilde U\subset U,S_{\Psi|\Phi}(U)\ge S_{\Psi|\Phi}(\tilde U)$ .这等价于要求 $\tilde U$ 的RT模算符大于 $U$ 的RT模算符.

我们定义 $P\ge Q:\bra\chi\frac{1}{s+P}\ket\chi\le\bra\chi\frac{1}{s+Q}\ket\chi$ .这种定义适用于无界的算符.

###### 厄密形式

模算符对应了厄密形式 $F(\chi,\eta)=\bra{S\chi}\ket{S\eta}=\bra{S^\dagger S\eta}\ket{\chi}$ .以外导数为例，我们定义紧致的区域M，其边界为 $\partial M\equiv N$ ，对于其上的连续函数 $\phi$ ，算符 $\rm d$ 会将他映射到一个1-形式 . 但是这种外导数有两种版本，一种是 $\rm \hat T_0$ ,它要求函数在边界上为0；一种是 $\rm \hat T_1$ ,它对函数在边界上的取值没有限制.

对应的厄密形式为 $F_0(\phi,\rho)=\bra{T_0\phi}\ket{T_0\rho}=\int_M{\rm d}^nx\partial^i\bar\phi\cdot\partial_i\rho 、F_1(\phi,\rho)=\bra{T_1\phi}\ket{T_1\rho}=\int_M{\rm d}^nx\partial^i\bar\phi\cdot\partial_i\rho$ . 

对应的拉普拉斯算符定义为 $\Delta=\rm d^\dagger d=-\partial\cdot\partial$ ,我们想让 ${\rm T^\dagger T}\phi=\Delta\phi\rightarrow\int_M{\rm d^D}x(-\partial^i\partial_i\bar\phi)\rho=\int_M{\rm d^D}x\partial^i\bar\phi\partial_i\rho$ .这相当于分部积分.我们需要边界项 $\int_N{\rm d}\mu(-\partial_\bot\bar\phi)\rho$ 为0，其中 $\partial_\bot$ 为在N上的指向M内部的法向导数算符.为了让边界项消失，我们有两种边界条件可以选取，一种是让边界上的函数值为0的迪利克雷边界条件，定义的拉普拉斯算符为迪利克雷拉普拉斯算符，记作 $\Delta_{\rm D}$ .另一种是让垂直于边界的导数项为0的纽曼边界条件，定义的纽曼拉普拉斯算符记作 $\Delta_N$ .

为了证明 $\Delta_D\ge\Delta_N$ ,定义厄密形式 $G_\lambda(\phi,\rho)=\int_M{\rm d}^nx\partial^i\bar\phi\partial\rho+\lambda\int_N{\rm d}\mu\bar\phi\rho$ ,为了让它在某些函数上与普通拉普拉斯算符相等，我们需要边界N上的项 $\int_N{\rm d}\mu(-\partial_\bot\bar\phi+\lambda\bar\phi)\rho=0$ .注意到形式G对于变量 $\lambda$ 单调递增，而在变量等于0时为纽曼拉普拉斯子，在变量趋于无穷时为迪利克雷拉普拉斯子，由此便证明了不等式.

##### 有限维度的量子系统

我们考虑一个系统,它的希尔伯特空间 $H=H_1\bigotimes H_2$ ,我们发现作用在 $H_1$ 的线性算符代数  $A$ 有且只有一种对易的代数，即作用在 $H_2$ 上的代数 $A’$ ，前面的许多结论可以套到这两个代数上.任何态矢量可以做展开 $\psi=\sum_k c_k\psi_k\bigotimes\psi_k’$ ,展开的两组基矢量分别是两个希尔伯特空间的正交完备基矢量. 

当非0的 $c_k$ 对应的基矢量是完备的某个希尔伯特空间的基矢时，此时除了0外没有对应代数上的算符可以把所有矢量湮没为0，因此态矢量对这个代数是分离的，因而对另一个代数是cyclic的.

在这种情况下定义模算符：

对于 $A$ 来说的Tomita算符为： $S_\psi(({\rm \hat a\bigotimes1})\psi)=(\rm \hat a^\dagger\bigotimes1)\psi$ ，我们将算符 $\rm \hat a$ 的映射写出：${\rm \hat a}\ket i=\ket j、{\rm \hat a }\ket k=0(k\ne i)$ ,${\rm \hat a^\dagger}\ket j=\ket i$ 、 ${\rm\hat a^\dagger}\ket k=0(k\ne j)$ .   则有 $({\rm\hat a\bigotimes1})\psi=\sum_ic_i\ket{j(i)_a,i}、({\rm\hat a^\dagger\bigotimes 1})\psi=\sum_jc_j\ket{i(j)_{a^\dagger},j}$  ,由此得到
$$
S_\psi\sum_ic_i\ket{j(i)_a,i}=\sum_jc_j\ket{i(j)_{-1},j}\rightarrow S_\psi\ket{j,i}=\frac{c_j}{\bar c_i}\ket{i,j}$$$$
,S_\psi^\dagger\ket{i,j}=\frac{ c_j}{ \bar c_i}\ket{j,i}\\\Delta_\psi\ket{j,i}=\frac{c_j\bar c_j}{c_i\bar c_i}\ket{j,i}
$$
需要注意求共轭Tomita作用与模算符作用时，要用反线性算符规则对待共轭Tomita算符.

对应的模共轭为 $J_\psi\ket{j,i}=\sqrt{\frac{c_jc_i}{\bar c_j\bar c_i}}\ket{i,j}、\Delta^{1/2}_\psi\ket{j,i}=\sqrt{\frac{c_j\bar c_j}{c_i\bar c_i}}\ket{j,i}$ .

在引入第二个态 $\phi$ 后，我们定义相对的模算符.

###### 有限维度量子系统的相对熵

$$
S_{\psi|\phi}(({\rm\hat a\bigotimes1})\psi)=({\rm \hat a^\dagger}\bigotimes1)\phi\\\phi=\sum_{\alpha=1}^nd_\alpha\phi_\alpha\bigotimes\phi_\alpha’\\{\rm\hat a}\ket i=\ket\alpha,{\rm\hat a}\ket j=0(j\ne i)、$$$${\rm\hat a^\dagger}\ket\alpha=\ket i,{\rm\hat a^\dagger}\ket\beta=0(\beta\ne\alpha)\\{(\rm\hat a\bigotimes1)}\psi=c_i\ket{\alpha,i},({\rm\hat a^\dagger\bigotimes1})\phi=d_\alpha\ket{i,\alpha}$$$$S_{\psi|\phi}\ket{\alpha,i}=\frac{d_\alpha}{\bar c_i}\ket{i,\alpha},S_{\psi|\phi}^\dagger\ket{i,\alpha}=\frac{d_\alpha}{\bar c_i}\ket{\alpha,i}$$$$\Delta_{\psi|\phi}\ket{\alpha,i}=\frac{d_\alpha\bar d_\alpha}{c_i\bar c_i}\ket{\alpha,i}
$$

注意到上面对于算符的作用只考虑了两个态间的转变.

这些形式可以方便的转到密度矩阵上.重要的在于模算符的形式为 $\Delta_{\psi|\phi}=\sigma_1\bigotimes\rho_2^{-1}$ .

如此得到相对熵的密度算符形式 $S_{\psi|\phi;U}=-\bra\psi\log\Delta_{\psi|\phi;U}\ket\psi=-Tr_{12}\rho_{12}\log(\sigma_1\bigotimes\rho_2^{-1})$$Tr_{12}\rho_{12}\log\rho_2=Tr_2\rho_2\log\rho_2=Tr_1\rho_1\log\rho_1、$
$S_{\psi|\phi;U}=Tr_1\rho_1(\log\rho_1-\log\sigma_1)$
所以相对熵的大小在于两者约化密度矩阵的差别.























































































