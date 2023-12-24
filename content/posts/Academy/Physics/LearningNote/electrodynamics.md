---
title: '课程笔记：电动力学知识点总结'
date: 2023-10-24T15:39:04+08:00
image: ""
tags: ["learning_note","electrodynamics","physics"]
description:  '课程笔记：电动力学知识点总结'
lastmod: 2023-10-24T15:39:04+08:00
draft: true
categories: 	
    - "Academy"
    - "LearningNote"
---

> 《电动力学》课程学期期间学习笔记（期末总结）



## 数学部分

**定义：** 

- 梯度：方向导数的最大值 $(grad\varphi)_l=\frac{d\varphi}{dl}$
- 散度：$div\vec{f}=\lim\limits_{\Delta V\to0}\frac{\oint\vec{f}\cdot d\vec{S}}{\Delta V}$
- 旋度：$rot\vec{f}=\lim\limits_{\Delta S\to0}\frac{\oint\vec{f}\cdot d\vec{l}}{\Delta S}\vec{n}$

**柱坐标系：** 

- $\nabla$ :$\nabla=\vec{e_r}\frac{\partial}{\partial r}+\vec{e_\theta}\frac{1}{r}\frac{\partial}{\partial\theta}+\vec{e_z}\frac{\partial}{\partial z}$ 

- 散度:$\nabla\cdot\vec{A}=\frac{\partial A_r}{\partial r}+\frac{A_r}{r}+\frac{1}{r}\frac{\partial A_\theta}{\partial\theta}+\frac{\partial A_z}{\partial z}$ 

**球坐标：** 

- $\nabla$ : $\vec{e_r}\frac{\partial}{\partial r}+\vec{e_\theta}\frac{1}{r}\frac{\partial}{\partial\theta}+\vec{e_\phi}\frac{1}{r\sin\theta}\frac{\partial}{\partial\varphi}$

**公式：**

- 复合函数
  - $\nabla f(u)=\frac{df}{du}\nabla u$
  - $\nabla\cdot\vec{A}(u)=\frac{d\vec{A}}{du}\cdot\nabla u$
  - $\nabla\times\vec{A}(u)=\nabla u\times\frac{d\vec{A}}{du}$ 
- 常用公式
  - $\nabla(\varphi\psi)=(\nabla\varphi)\psi+\varphi\nabla\psi$
  - $\nabla\cdot(\varphi\vec{A})=\nabla\varphi\cdot\vec{A}+\varphi\nabla\cdot\vec{A}$
  - $\nabla\times(\varphi\vec{A})=\nabla\varphi\times\vec{A}=\varphi\nabla\times\vec{A}$
  - $\nabla\cdot(\vec{A}\times\vec{B})=\vec{B}\cdot(\nabla\times\vec{A})-\vec{A}\cdot(\nabla\times\vec{B})$
  - $\nabla\times(\vec{A}\times\vec{B})=(\vec{B}\cdot\nabla)\vec{A}+(\nabla\cdot\vec{B})\vec{A}-(\nabla\cdot\vec{A})\vec{B}-(\vec{A}\cdot\nabla)\vec{B}$ 
  - $\nabla(\vec{A}\cdot\vec{B})=\vec{A}\times(\nabla\times\vec{B})+\vec{B}\times(\nabla\times\vec{A})+(\vec{A}\cdot\nabla)\vec{B}+(\vec{B}\cdot\nabla)\vec{A}$ 
  - $\nabla\cdot\nabla\varphi\equiv\nabla^2\varphi$
  - $\nabla\times(\nabla\times\vec{A})=\nabla(\nabla\cdot\vec{A})-\nabla^2\vec{A}$
- 高斯公式和斯托克斯公式：$\oint_S\vec{f}\vdot d\vec{S}=\int_V\nabla\cdot\vec{f}dV$,  $\oint_L\vec{f}\cdot d\vec{l}=\int_S(\nabla\times\vec{f})\cdot d\vec{S}$

**一些值：** $\nabla r=\frac{\vec{r}}{r}$  ,   $\nabla\vec{r}=3$,    $\nabla\cdot\frac{\vec{r}}{r^3}=\nabla\times\frac{\vec{r}}{r^3}=0$   

## 第一章

