---
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 13.平面弯曲应力

## 梁横截面上的内力

***

![梁横截面上的内力](../../img/梁横截面上的内力.png)

* 剪力 $F\_s \rightarrow \tau dA$
* 弯矩 $M \rightarrow \sigma dA$

## 梁横截面上的正应力

***

### 1. 变形几何关系 📐

![变形几何关系](../../img/平面弯曲几何关系.png)

1. 纵线变为曲线，且梁上部纵线缩短，下部纵线伸长；
2. 横线仍为直线，但旋转了一个角度，并与弯曲后的纵线**正交**；
3. 纵线伸长区，梁的宽度减小；纵线缩短区，梁的宽度增大

{% hint style="info" %}
**两个假设**

* 平面假设 变形后，横截面仍保持为平面，并和弯曲后的纵线正交
* 单向受力假设： 梁内各纵向线之间互不挤压，只承受单向拉伸或单向压缩
{% endhint %}

#### **中性层**

![中性层](../../img/中性层.png)

中间有一层纵线既不伸长，也不缩短，称为**中性层**。中性层与横截面的交线为中性轴

#### 线应变

![线应变](../../img/线应变示意图.png)

$d\theta$ 1-1 和 2-2 截面的相对转角 $\rho$ 变形后中性层的曲率半径 $y$ 任一纵线到中性层的距离

ab 的线应变：

$$\epsilon=\frac{a'b'-ab}{ab}=\frac{(\rho+y)d\theta-\rho d\theta}{\rho d\theta}=\frac{y}{\rho}$$

### 2. 物理关系

在线弹性范围内 $\sigma =E\epsilon = E\frac{y}{\rho}$

正应力沿截面高度**线性分布**，沿截面宽度**均匀分布**， 中性轴上正应力为**零**。

### 3. 静力学关系

1. $$F_N=\int_A \sigma dA = 0 \rightarrow \int_A y dA = 0$$ 横截面对中性轴的面积矩等于零
2. $$M_y=\int_A z\sigma d A= 0 \rightarrow \int_A yz dA = 0$$
3. $$M_z=\int_A y\sigma d A= 0 \rightarrow \frac{E}{\rho} \int_A y^2 dA = 0 \rightarrow \frac{1}{\rho} =\frac{M}{EI_Z}\rightarrow \sigma = \frac{My}{I_Z}$$

$$EI_Z$$梁的弯曲刚度

**最大正应力**：\$$