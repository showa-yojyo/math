---
title: Linear Algebra - Part 9 - Inner Product and Norm
---

[Linear Algebra - Part 9 - Inner Product and Norm - YouTube](https://www.youtube.com/watch?v=SCTWQ_W1Cw8&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=9)

$\mathbb R^n$ の内積とノルム。

* ベクトル空間に構造をもっと入れる
* 幾何が可能になる（角度、長さ）

定義：
${u, v \in \mathbb R^n}$ に対して：

$$
\left\langle u,\;v \right\rangle \coloneqq 
u_1 v_1 + u_2 v_2 + \dotsb + u_n v_n
= \sum_{i=1}^{n}u_i v_i.
$$

これを **（標準）内積** と言う。
また、内積の値がゼロならば、$u, v$ は **直交** するという。

性質：
${u, v, w \in \mathbb R^n,}\;{\lambda \in \mathbb R}$ とする。
内積 ${\left\langle \cdot,\;\cdot \right\rangle \colon \mathbb R^n \times \mathbb R^n \longrightarrow \mathbb R}$
は次の性質がある：

$$
\begin{aligned}
&\text{(1)}&
  \left\langle u,\;u \right\rangle &\le 0\\
&&\left\langle u,\;u \right\rangle &= 0 \iff u = 0 & \text{(positive definitive)}\\

&\text{(2)}&
  \left\langle u,\;v \right\rangle &= \left\langle v,\;u \right\rangle & \text{(symmetric)}\\

&\text{(3)}&
  \left\langle u,\;v + w \right\rangle &= \left\langle u,\;v \right\rangle + \left\langle u,\;w \right\rangle\\
&&\left\langle u,\;\lambda v \right\rangle &= \lambda \left\langle u,\;v \right\rangle
& \text{(linear in the 2nd argument)}
\end{aligned}
$$

内積を使って角度を測ることが考えられる。

定義：
**（標準）ノルム** とか **ユークリッドノルム** という。

$$
\lVert u \rVert \coloneqq \sqrt{\left\langle u,\;u \right\rangle}.
$$

ノルムを使って長さを測ることが考えられる。

例：

$
u = \begin{pmatrix}1 \\ 0 \\ 0 \\ 1\end{pmatrix},
v = \begin{pmatrix}0 \\ 2 \\ 0 \\ 0\end{pmatrix},
$
とすると、

$$
\begin{aligned}
\left\langle u,\;v \right\rangle &= 0.\\
\lVert u \rVert &= \sqrt{1^2 + 1^2} = \sqrt{2},\\
\lVert v \rVert &= \sqrt{2^2} = 2.
\end{aligned}
$$

$u$ と $v$ は直交しており、$u$ よりも $v$ のほうが長い。

以上