电荷守恒定律：$\nabla\cdot\vec{J}+\frac{\partial\rho}{\partial t}=0$, $I=\int_S\vec{J}\cdot d\vec{S}$, $\vec{J}=\sum\limits_i\rho_i\vec{v}_i$

毕奥萨伐尔定律：$\vec{B}=\oint_L\frac{\mu_0}{4\pi}\frac{Id\vec{l}\times\vec{t}}{r^3}=\frac{\mu_0}{4\pi}\int\frac{vec{J}(x')\times\vec{t}}{r^3}dV'$

$J_D=\varepsilon_0\frac{\partial\vec{E}}{\partial t}$,  $\vec{f}=\rho\vec{E}+\vec{J}\times\vec{B}$ , $\rho_P=-\nabla\cdot\vec{P}$, $D=\varepsilon_0E+P$ ,$P=\chi_e\varepsilon_0$E

$J_M=\nabla\times\vec{M},\vec{J}_P=\partial P/\partial t$,  $M=\chi_eH$ ,$\sigma_p=-\vec{n}(\vec{P}_2-\vec{P}_1)$

$\hat{n}\cdot(\vec{D}_2-\vec{D}_1)=\sigma_f$, $\hat{n}\cdot(\vec{B}_2-\vec{B}_1)=0$ ,$\hat{n}\times(\vec{E}_2-\vec{E}_1)=0$, $\hat{n}\times(\vec{H}_2-\vec{H}_1)=\alpha$      $\nabla\cdot\vec{S}+\frac{\partial\omega}{\partial t}=-\vec{f}\cdot\vec{v}$ 



## 第二章

$E=-\nabla\varphi$  , $d\varphi=-E\cdot dl$,  $\varphi(x)=\int_V\frac{\rho(x')dV'}{4\pi\varepsilon_0r}$

总能量：$W=\frac{1}{2}\int_\infin E\cdot DdV=\frac{1}{2}\int_V\rho\varphi dV$ , 

## 第三章

$\nabla\cdot B=0,\ B=\nabla\times A,\ \nabla\cdot A=0$, $\nabla\times(A+\nabla\varphi)=\nabla\times A$

微分方程：$\nabla\times(\nabla\times A)=\mu J\to\nabla^2A=-\mu J\to A(x)=\frac{\mu}{4\pi}\int_V\frac{J(x')dV'}{r}$

$W=\frac{1}{2}\int B\cdot HdV\to\frac{1}{2}\int_VA\cdot dV$

磁标势：$\vec{H}=-\nabla\varphi_m$  $\nabla\cdot H=\rho_m/\mu_0$    $\rho_m=-\mu_0\nabla\cdot M$



## 简答题

- **电势所满足的微分方程及其边值关系的推导**

$\varphi(x)=\int_V\frac{\rho(x')dV'}{4\pi\varepsilon_0r}$   ,   $\nabla^2\varphi=-\frac{\rho}{\varepsilon},E,D边界条件\to\varphi_1=\varphi_2$,

$\varphi'_1-\varphi_1=\varphi'_2-\varphi_2\to\varphi'_1-\varphi_1=-E_1\cdot\Delta l 利用D条件\to\varepsilon_2\frac{\partial\varphi_2}{\partial n}-\varepsilon_1\frac{\partial\varphi_1}{\partial n}=-\sigma$ 



- **用分离变量法求静电场电势的适用条件；当电势具有轴对称和球对称时，拉普拉斯方程在球坐标系中的通解形式；解题步骤。**

$\nabla^2\varphi=0$, 

- **镜像电荷和镜像法的定义**

镜像电荷：将导体界面上感应电荷等效地看作一个或几个假想的点电荷

镜像法：采用镜像电荷求电势的方法

- **小区域电荷分布产生电势的多级展开第一、二、三项的物理意义及产生电势的表达式**

- **引入磁标势的条件？**

区域内没有链环着的电流



38、电流分布产生的磁偶极矩，磁偶极矩产生的矢势和标势的表达式

$\vec{m}=\frac{I}{2}\oint(\vec{x}'\times d\vec{l}')\to\vec{m=I\Delta\vec{S}}$







## 相对论

### 洛伦兹变换

1. 相对性原理：

   - 所有惯性系都是等价的，不存在特殊的绝对的惯性系
   - 一切物理定律在所有的惯性系都具有相同形式

2. 光速不变原理：真空中的光速相对于任何惯性系沿任一方向恒为从，并与光源运动无关

   
