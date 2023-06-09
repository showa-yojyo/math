---
title: Linear Algebra - Part 24 - Basis of a subspace
---

[Linear Algebra - Part 24 - Basis of a subspace - YouTube](https://www.youtube.com/watch?v=_XBTqXwPllI&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=24)

（※部分空間をおさらい）

平面 $\mathbb R^2$ でビデオの図のようにベクトル四個を取ると、

* ${\operatorname{span}(v^{(1)}, v^{(2)}, v^{(3)}, v^{(4)}) = \mathbb R^2.}$
* ${\operatorname{span}(v^{(1)}, v^{(3)}) = \mathbb R^2.}$
* ${\operatorname{span}(v^{(1)}, v^{(4)}) = \mathbb R \times \{0\} \ne \mathbb R^2.}$

定義：
${U \subset \mathbb R^n}$ を部分空間、
${B = (v^{(1)}, \dotsc, v^{(k)})}, v^{(j)} \in \mathbb R^n$ とする。
$B$ が $U$ の **基底** であるとは、次が成り立つことを言う：

* ${U = \operatorname{span}(B).}$
* $B$ が線形独立である。

例：

$$
\mathbb R^n = \operatorname{span}(e_1, \dotsc, e_n).
$$

これを $\mathbb R^n$ の正規基底という。

$$
\mathbb R^3 = \operatorname{span}\left(
    \!\begin{pmatrix}
    -3\\
    0\\
    0
    \end{pmatrix}\!,
    \!\begin{pmatrix}
    1\\
    1\\
    0
    \end{pmatrix}\!,
    \!\begin{pmatrix}
    2\\
    0\\
    -1
    \end{pmatrix}\!
\right).
$$

以上
