---
title: Linear Algebra - Part 6 - Linear Subspaces
---

[Linear Algebra - Part 6 - Linear Subspaces - YouTube](https://www.youtube.com/watch?v=TITspOSjMZw&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=6)

（線形）部分空間：
直線、平面、空間、……であって特別の性質があるもの。

$\mathbb R^2$ ならば線形部分空間と affine 部分空間が存在する。

定義：
$\varnothing \ne U \subset \mathbb R^n$ が $\mathbb R$ の（線形）部分空間であるとは、
$U$ のすべての線形結合がまた $U$ に残ることを言う：

$$
u^{(1)}, \dotsc, u^{(k)} \in U,\;
\lambda_1, \dotsc, \lambda_k \in \mathbb R
\implies
\sum_{j=1}^{k}\lambda_j u^{(j)} \in U.
$$

部分空間の特徴付け：
$U \subset \mathbb R^n$ が部分空間であることと、$U$ に次の三点の性質があることは同値：

$$
\begin{aligned}
\text{(a)}&& 0 \in U&\\
\text{(b)}&& u \in U,\;\lambda \in \mathbb R &\implies \lambda u \in U\\
\text{(c)}&& u,v \in U &\implies u + v \in U\\
\end{aligned}
$$

例：ベクトル空間 $\mathbb R^n$ において、

* $U = \lbrace 0 \rbrace$ は部分空間である。
* $U = \mathbb R^n$ は部分空間である。

$\mathbb R^n$ のどの部分空間 $U$ も次を満たす：

$$
\lbrace 0 \rbrace \subset U \subset \mathbb R^n.
$$

以上
