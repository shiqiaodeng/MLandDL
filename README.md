---
export_on_save:
html: true
---

# MLandDL

## 逻辑回归
线性模型：
$f(\boldsymbol{x})=w_{1} x_{1}+w_{2} x_{2}+\ldots+w_{d} x_{d}+b$   
向量形式：   
$f(\boldsymbol{x})=\boldsymbol{w}^{\mathrm{T}} \boldsymbol{x}+b$,  
其中$\boldsymbol{w}=\left(w_{1} ; w_{2} ; \ldots ; w_{d}\right)$ 和 $b$ 为模型参数。   
线性模型的目标就是学习到合适的 $w$ 和 $b$ 去作回归预测，如房价预测，西瓜好坏。
如何学习到$w$ 和 $b$? 
1. 首先定义损失函数，计算当前预测值与实际输出值之间的差异，包括均方误差，交叉熵等。   
2. 选择优化算法，目前所有优化算法都是基于梯度下降，通过调整学习率跟梯度方向提出了包括随机梯度下降，mini-batch 梯度下降、Momentum 动量算法、AdaGrad 算法、RMSProp 算法、Adam 算法。
若选择均方误差作为线性回归的损失函数，最优问题：
$\begin{aligned}\left(w^{*}, b^{*}\right) &=\underset{(w, b)}{\arg \min } \sum_{i=1}^{m}\left(f\left(x_{i}\right)-y_{i}\right)^{2} \\ &=\underset{(w, b)}{\arg \min } \sum_{i=1}^{m}\left(y_{i}-w x_{i}-b\right)^{2} \end{aligned}$

线性回归虽然简单但是却难以预测非线性模型，而非线性模型在现实世界中的任务有比较常见，因此有人引入对数来预测非线性模型，其定义如下：
$\ln y=\boldsymbol{w}^{\mathrm{T}} \boldsymbol{x}+b$.
这就是对数线性回归，$y=e^{\boldsymbol{w}^{\mathrm{T}} \boldsymbol{x}+b}$,通过将输出映射到对数空间中预测。
更一般化，使用其他函数作为非线性映射函数：
$y=g^{-1}\left(\boldsymbol{w}^{\mathrm{T}} \boldsymbol{x}+b\right)$
只要$g(x)$ 可微。

对数回归

## 支持向量机

## 决策树

## BP神经网络

## 聚类

### K-means 聚类

## DNN深度神经网络
### CNN 卷积神经网络

### RNN 循环神经网络

### LSTM

## 集成学习

### AdaBoost 算法

### XGBoost 算法

## 优化算法

### SGD 随机梯度下降

### Momentum 动量算法

### AdaGrad 算法

### RMSProp 算法

### Adam 算法

## 图神经网络

### 图嵌入（Graph embedding）

## 推荐系统

## NLP

### Wordtovec

