---
title: Linear Algebra - Part 4 - Lines in $\mathbb R^2$
---

[Linear Algebra - Part 4 - Lines in $\mathbb R^2$ - YouTube](https://www.youtube.com/watch?v=o1zIl30ElY0&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=4)

原点を通る直線は次の形に書ける。ここでベクトル $a$ は直線の方向を、
ベクトル $n$ は直線に対して垂直な向きを持つベクトルとする：

$$
\begin{aligned}
L &= \!\left\{\left. v \in \mathbb R^2 \,\right|\left.\,
    v = \lambda a,\; \lambda \in \mathbb R \right.\right\}\\
&= \!\left\{\left. v \in \mathbb{R}^2 \,\right|\left.\,
    \left\langle n,\;v \right\rangle = 0 \right.\right\}.
\end{aligned}
$$

原点を通らない直線を考える。通過点を位置ベクトルを $p$ とする。
直線上の点の位置ベクトル $v$ に対し、その差が直線と平行なのだから：

$$
\begin{aligned}
L &= \!\left\{\left. v \in \mathbb R^2\,\right|\left.\, 
    \left\langle n,\;v - p \right\rangle = 0\right.\right\}\\
&= \!\left\{\left.\begin{pmatrix}x \\ y\end{pmatrix} \in \mathbb R^2\,\right|\left.\, n_1 x + n_2 y = \delta \right.\right\}.
\end{aligned}
$$

ここで ${n = \begin{pmatrix}n_1 \\ n_2\end{pmatrix}\!,\;}{\delta \coloneqq \left\langle n,\;v - p \right\rangle.}$

（※この $\delta$ の意味は直線と原点との距離のはず）

例：
$y = 2x + 5$ を上の形に書く。$a$ と $n$ を括って出す。

以上。
