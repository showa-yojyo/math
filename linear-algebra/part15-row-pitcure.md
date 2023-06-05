---
title: Linear Algebra - Part 15 - Row Picture
---

[Linear Algebra - Part 15 - Row Picture - YouTube](https://www.youtube.com/watch?v=g1qLd_1F10Q&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=15)

${A \in \mathbb R^{m \times n} }$ を、行ベクトルを縦に並べたものとみなす。

今度は

$$
A = \!\begin{pmatrix}
a_{11} & \dots & a_{1n}\\
\vdots & \dots & \vdots\\
a_{m1} & \dots & a_{mn}
\end{pmatrix}\!
=
\!\begin{pmatrix}
\alpha_1^{\;\mathrm T}\\
\vdots\\
\alpha_m^{\;\mathrm T}
\end{pmatrix}\!,\;
\alpha_{i}^{\;\mathrm T} \coloneqq
\!\begin{pmatrix}
a_{i1} & \dots & a_{in}
\end{pmatrix}\!.
$$

${}^{\mathrm T}$ は **転置** という：

$$
u^{\mathrm{T}}
= \!\begin{pmatrix}
u_1 \\
\vdots \\
u_n
\end{pmatrix}^{\!\mathrm{T}}
=
\!\begin{pmatrix}u_1 & \dots & u_n\end{pmatrix}\!.
$$

${x \in \mathbb R^n}$ に対して $u^{\mathrm T}x$ が定義される。

例：

$$
\!\begin{pmatrix}1 & 3 & 5\end{pmatrix}\!
\!\begin{pmatrix}
2\\
4\\
6
\end{pmatrix}\!
= 1 \cdot 2 + 3 \cdot 4 + 5 \cdot 6.
$$

内積とみなせる。

$$
u, v \in \mathbb R^n:
u^{T}v = \left\langle u,\;v \right\rangle.
$$

行列ベクトル積：

$$
\!\begin{pmatrix}
\alpha_1^{\;\mathrm T}\\
\vdots\\
\alpha_m^{\;\mathrm T}
\end{pmatrix}\!
\!\begin{pmatrix}
x
\end{pmatrix}\!
= \!\begin{pmatrix}
\alpha_1^{\;\mathrm T}x \\
\vdots\\
\alpha_m^{\;\mathrm T}x \\
\end{pmatrix}\!
$$

例：

$$
\!\begin{pmatrix}
2 & 1 & 2\\
3 & 2 & 1
\end{pmatrix}\!
\!\begin{pmatrix}
3\\
1\\
0
\end{pmatrix}\!
= \!\begin{pmatrix}
2 \cdot 2 + 1 \cdot 1 + 2 \cdot 0\\
3 \cdot 3 + 2 \cdot 1 + 1 \cdot 0
\end{pmatrix}\!
=
\!\begin{pmatrix}
7\\
11
\end{pmatrix}\!.
$$

以上
