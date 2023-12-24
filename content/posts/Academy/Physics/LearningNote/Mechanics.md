---
title: '课程笔记：理论力学知识点总结'
date: 2023-10-24T15:39:04+08:00
image: ""
tags: ["learning_note","theoretical_mechanics","physics"]
description:  '课程笔记：理论力学知识点总结'
lastmod: 2023-10-24T15:39:04+08:00
draft: true
categories: 	
    - "Academy"
    - "LearningNote"
---

> 《理论力学》课程学期期间学习笔记（期末总结）





## 微振动

**勒襄-狄里赫里定理：**
$$
\frac{dV\frac{dV}{dq}=0\frac{dV}{dq}=0}{dq}=0,\frac{d^2V}{dq^2}>0\\
\frac{dV}{dq_1}=\frac{dV}{dq_2}=0\\
\left\{\begin{matrix}
 &\left(\frac{\partial^2 V}{\partial q_1\partial q_2}\right)^2- \frac{\partial^2 V}{\partial q_1^2}\frac{\partial^2 V}{\partial q_1^2} <0\\
 &\frac{\partial^2 V}{\partial q_1^2}>0,\frac{\partial^2 V}{\partial q_2^2}>0 \\

\end{matrix}\right.
$$
**线性振动：**力学体系在平衡位置附近作微振动

### 两个自由度保守体系的自由振动

**动能：**$T=\frac{1}{2}\sum\limits^2_{i,j=1}A_{ij}\dot{x}_i\dot{x}_j=\frac{1}{2}\left(A_{11}\dot{x}_1^2+2A_{12}\dot{x}_1\dot{x}_2+A_{22}\dot{x}^2_2\right)$

**零点展开**

**势能：** $V(x_1,x_2)=\frac{1}{2}\sum\limits^2_{i,j=1}\left(\frac{\partial V^2}{\partial x_i\partial x_j}\right)_0x_ix_j=\frac{1}{2}(b_{11}x_1^2+2b_{12}x_1x_2+b_{22}x_2^2)$

**动能：** $T=\frac{1}{2}\left(a_{11}\dot{x}_1^2+2a_{12}\dot{x}_1\dot{x}_2+a_{22}\dot{x}^2_2\right)$

得：
$$
\sum\limits_{j=1}^2(a_{ij}\ddot{x}_j+b_{ij}x_j)=0,\quad i=1,2\\
\text{试取解：}
\left\{\begin{matrix}
&x_1=A_1\sin(\omega t+\alpha)\\
&x_2=A_2\sin(\omega t+\alpha)
\end{matrix}\right.
$$
**频率方程：** $(b_{11}-a_{11}\omega^2)(b_{22}-a_{22}\omega^2)-(b_{12}-a_{12}\omega^2)^2=0$

$a_{11},a_{22},b_{11},b_{22}>0,\quad a_{11}a_{22}>a_{12},b_{11}b_{22}>b_{12}$

## 哈密顿

### 勒让德变换

新的函数等于不要的变量乘以原来的函数对该变量的偏微商再减去原来的函数。
$$
f=f(x,y),\quad df=udx+vdy\quad u=\frac{\partial f}{\partial x},v=\frac{\partial f}{\partial y}\\
\bar{f}(u,y)=f[x(u,y),y]\\

\left.\begin{matrix}
&\frac{\partial\bar{f}}{\partial y}=v+u\frac{\partial x}{\partial y}\\
&\frac{\partial \bar{f}}{\partial u}=u\frac{\partial x}{\partial u}
\end{matrix}\right\}\\

\left.\begin{matrix}
&v=-\frac{\partial }{\partial y}(-\bar{f}+ux)=-\frac{\partial g}{\partial y}\\
&x=-\frac{\partial }{\partial u}(-\bar{f}+ux)=-\frac{\partial g}{\partial y}
\end{matrix}\right\}
$$

### 正则方程

$\dot{q}_\alpha\to p_\alpha\Rightarrow H(p,q,t)=-L+\sum p_\alpha\dot{q}_\alpha\Rightarrow dH=\sum (-\dot{p}_\alpha dq_\alpha+p_\alpha d\dot{q}_\alpha)+\frac{\partial L}{\partial t}dt$

H is the function of the $q,p,t\to\quad \dot{q}_\alpha=\frac{\partial H}{\partial p_\alpha}\quad \dot{p}_\alpha=-\frac{\partial H}{\partial q_\alpha},\quad \frac{\partial H}{\partial t}=-\frac{\partial L}{\partial t}$ 

### 能量积分和循环积分

H不显含t，$H=T+V$

### <font color="orange">**求解方法**</font>

1. 列出拉格朗日函数
2. 列出$p_\alpha$ ，$H$
3. 求出 $\dot{p}_\alpha$  ， $\dot{q}_\alpha$

### 泊松括号

$\left[\varphi,H\right]=\sum\limits_{\alpha =1}^s \left( \frac{\partial\varphi}{\partial q_\alpha}  \frac{\partial H}{\partial p_\alpha} - \frac{\partial\varphi}{\partial p_\alpha} \frac{\partial H}{\partial q_\alpha} \right)$ $\left.\begin{matrix}&\dot{p}_\alpha=\left[p_\alpha,H\right]\\ &\dot{q}_\alpha=\left[q_\alpha,H\right] \end{matrix}\right\}\quad(\alpha =1,2,3,\dots,s)$

#### 泊松括号的特性

1. $\left[c,\psi\right]=0$
2. $\left[\varphi,\psi\right]+\left[\psi,\varphi\right]=0$
3. $\left[\varphi,\psi\right]=\sum\limits^n_{j=1}\left[\varphi,\psi_j\right]$
4. $\left[-\varphi,\psi\right]=-\left[\varphi,\psi\right]$
5. $\frac{\partial}{\partial  t}\left[\varphi,\psi\right]=\left[\frac{\partial\varphi}{\partial t},\psi\right]+\left[\varphi,\frac{\partial\varphi}{\partial t}\right]$
6. $\left[\theta,\left[\varphi,\psi\right]\right]+\left[\varphi,\left[\psi,\theta\right]\right]+\left[\psi,\left[\theta,\varphi\right]\right]$
7. $\left[q_\alpha,p_\beta\right]=\delta_{\alpha\beta}=\left\{\begin{matrix}&1\quad(\alpha=\beta)\\&0\quad(\alpha\neq\beta)\end{matrix}\right.$

第四章 刚体 100

第五章  非惯性参考系 150

第六章 多自由度体系的微振动 172
