---
title: '课程笔记：光的衍射'
date: 2023-10-24T15:39:04+08:00
image: ""
tags: ["learning_note","electrodynamics","physics","light"]
description:  ' '
lastmod: 2023-10-24T15:39:04+08:00
categories: 	
    - "Academy"
    - "LearningNote"

---

> 《物理光学》课程学期期间学习笔记——光的衍射部分



## 一、定义

**1.衍射：**波在传播过程中遇到障碍物偏离几何路径传播（进入几何阴影区）的现象。$\rightarrow$ 和干涉同时存在  $\rightarrow$  是==一切波动==固有的特性

**2.衍射屏和屏函数**： $\tilde{E_i} \ \rightarrow \ 衍射屏\  \rightarrow \ \tilde{E_t}$ 

**3.复振幅透射函数:**  $\tilde{t}(x,y)=\frac{\tilde{E_t}(x,y)}{\tilde{E_i}(x,y)} \rightarrow 瞳函数$ 

## 二、衍射三要素

1. 光源发出的光波
2. 衍射物
3. 衍射图形

## 三、菲涅尔衍射和夫琅禾费衍射

- 菲涅尔衍射$\rightarrow$ 光源和接收屏在有限远处，满足傍轴近似

- 夫琅禾费衍射$\rightarrow$ 光源和接收屏在无限远处，满足远场近似

### 惠更斯-菲涅尔原理

**含义：**波前上的每一个面元都可以看作是一个次级扰动中心，它们能产生球面子波。后一时刻的波前的位置是所有这些子波前的包络面

**相干叠加：**P点的振动是次波对P点的相干叠加的结果，波前$\Sigma$ 上任一点的复振幅：$E_Q=A\frac{exp(ikR)}{R}$ ，Q处小面元$d\sigma$ 发出的子波：$K(\theta)CE_Q d\sigma \frac{exp(ikRr)}{r}$

则$P$点的复振幅：
$$
E(P)=\iint\limits_{\Sigma'}CK(\theta)E_Q\frac{exp(ikr)}{r}d\sigma\\=CE_Q\iint\limits_{\Sigma'}K(\theta)\frac{exp(ikr)}{r}d\sigma
$$
**惠更斯-菲涅尔原理：**

1. 波传到的任意点都是次波的中心
2. 包围光源的任一波前上各次波在空间各点进行相干叠加

### 基尔霍夫衍射积分公式

$$
E(P)=\frac{1}{i\lambda} \iint\limits_\Sigma \frac{Aexp(ikl)}{l}\frac{exp(ikr)}{r}\frac{\cos \alpha_1+\cos \alpha_2}{2}d\sigma
$$

**近似-1：**光源离开孔足够远 $\to$ 入射光视为垂直入射 $\to\ \cos \alpha_1=1,\cos \alpha_2=\cos \theta \to\ K(\theta)=\frac{1+\cos \theta}{2}$  

- $\theta=0,K(\theta)=1 \to\ 波面法线法线方向上子波的振幅最大$
- $\theta=\pi,K(\theta)=0\to\ 证明菲涅尔关于\theta=\frac{\pi}{2}时K(\theta)=0的结论时错误的$

**近似-2：**

- 实际中，衍射孔线度 $\ll$ 光源、观察屏到衍射屏距离$\to \theta\ 变化很小\to K(\theta)可提出积分外，取K(\theta)=1$
- 实际中，$r$ 的变化不大，约取$\frac{1}{r}\approx\frac{1}{z_1}$ 

**得简化的基尔霍夫公式：**
$$
\tilde{E}(P)=\frac{1}{i\lambda z_1}\iint\limits_\Sigma\tilde{E}(Q)exp(ikr)d\sigma
$$
**近似-3：** 对 $r=z_1[1+(\frac{x-x_1}{z_1})^2+(\frac{y-y_1}{z_1})^2]$ 作二项展开，因为 $z_1\gg x,y,x_1,y_1$，有只取展开后的前两项 
$$
r=z_1\{1+\frac{1}{2}[\frac{(x-x_1)^2+(y-y_1)^2}{z^2_1}]\}\to\ 菲涅尔近似
$$

### 单缝夫琅禾费衍射

**光强：**   $I(P)=\frac{\sin^2 \alpha}{\alpha^2}=I_0\sin c^2\alpha$  ，其中$\alpha=\frac{\pi}{\lambda}a\sin\theta$

**振幅矢量法：**

- 暗纹：$\frac{\pi a}{\lambda}\sin\theta=k\pi$
- 明纹中心：$\tan\alpha=\alpha$

