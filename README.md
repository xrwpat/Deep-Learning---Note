# Deep-Learning---Note
my own notebook

## 第六章 前馈神经网络（笔记）
### 6.1 实例：学些 XOR
XOR 函数(‘‘异或’’ 逻辑)是两个二进制值 x1 和 x2 的运算。当这些二进制值 中恰好有一个为 1 时，XOR 函数返回值为 1。其余情况下返回值为 0。
评估整个训练集上表现的 MSE 损失函数为：$$J(\theta)=1/4\sum_{f^{*}(x)-f(x;\theta))^{2}$$
我们现在必须要选择我们模型 $f(\omega ; \theta)$的形式。
网络现在包含连接在一起的两个函数：$$f(x;W,c,\omega,b)=f^{(2)}(f^{(1)}(x))$$

#### 6.2.1.1 使用最大似然学习条件分布
大多数现代的神经网络使用最大似然来训练。这意味着代价函数就是负的对数似然，它与训练数据和模型分布间的交叉熵等价。这个代价函数表示为$$J(\theta)=-E_{x,y~p^hat{^}}logp_{model}(y\x)$$
代价函数的具体形式随着模型而改变，取决于$p_{model}$的具体形式
