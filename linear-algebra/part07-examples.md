---
title: Linear Algebra - Part 7 - Examples for Subspaces
---

[Linear Algebra - Part 7 - Examples for Subspaces - YouTube](https://www.youtube.com/watch?v=gVQCXMbw098&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=7)

部分空間の例と反例を見ていく。

$\text{(1)}$

$$
U = \!\left\{ \begin{pmatrix}x_1 \\ x_2 \\ x_3\end{pmatrix} \in \mathbb R^3
\,\middle|\,
x_1 = x_2,\;x_3 = -2x_2
\right\}
$$

は部分空間か。前回の三性質を確認すればわかる。

$\text{(a)}$ $0 \in U$ は OK.

$$
x \coloneqq \begin{pmatrix}x_1 \\ x_2 \\ x_3\end{pmatrix} = 0
$$

とおくと、${0 = x_1 = x_2}$ かつ ${0 = x_3 = -x_2}$ が成り立つ。ゆえに ${0 \in U.}$

$\text{(b)}$ $U$ はスカラー倍について閉じているか。
${u \in U,}\;{\lambda \in \mathbb R}$ とし、

$$
x = \lambda u\coloneqq
\begin{pmatrix}\lambda u_1 \\ \lambda u_2 \\ \lambda u_3\end{pmatrix}
$$

とおく。${u_1 = u_2,}\;{u_3 = -2u_2,}$ から ${x_1 = x_2,}\;{x_3 = -2x_2}$ を示せばいい：

$$
\begin{aligned}
x_1 - x_2 &= \lambda u_1 - \lambda u_2 = \lambda(u_1 - u_2) = 0.\\
x_3 + 2x_2 &= \lambda u_3 + 2\lambda u_2 = \lambda(u_3 + 2u_2) = 0.
\end{aligned}
$$

ゆえに $x \in U.$

$\text{(c)}$ $U$ は加法について閉じているか。
$u, v \in U$ とし、

$$
x = u + v \coloneqq
\begin{pmatrix}u_1 + v_1 \\ u_2 + v_2 \\ u_3 + v_3\end{pmatrix}
$$

とおく。${u_1 = u_2,}\;{u_3 = -2u_2,}\;{v_1 = v_2,}\;{v_3 = -2v_2}$ から
${x_1 = x_2,}\;{x_3 = -2x_2}$ を示せばいい。

以上により $U$ は $\mathbb R^3$ の部分空間である。

$\text{(2)}$

$$
U = \!\left\{ \begin{pmatrix}x_1 \\ x_2\end{pmatrix} \in \mathbb R^2
\,\middle|\,
x_1^2 = x_2
\right\}
$$

は部分空間か。

例えば $\text{(b)}$ が成り立たないことを示せば、部分空間でないことが言える。

${u = \begin{pmatrix}1 \\ 1\end{pmatrix} \in U}$
に対して

$$
2u = \begin{pmatrix}2 \\ 2\end{pmatrix}.
$$

$2^2 \ne 2$ だ。$U$ はスカラー倍に対して閉じていないので、部分空間ではない。

以上
