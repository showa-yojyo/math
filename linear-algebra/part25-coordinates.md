---
title: Linear Algebra - Part 25 - Coordinates with respect to a Basis
---

[Linear Algebra - Part 25 - Coordinates with respect to a Basis - YouTube](https://www.youtube.com/watch?v=6cG9CMC89gg&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=25)

（※部分空間の基底をおさらい）

ベクトルの成分（座標）は基底の取り方による。

座標：
${U \subset \mathbb R^n}$ を部分空間、
${B = (v^{(1)}, \dotsc, v^{(k)})}$ を $U$ の基底とする。
このとき、どんなベクトル $u \in U$ も線形結合の形に書くことが可能：

$$
u = \lambda_x v^{(1)} + \dotsb + \lambda_k v^{(k)}, \lambda_j \in \mathbb R.
$$

これらの $\lambda_j$ は一意に定まり、これを $u$ の $B$ に関する **座標** という。
つまり次の記法が成り立つ：

$$
u = \!\begin{pmatrix}
\lambda_1\\
\vdots\\
\lambda_k
\end{pmatrix}\!.
$$

例：

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

$$
u = \!\begin{pmatrix}
1\\
2\\
-1
\end{pmatrix}\!
= 1 \cdot \!\begin{pmatrix}
    -3\\
    0\\
    0
\end{pmatrix}\!
+ 2 \cdot \!\begin{pmatrix}
    1\\
    1\\
    0
\end{pmatrix}\!
+ 1 \cdot \!\begin{pmatrix}
    2\\
    0\\
    -1
\end{pmatrix}\!.
$$

$$
\tilde{u} =
\!\begin{pmatrix}
3\\
0\\
0
\end{pmatrix}\!
= -1 \cdot
\!\begin{pmatrix}
    -3\\
    0\\
    0
\end{pmatrix}\!
+ 0 \cdot \!\begin{pmatrix}
    1\\
    1\\
    0
\end{pmatrix}\!
+ 0 \cdot \!\begin{pmatrix}
    2\\
    0\\
    -1
\end{pmatrix}\!.
$$

以上