**菲涅尔半波带法：** 
$$
\delta=a\sin \theta=k\frac{\lambda}{2}, \quad \left\{\begin{matrix}
 k=2n-1, \quad n=1,2,3\dots \quad 亮纹\\
 k=2n,\quad n=1,2,3\dots \quad 暗纹
\end{matrix}\right.
$$
**条纹角宽度：**

1. 中央明纹半角宽度：$\frac{\lambda}{a}$
2. 其他明纹：$\Delta\theta_k=\theta_{暗k+1}-\theta_{暗k}\approx\frac{\lambda}{a}$

## 四、圆孔、圆环和多边形孔的夫琅禾费衍射

### 圆孔夫琅禾费衍射

**光强：** $I_p=I_0[\frac{2J_1(\psi)}{\psi}]^2 \quad\to\ J_1(\psi):一级贝塞尔函数$

​			$J_1(\psi)的级数展开\quad J_1(\psi)=\frac{\psi}{2}-\frac{\psi^2}{2^2\cdot4}+\frac{\psi^3}{2^2\cdot4^2\cdot6}-\dots$

​			第一级：$\sin \theta=1.22\frac{\lambda}{D}$

### 圆环的夫琅禾费衍射

$\varepsilon=\frac{R_1}{R_2}$ 接收屏上P点的光强：
$$
I(P)=\frac{I_0}{(1-\varepsilon^2)^2}[\frac{2J_1(\psi_2)}{\psi_2}-\varepsilon^2\frac{2J_1(\psi_1)}{\psi_1}]^2
$$
**特点：** 中央为亮斑，周围是明暗相间的圆环；$\varepsilon$ 越大，中央亮斑越小，条纹向中心收缩

## 五、成像仪器像分辨本领

**瑞利判据：** 点物$S_1$的艾里斑中心恰好与另一个点物$S_2$的艾里斑边缘（第一衍射极小）相重合时，恰好分辨两物点。

**最小分辨角：** $\delta\varphi=1.22\lambda/D$

## 六、衍射光栅

### 分类

1. 结构
   - 一维光栅：平板等距划痕
   - 二维
   - 三维
2. 材料
   - 振幅型
   - 位相型
3. 功能
   - 透射式
   - 反射式

### 光栅衍射

**光栅常数：** $d=a+b\quad a:透光,b:不透光$     $d=\frac{1}{N}$

#### 缝间干涉因子

**多振幅干涉：** 合振幅  $A=A_0\frac{\sin \frac{N\varphi}{2}}{\sin\frac{\varphi}{2}}$

- 主极大：$d\sin\theta=k\lambda, \quad k=0, \pm 1, \pm 2, \dots$
- 暗纹：$d\sin \theta=\frac{k'}{N}\lambda ,\ k'为整数且\neq 0,\pm N, \pm 2N, \dots$

​	相邻主极大之间有 N-1个暗纹，N-2个次极大

**缺级现象：** $k=\pm \frac{d}{a}k', 其中k'为衍射级次$

#### 光栅衍射光强公式

$$
I_P=I_0(\frac{\sin u}{u})^2\cdot(\frac{\sin N\beta}{\sin \beta})^2\\
u=\frac{\pi a\sin \theta}{\lambda},\quad \beta=\frac{\varphi}{2}=\frac{\pi d\sin\theta}{\lambda}
$$

### 谱线的半角宽度

$$
\Delta\theta=\frac{\lambda}{Nd\cos\theta_K}
$$

### 倾斜入射时的光栅方程

$$
d(\sin i\pm\sin\theta)=m\lambda
$$

### 光谱色散

$$
D=\frac{\delta\theta}{\delta\lambda}\\
D=\frac{K}{d\cos\theta}\to D_l=\frac{Kf'}{d\cos\theta}( 线色散本领 )\\
色分辨本领:R\equiv\frac{\lambda}{\Delta\lambda}=kN
$$

#### 棱镜

色散本领：在最小偏向角时
$$
D=\frac{d\delta_m}{d\lambda}=(\frac{dn}{d\delta_m})^{-1}\frac{dn}{d\lambda},\quad\frac{dn}{d\lambda}\to棱镜材料的色散率\\
色散本领:D\frac{2\sin\frac{\alpha}{2}}{\sqrt{1-n^2\sin^2 \frac{\alpha}{2}}}\cdot\frac{dn}{d\lambda}\\ 
线色散:D_l=\frac{dl}{d\lambda}=Df'=\frac{2f'\sin\frac{\alpha}{2}}{\sqrt{1-n^2\sin^2\frac{\alpha}{2}}}\cdot\frac{dn}{d\lambda}
$$
色分辨本领：
$$
R=t\cdot\frac{dn}{d\lambda}
$$

## 菲涅尔衍射

### 菲涅尔半波带法

各半波带在P点的$\alpha_i$相邻带在Pd点产生的振动位相相反，合振动取决于：波带面积、距离、倾斜因子

#### 小圆孔衍射

露出半波带数
$$
n=\frac{\rho^2(R+r_0)}{Rr_0\lambda}
$$


$$
a\sin\theta_x=n\lambda\quad\to\quad\text{Dark}\\
\tan\alpha=\alpha\quad\to\quad\text{Light(Page 168)}
$$

$$
\frac{I}{I_0}=\left [\frac{2J_1(Z)}{Z} \right ]^2\\
J_1(Z)=0\to\text{Dark},\quad\frac{d}{dZ}\frac{J_1(Z)}{Z}=0\to\text{Light}\quad\text{(Page 172)}
$$

