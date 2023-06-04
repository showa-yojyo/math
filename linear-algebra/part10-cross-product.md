---
title: Linear Algebra - Part 10 - Cross Product
---

[Linear Algebra - Part 10 - Cross Product - YouTube](https://www.youtube.com/watch?v=HZM7K6MEdDU&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=10)

クロス積、ベクトル積は
写像 $\times \colon \mathbb R^3 \times \mathbb R^3 \longrightarrow \mathbb R^3$ だ。

定義：いつものように記号を用いる。クロス積を次で定義する：

$$
u \times v
= \!\begin{pmatrix}u_1 \\ u_2 \\ u_3\end{pmatrix}\! \times
  \!\begin{pmatrix}v_1 \\ v_2 \\ v_3\end{pmatrix}\!
= \!\begin{pmatrix}
u_2 v_3 - u_3 v_2\\
u_3 v_1 - u_1 v_3\\
u_1 v_2 - u_2 v_1
\end{pmatrix}\!.
$$

Levi-Civita 記号というものがある：

$$
u \times v = \sum_{i,j,k=1}^{3} \varepsilon_{ijk} u_i v_j e_k
$$

性質：

1. 直交性：${u \times v}$ は $u$ にも $v$ にも直交する。成分計算で証明される。
2. 向き：右手の法則（ビデオ参照）
3. 長さ：${\lVert u \times v \rVert}$ は $u$ と $v$ を二辺とする平行四辺形の面積に等しい。

例：実質 $\mathbb R^2$ のベクトルだが、検証しやすい。

$$
\!\begin{pmatrix} 2\\ 1\\ 0\end{pmatrix}\!
\!\begin{pmatrix} 0\\ 1\\ 0\end{pmatrix}\!
=
\!\begin{pmatrix}
1 \cdot 0 - 0 \cdot 1\\
0 \cdot 0 - 2 \cdot 0\\
2 \cdot 1 - 1 \cdot 0
\end{pmatrix}\!
=
\!\begin{pmatrix} 0\\ 0\\ 2\end{pmatrix}\!.
$$

以上
