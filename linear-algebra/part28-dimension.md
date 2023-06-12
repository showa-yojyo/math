---
title: Linear Algebra - Part 28 - Conservation of Dimension
video: https://www.youtube.com/watch?v=XtiteY3n0Oc&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=28
---

※部分空間の次元のおさらいから

定理：
部分空間 $U, V \subset \mathbb R^n$ に対して、

$\text{(a)}$ $\dim(U) = \dim(V)$ であることと、
全単射線形写像 ${f \colon U \longrightarrow V}$ が存在することは同値。

※逆写像も線形写像であることになる

$\text{(b)}$ ${U \subset V}$ かつ ${\dim U = \dim V}$ ならば ${U = V.}$

証明：

${\text{(a)} \implies:}$
$\dim(U) = \dim(V)$ であるので $U, V$ それぞれの基底を次のようにとれる：

$$
\begin{aligned}
\mathcal B = \left(u^{(1)}, \dotsc, u^{(k)}\right),\\
\mathcal C = \left(v^{(1)}, \dotsc, v^{(k)}\right).\\
\end{aligned}
$$

線形写像 ${f \colon U \longrightarrow V}$ を、まず基底ベクトルに対して
${f\left(u^{(i)}\right) = v^{(i)}}$ で定める。これで $f$ が $U$ 上完全に定まる：

${x \in U}$ に対して $\exists \lambda_1, \dotsc, \lambda_k \in \mathbb R$ で：

$$
\begin{aligned}
f(x) &= f\left(\lambda_1 u^{(1)} + \dotsb + \lambda_k u^{(k)}\right)\\
&= \lambda_1 f\left(u^{(1)}\right) + \dotsb + \lambda_k f\left(u^{(k)}\right)\\
&= \lambda_1 v^{(1)} + \dotsb + \lambda_k v^{(k)}.
\end{aligned}
$$

ここで逆写像 ${f^{-1} \colon V \longrightarrow U}$ を次で定められる：

$$
f^{-1}\left(v^{(i)}\right) = u^{(i)}
$$

このとき ${(f^{-1} \circ f)(x) = x}$ かつ ${f\circ f^{-1}(y) = y.}$
ゆえに $f$ は全単射かつ線形である。

$\impliedby:\quad$ ${f \colon U \longrightarrow V}$ が全単射かつ線形であるとする。
上の記号を使って $U$ の基底 $\mathcal B$ を取る。
このとき $\left(f(u^{(1)}), \dotsc, f(u^{(k)})\right)$ は $V$ の基底になる：

* $f$ が単射であることから、このベクトル族は線形独立であり、
* $f$ が全射であることから ${\operatorname{span}\left(f\left(u^{(1)}\right), \dotsc, f\left(u^{(k)}\right)\right) = V.}$

以上のことから $\dim U = \dim V$ が示された。

$\text{(b)}$ $U$ を基底とする。上の記号を用いる。
このとき、その基底は $V$ の基底でもある。
したがって、${v \in V}$ ごとにスカラー $\lambda_1, \dotsc, \lambda_k$ が定まって
${v = \lambda_1 u^{(1)} + \dotsc + \lambda_k u^{(k)}.}$
右辺は $U$ のベクトルでもあるから ${v \in U}$ でもある。
したがって ${V \subset U}$ であり、結局 ${U = V.}$

以上
