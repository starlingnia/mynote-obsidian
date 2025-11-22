弦论note：

###### 基本的弦的形式

$$
e^{iS}\text{，}S_M=-\frac{T}{2}\int{\text{d}\sigma^2}\sqrt{-g}\partial _{\alpha}X^{\mu}\partial ^{\alpha}X_{\mu}
$$

$$
\sigma ^{0,1}\,\,\in \left[ -\infty ,\infty \right] ,\left[ 0,l \right]
$$
$$
z=\exp \left[ \frac{2\pi i}{l}\left( \sigma ^0-\sigma ^1 \right) \right] ,\bar{z}=\exp \left[ \frac{2\pi i}{l}\left( \sigma ^0+\sigma ^1 \right) \right]
$$
$$
Wick\ rotation:\ \ \ \ \ \tau =i\sigma ^0,
$$
$$
z=\exp \left[ \frac{2\pi}{l}\left( \tau -i\sigma ^1 \right) \right] ,\bar{z}=\exp \left[ \frac{2\pi}{l}\left( \tau +i\sigma ^1 \right) \right] .
$$

对于开弦，不要求周期性条件，则 $z=\exp[\frac{\pi i}l(\sigma^0-\sigma^1)]$ .

以z为变量写的式子，最后的结果将于选取的世界面空间部分的区间长度 $l$ 无关.

转动到欧几里得形式后，我们一般会定义新的欧几里得形式的作用量 $S_E=-iS_M$ ,
$$
S_E=\frac{T}{2}\int{\text{d}\sigma \text{d}\tau}\sqrt{\delta}\ \partial _iX^{\mu}\partial ^iX_{\mu},
$$
我们总是可以做坐标变换更改度规，由于使用的都是不变量，形式在各自各自体系下不会有变化.
$$
T_{\alpha \beta}=\frac{4\pi}{\sqrt{-g}}\frac{\delta S_M}{\delta g^{\alpha \beta}}=-\frac{1}{\alpha}\left( \partial _{\alpha}X^{\mu}\partial _{\beta}X_{\mu}-g_{\alpha \beta}\partial _{\gamma}X^{\mu}\partial ^{\gamma}X_{\mu} \right)
$$
$$
=-\frac{4\pi}{\sqrt{\delta}}\frac{\delta S_E}{\delta \ \delta ^{\alpha \beta}}=-\frac{1}{\alpha}\left( \partial _{\alpha}X^{\mu}\partial _{\beta}X_{\mu}-\delta _{\alpha \beta}\partial _{\gamma}X^{\mu}\partial ^{\gamma}X_{\mu} \right) .\\T=\frac{1}{2\pi\alpha}
$$

能动张量在坐标变换下以张量形式变化，包括维克转动.

特别的，在z的形式下，T将可以进行展开，展开的系数恰好是物理约束.
$$
T\left( z \right) =T_{zz}=-\frac{1}{\alpha}\partial_zX\partial_zX=\sum_{-\infty}^{\infty}{L_mz^{-m-2}}
$$
$$
\bar{T}\left( \bar{z} \right) =\bar{T}_{zz}=-\frac{1}{\alpha}\partial_{\bar z}X\partial_{\bar z}X=\sum_{-\infty}^{\infty}{\tilde{L}_m\bar{z}^{-m-2}}
$$


