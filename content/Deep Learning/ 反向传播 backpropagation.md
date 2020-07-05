---
date:2020-07-05

---


## Backpropagation 
反向传播（英語：Backpropagation，缩写为BP）是“误差反向传播”的简称，是一种与最优化方法（如梯度下降法）结合使用的，用来训练人工神经网络的常见方法。 该方法对网络中所有权重计算损失函数的梯度。 这个梯度会反馈给最优化方法，用来更新权值以最小化损失函数。

### Forward vs Back propagation
##### 正反馈的神经网络
* **forward propagation** x1,x2,x3....hidden layers ===> y1,y2,y3
* **back propagation**  如果y1要下降一点 梯度该怎样调整 会使得 y1更接近真实值


##### Chain Rule
Δw → Δx → Δy → Δz  
∂z / ∂w =(∂z / ∂y) * (∂y / ∂x) * (∂x / ∂w)  
w 的变动导致多少 y 的变动 y 的变动导致 z 发生了多少变动@forward  
y 要怎么变会使 z 变动...@back 