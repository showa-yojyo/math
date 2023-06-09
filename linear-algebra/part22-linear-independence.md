---
title: Linear Algebra - Part 22 - Linear Independence (Definition)
---

[Linear Algebra - Part 22 - Linear Independence (Definition) - YouTube](https://www.youtube.com/watch?v=UeHqH1yhoqU&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=22)

$\mathbb R^2$ ベクトル二つが同一直線に乗る：
${u = \lambda v.}$

$\mathbb R^3$ ベクトル三つが同一平面内に乗る：
${u = \lambda v + \mu w.}$

これらを一般化する。

定義：
${v^{(1)},\dotsc,v^{(k)} \in \mathbb R^n}$ とする。
ベクトルの族 ${(v^{(1)},\dotsc,v^{(k)})}$ が **線形従属** であるとは、
次のベクトルがゼロで **ない** ような ${\lambda_1, \dotsc, \lambda_k \in \mathbb R}$
が存在することを言う：

$$
\sum_{j=1}^{k}\lambda_j v^{(j)} = 0 \in \mathbb R^n.
$$

ベクトルの族が **線形独立** であるとは、次が成り立つ場合を言う：

$$
\sum_{j=1}^{k}\lambda_j v^{(j)} = 0
\implies \lambda_1 = \dotsb = \lambda_k = 0.
$$

以上