我们可以选择在 $z$ 下发现弦运动模式的分解.
$$
S_M=-\frac{T}{2}\int{\text{d}z\text{d}\bar{z}}\cdot \frac{1}{2}\left( \frac{l}{2\pi} \right) ^2\frac{1}{z\bar{z}}\cdot \left( \begin{matrix}
	0&		2\left( \frac{2\pi}{l} \right) ^2z\bar{z}\\
	2\left( \frac{2\pi}{l} \right) ^2z\bar{z}&		0\\
\end{matrix} \right) _{z,\bar{z}}\cdot \left( \begin{matrix}
	\partial _zX\cdot \partial _zX&		\partial _zX\cdot \partial _{\bar{z}}X\\
	\partial _{\bar{z}}X\cdot \partial _zX&		\partial _{\bar{z}}X\cdot \partial _{\bar{z}}X\\
\end{matrix} \right)
$$
$$
=-T\int{\text{d}z\text{d}\bar{z}}\cdot \partial _zX\cdot \partial _{\bar{z}}X
$$
$$
h_{\alpha \beta}=\left( \begin{matrix}
	0&		\frac{1}{2}\left( \frac{l}{2\pi} \right) ^2\frac{1}{z\bar{z}}\\
	\frac{1}{2}\left( \frac{l}{2\pi} \right) ^2\frac{1}{z\bar{z}}&		0\\
\end{matrix} \right) _{z,\bar{z}}
$$
$$
\frac{\delta S_M}{\delta X^{\mu}}=-2T\partial \bar{\partial}X_{\mu}=0,
$$

如果是在欧几里得形式下看这个式子，我们将会得到这意味着X能够分解为全纯的与非全纯的两部分.
$$
S_E=\frac{T}{2}\int{\text{d}z\text{d}\bar{z}}\cdot \frac{1}{2}\left( \frac{l}{2\pi} \right) ^2\frac{1}{z\bar{z}}\cdot \left( \begin{matrix}
	0&		2\left( \frac{2\pi}{l} \right) ^2z\bar{z}\\
	2\left( \frac{2\pi}{l} \right) ^2z\bar{z}&		0\\
\end{matrix} \right) _{z,\bar{z}}\cdot \left( \begin{matrix}
	\partial _zX\cdot \partial _zX&		\partial _zX\cdot \partial _{\bar{z}}X\\
	\partial _{\bar{z}}X\cdot \partial _zX&		\partial _{\bar{z}}X\cdot \partial _{\bar{z}}X\\
\end{matrix} \right) 
$$
$$
=T\int{\text{d}z\text{d}\bar{z}}\cdot \partial _zX\cdot \partial _{\bar{z}}X
$$
$$
\delta _{\alpha \beta}=\left( \begin{matrix}
	0&		\frac{1}{2}\left( \frac{l}{2\pi} \right) ^2\frac{1}{z\bar{z}}\\
	\frac{1}{2}\left( \frac{l}{2\pi} \right) ^2\frac{1}{z\bar{z}}&		0\\
\end{matrix} \right) _{z,\bar{z}}
$$
$$
\frac{\delta S_M}{\delta X^{\mu}}=-2T\partial \bar{\partial}X_{\mu}=0,
$$

我们将弦的运动分解为各种模：

对于开弦（最大NN条件）：
$$
X^{\mu}=x^{\mu}-i\sqrt{\frac{\alpha}{2}}\alpha _0^{\mu}\ln \left( z\bar{z} \right) +i\sqrt{\frac{\alpha}{2}}\sum_{-\infty ,n\ne 0}^{\infty}{\frac{\alpha _n^{\mu}}{n}\left( z^{-n}+\bar{z}^{-n} \right)}
$$
$$
X^{\mu}=x^{\mu}-i\alpha p^{\mu}\ln \left( z\bar{z} \right) +i\sqrt{\frac{\alpha}{2}}\sum_{-\infty ,n\ne 0}^{\infty}{\frac{\alpha _n^{\mu}}{n}\left( z^{-n}+\bar{z}^{-n} \right)}
$$

对于闭弦：
$$
X^{\mu}=x^{\mu}-i\sqrt{\frac{\alpha}{2}}(\alpha _{0}^{\mu}\ln z+\tilde{\alpha}_0^\mu\ln\bar{z})+i\sqrt{\frac{\alpha}{2}}\sum_{-\infty ,n\ne 0}^{\infty}{\frac{\alpha _{n}^{\mu}z^{-n}+\tilde{\alpha}_{n}^{\mu}\bar{z}^{-n}}{n}}
$$
$$
X^{\mu}=x^{\mu}-i\frac{\alpha}{2}p^\mu(\ln z+\ln\bar{z})+i\sqrt{\frac{\alpha}{2}}\sum_{-\infty ,n\ne 0}^{\infty}{\frac{\alpha _{n}^{\mu}z^{-n}+\tilde{\alpha}_{n}^{\mu}\bar{z}^{-n}}{n}}
$$

