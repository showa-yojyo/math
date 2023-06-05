---
title: Linear Algebra - Part 14 - Column picture of the matrix-vector product
---

[Linear Algebra - Part 14 - Column picture of the matrix-vector product - YouTube](https://www.youtube.com/watch?v=PZyTBvc9qxQ&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=14)

${A \in \mathbb R^{m \times n} }$ を、列ベクトルを横に並べたものをみなす：

$$
A = \!\begin{pmatrix}
a_{11} & \dots & a_{1n}\\
\vdots & \dots & \vdots\\
a_{m1} & \dots & a_{mn}
\end{pmatrix}\!
=
\!\begin{pmatrix}
a_1 & \dots & a_n
\end{pmatrix}\!,\;
a_{i} \coloneqq
\!\begin{pmatrix}
a_{1i} \\
\vdots\\
a_{mi}
\end{pmatrix}\!.
$$

行列ベクトル積：

$$
\begin{aligned}
Ax &= \!\begin{pmatrix}
a_1 & \dots & a_n
\end{pmatrix}\!
\!\begin{pmatrix}
x_1 \\
\vdots \\
x_n\\
\end{pmatrix}\\
&= x_1a_1 + \dotsb + x_na_n.
\end{aligned}
$$

定義：行列 $A$ から定まる写像 $f_A$ を次で定義する：

$$
f_A \colon \mathbb R^n \longrightarrow \mathbb R^m,\;x \longmapsto Ax
$$

線形写像。

以上