以闭弦右模举例：
$$
X_R^{\mu}=\frac{x^{\mu}}{2}+\frac{2\pi}{l}\sqrt{\frac{\alpha}{2}}\alpha _{0}^{\mu}\left( \sigma ^0-\sigma ^1 \right) +i\sqrt{\frac{\alpha}{2}}\sum_{-\infty ,n\ne 0}^{\infty}{\frac{\alpha _{n}^{\mu}\exp \left[ -\frac{2\pi in}{l}\left( \sigma ^0-\sigma ^1 \right) \right]}{n}}
$$

$$
\partial _-X_R=\frac{2\pi i}{l}z\partial _zX_R=\frac{2\pi}{l}\sqrt{\frac{\alpha}{2}}\sum_{-\infty}^{\infty}{\alpha _{n}^{\mu}z^{-n}},\alpha _{0}^{\mu}=\frac{l_s}{2}p^{\mu}
$$

$$
T_{--}=-\frac{1}{\alpha}\partial _-X_R\partial _-X_R=-\left( \frac{2\pi}{l} \right) ^2\frac{1}{2}\sum_{-\infty}^{\infty}\alpha _{m}^{\mu}\alpha _{n-m,\mu}z^{-n}=-\left( \frac{2\pi}{l}
 \right) ^2\ zz\ \partial _zX_R\partial _zX_R
$$
$$
=-\left( \frac{2\pi}{l} \right) ^2\sum_{-\infty}^{\infty}{L_nz^{-n}}
$$

$$
H=\int_0^l\text{d}\sigma ^1\left( \dot{X}\cdot P-\mathscr{L} \right)=\int_0^l{\text{d}}\sigma ^1\left( \dot{X}\cdot T\dot{X}-\frac{T}{2}\left( \dot{X}^2-X’^2 \right) \right)
$$
$$
=T\int_0^l{\text{d}}\sigma ^1\left( \partial _+X_L\partial _+X_L+\partial _-X_R\partial _-X_R \right) 
$$
$$
=-\frac{1}{2\pi}\int_0^l{\text{d}}\sigma ^1\left( T_{--}+T_{++} \right) =\frac{2\pi}{l}\left( L_0+\tilde{L}_0 \right)
$$

实际上，我们可以带个普遍的常数k，对于开弦取1，并让左右模相等；对于闭弦取 $\frac{1}2$ .
$$
\alpha _{0}^{\mu}=kl_sp^{\mu}=\sqrt{k^2\frac{\alpha}{2}}p^{\mu}
$$
$$
\partial _-X\partial _-X=\left( \frac{\pi i}{kl} \right) ^2zz\,\,\partial _zX\partial _zX=\alpha \left( \frac{\pi}{kl} \right) ^2\sum_{-\infty}^{\infty}{L_nz^{-n}}
$$
$$
T_{--}=-\left( \frac{\pi}{kl} \right) ^2\sum_{-\infty}^{\infty}{L_nz^{-n}}
$$
$$
H=T\int_0^l{\text{d}}\sigma ^1\left( \partial _+X\partial _+X+\partial _-X\partial _-X \right) 
$$
$$
=-\frac{1}{2\pi}\int_0^l{\text{d}}\sigma ^1\left( T_{--}+T_{++} \right) =\frac{\pi}{2k^2l}\left( L_0+\tilde{L}_0 \right) =\left\{ \begin{array}{l}
	\frac{2\pi}{l}\left( L_0+\tilde{L} \right)\\
	\frac{\pi}{l}L_0\\
\end{array} \right.
$$

接下来，写下量子层面的代数：
$$
\left[ L_m,L_n \right] =\frac{1}{2}\left[ \sum_{-\infty}^{\infty}{:\alpha _p\cdot \alpha _{m-p}:},L_n \right] =\frac{1}{2}\sum_{p<\frac{m}{2}}{\left( \alpha _p\left[ \alpha _{m-p},L_n \right] +\left[ \alpha _p,L_n \right] \alpha _{m-p} \right)}+
$$
$$
\frac{1}{2}\sum_{p>\frac{m}{2}}{\left( \left[ \alpha _{m-p},L_n \right] \alpha _p+\alpha _{m-p}\left[ \alpha _p,L_n \right] \right)}.
$$
$$
\left[ \alpha _m,L_n \right] =\frac{1}{2}\sum_{-\infty}^{\infty}{\left( \alpha _p\left[ \alpha _m,\alpha _{n-p} \right] +\left[ \alpha _m,\alpha _p \right] \alpha _{n-p} \right)}=m\alpha _{m+n}
$$
$$
\left[ L_m,L_n \right] =\frac{1}{2}\sum_{p<\frac{m}{2}}{\left( \left( m-p \right) \alpha _p\alpha _{m-p+n}+p\alpha _{p+n}\alpha _{m-p} \right) +}
$$
$$
\frac{1}{2}\sum_{p>\frac{m}{2}}{\left( \left( m-p \right) \alpha _{m-p+n}\alpha _p+p\alpha _{m-p}\alpha _{p+n} \right)}=\left( m-n \right) L_{m+n}+\delta _{m+n}\frac{cm\left( m+1 \right) \left( m-1 \right)}{12}\ \ ?
$$

这也可以通过能动张量的计算得到，在CFT中，OPE是更需要被聚焦的形式：

路径积分式的守恒：
$$
\int{D\left[ \phi \right] O\left[ \phi \right] e^{-S}}=\int{D\left[ \phi \right] O\left[ \phi \right] \exp \left( -S-\frac{1}{2\pi i}\int{\text{d}^DxJ^{\alpha}\partial _{\alpha}\epsilon} \right)}
$$
$$
\delta \left< \left. O \right> \right. =\frac{1}{2\pi i}\left< \left. \partial _{\alpha}J^{\alpha}O \right> =0 \right.
$$

对X求Ward等式，我们可以得到
$$
\delta ^2\left( z-w,\bar{z}-\bar{w} \right) \left[ **\frac{\delta X\left( z \right)}{\delta X\left( w \right)} \right] -\int{\text{d}^2z_1}X\left( z \right) \frac{\delta \left( \frac{1}{2\pi \alpha}\partial _{z_1}X\left( z_1,\bar{z}_1 \right) \partial _{\bar{z}_1}X\left( z_1,\bar{z}_1 \right) \right)}{\delta X\left( w \right)}=0
$$
$$
\delta ^2\left( z-w,\bar{z}-\bar{w} \right) =-\frac{1}{\pi \alpha}X\left( z \right) \partial \overline{\partial }X\left( w \right) 
$$
$$
\partial \overline{\partial }\left< \left. X\left( z \right) X\left( w \right) \right> \right. =-\pi \alpha \delta ^2\left( z-w,\bar{z}-\bar{w} \right) 
$$
$$
\partial \overline{\partial }\ln \left( z-w \right) ^2=2\pi \delta ^2\left( z-w,\bar{z}-\bar{w} \right) 
$$
$$
\left< \left. X\left( z \right) X\left( w \right) \right> \right. =-\frac{\alpha}{2}\ln \left( z-w \right) ^2
$$

让我们把这个命名为场的contraction.

则，我们可以对任意的算符乘积，注意是不含路径积分的算符乘积代数，做展开.以X为例.
$$
X^{\mu}\left( z,\bar{z} \right) X^{\nu}\left( w,\bar{w} \right) =:X^{\mu}\left( z,\bar{z} \right) X^{\nu}\left( w,\bar{w} \right) :-\eta ^{\mu \nu}\frac{\alpha}{2}\ln \left( z-w \right) ^2
$$
单独把contraction写出来，显然是一个可以很普遍的进行的操作，在CFT中，当 $z$ 与 $w$ 互相靠的很近很近时（实际上，有效的范围如果认为是级数收敛的范围，那么将是可以非常大的），我们可以把留下的非极点且在重合时不消失的项，等作自然排序在此时的值.
$$
A\left( z \right) B\left( w \right) =\sum_{n=-\infty}^N{\frac{AB_n\left( w \right)}{\left( z-w \right) ^n}}=:A\left( z \right) B\left( w \right) :+contraction
$$

$$
:A\left( z \right) B\left( z \right) :=AB_0\left( z \right) ,\ \ :A\left( z \right) B\left( w \right) :=\sum_{k\ge 0}^N{AB_k\left( w \right) \left( z-w \right) ^k}
$$

并且他在自由理论中正是湮没在右产生在左的排序，在路径积分中将给出0的值（并不意味着都会湮没所有态）.

###### FP鬼场做BRST

接下来引入鬼场：
$$
\int{D\left[ X,h^g \right] \exp \left( -S\left[ X,h^g \right] \right)}=\int{D\left[ B \right] \exp \left( -iBF \right)}\int{D\left[ X,h^g \right] \delta \left( F\left( g \right) \right) \text{Det}\left( \frac{\delta F}{\delta g} \right) \exp \left( -S\left[ X,h^0 \right] \right)}
$$
$$
=\int{D\left[ X,h^g,c,b,B \right] \exp \left( -S\left[ X,h^0 \right] -\frac{1}{2\pi \alpha}\int{\text{d}^Dx\ b\frac{\delta F}{\delta g}c}-iBF\left( h \right) \right)}
$$
$$
=\int{D\left[ X,h^g,c,c^{\left( 1 \right)},b,B \right] \exp \left( -\frac{1}{2\pi \alpha}\int{\text{d}^2z}\partial X\overline{\partial }X-\frac{1}{2\pi \alpha}\int{\text{d}^2z\ b^{\mu \nu}\left( D_{\mu}c_{\nu}+D_{\mu}c_{\nu}+2c^{\left( 1 \right)}h_{\mu \nu} \right)}-iB\left( h_{\mu \nu}-\delta _{\mu \nu} \right) \right)}
$$
$$
=\int{D\left[ X,c,b \right] \exp \left( -\frac{1}{2\pi \alpha}\int{\text{d}^2z}\partial X\overline{\partial }X-\frac{1}{2\pi \alpha}\int{\text{d}^2z\ b^{\mu \nu}\left( D_{\mu}c_{\nu}+D_{\mu}c_{\nu} \right)} \right)}
$$

上面的希腊字母表示的是世界面指标.

我们将通过鬼场，看到共形反常是如何消除的，只需要计算能动张量.

鬼场中心荷将为26，为了与物质场的中心荷刚好消掉保留理论整体的weyl不变性，我们必须有维度为26.（计算待）                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                

能动张量的发散问题，是取对应的自然排序，减去带来发散的contraction，或者奇点.
$$
\frac{1}{2\pi \alpha}\int{\text{d}^2z\,\,b^{\mu \nu}\left( D_{\mu}c_{\nu}+D_{\mu}c_{\nu} \right)}\rightarrow \frac{1}{2\pi \alpha}\int{\text{d}^2z\sqrt{h}\ h^{\gamma \lambda}h^{\alpha \beta}b_{\alpha \gamma}\left( \partial _{\beta}c_{\lambda}+\partial _{\lambda}c_{\beta} \right)}
$$
$$
\rightarrow \frac{1}{2\pi \alpha}\int{\text{d}^2z\left( b_{zz}\overline{\partial }c^z+b_{\bar{z}\bar{z}}\partial c^{\bar{z}} \right) \,\,}
$$

我们将重点讨论这种理论的中心荷，因为他们在接下来将有许多的运用：
$$
S=\frac{1}{2\pi}\int{\text{d}^2z\ b\overline{\partial }c}\ ,\ h_b=\lambda \ ,\ h_c=1-\lambda 
$$
$$
\delta ^2\left( z \right) -\frac{\delta S}{\delta b}=0\rightarrow \overline{\partial }\left< \left. bc \right> =2\pi \delta ^2 \right. 
$$
$$
\left< \left. b\left( z_1 \right) c\left( z_2 \right) \right> \right. =\frac{1}{z_{12}}
$$
$$
T\left( z \right) =-4\pi \cdot \frac{1}{2\pi}\cdot \frac{\delta h^{\lambda}b\partial c}{\delta h}=-2:\lambda b\partial c-\frac{1}{2}c\partial b:=2\left( -\lambda :b\partial c:+:c\partial b: \right)
$$

上面能动张量的推导不会？

其中心荷为 $c=-3(2\lambda-1)^2+1$ .

为了理论是可以计算的，我们需要消去反常，就是把能动张量的中心荷归为0，由于能动张量只是线性的加在一起，且相互之间没有影响，所以就是各自场的中心荷加在一起为0.

###### off shell 形式

求弦论中的散射振幅就是求对应的“模”的顶点算符（动量决定）作用在世界面的CFT上（含世界面坐标）的振幅.

最后的结果会积掉世界面坐标，对应模空间问题.由于广相要求的协变性，结果的振幅不该与有限的靶空间坐标有关，弦必须能延长到无穷远处才不会矛盾.

一般来说，我们可以用背景场方法进行在很强的固定的外场下的计算：
$$
e^{-S_{\sigma}}=\exp{[-\frac{1}{4\pi}\int{\text{d}^2\sigma\sqrt{g} \ R\Phi}]} e^{-S}\left( 1-\frac{1}{4\pi \alpha}\int{\text{d}^2\sigma \ \sqrt{g}g^{ab}h_{\mu \nu}\left( X \right) \partial _aX^{\mu}\partial _bX^{\nu}}-\frac{1}{4\pi \alpha}\int{\text{d}^2\sigma\sqrt{g} \ \epsilon ^{ab}B_{\mu \nu}\left( X \right) \partial _aX^{\mu}\partial _bX^{\nu}}+\cdots \right)
$$

$$
e^{-S_{\sigma}}=\exp \left( -\frac{1}{4\pi \alpha}\int{\text{d}^2\sigma \,\,\sqrt{g}\left( g^{ab}G_{\mu \nu}+i\epsilon ^{ab}B_{\mu \nu}\left( X \right) \right) \partial _aX^{\mu}\partial _bX^{\nu}}-\frac{1}{4\pi}\int{\text{d}^2\sigma\sqrt{g} \,\,R\Phi} \right)
$$

即弦是在固定的弯曲时空度规，胀子，一些场的作用下的振幅.包含了各种可能的引力与场的耦合，与来自于路径积分的测量的胀子项.

可以计算能动张量，在共形不变下能动张量的迹为0，但是在off shell形式里，我们保留下形式进行更多讨论.并且可以直接的推出在靶空间中的作用量形式，而不是像在壳时一样通过运动方程反推.

如果对系统做共形变换，则对于XX contraction应该改为  $XX \approx-\alpha \omega-\frac{\alpha}2\ln(z-w)^2$ .

对于闭弦背景场，能动张量求出来为：（）

开弦也可以做一样的操作，得到的是杨米尔斯规范场的形式.

###### 计算配分函数：

1.测量的问题，我们考虑理论：

$Z=\int\Pi {\rm d}X\sqrt{G(X)}\exp{[-\frac{1}{4\pi\alpha}\int{\rm d}z\sqrt{g}\left(\alpha R^{(2)}\Phi(X)+\partial_AX^\mu\partial^AX^\nu G_{\mu\nu}\right)]}$  .
