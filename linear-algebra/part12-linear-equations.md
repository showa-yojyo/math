---
title: Linear Algebra - Part 12 - Systems of Linear Equations
---

[Linear Algebra - Part 12 - Systems of Linear Equations - YouTube](https://www.youtube.com/watch?v=740F1l5E8Cc&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=12)

例：

$$
\begin{cases}
x &= y + 2\\
x + y &= 40
\end{cases}
$$

例：

$$
\begin{aligned}
2x_1 - 3x_2 + 4x_3 &= -7\\
-3x_1 + x_2 - x_3 &= 0\\
20x_1 + 10x_2 &= 80\\
10x_2 + 25x_3 &= 90
\end{aligned}
$$

線形方程式：
$C_1, \dotsc, C_n, C$ を定数とする。次の形の方程式のことを言う：

$$
C_1 x_1 + C_2 x_2 + \dotsb + C_n x_n = C.
$$

定義：

連立線形方程式：

$$
\begin{aligned}
a_{11}x_1 + \dotsb + a_{1n}x_n &= b_1\\
\vdots &= \vdots\\
a_{m1}x_1 + \dotsb + a_{mn}x_n &= b_m\\
\end{aligned}
$$

解：すべての方程式を満たす $x_1, \dotsc, x_n$ を解という。

* 解がない可能性がある。
* 一意の解がある可能性がある。
* たくさんの解がある可能性がある。

連立線形方程式を次のように書き表す：

$$
Ax = b, A = \!\begin{pmatrix}
a_{11} & \dots & a_{1n}\\
\vdots & \dots & \vdots\\
a_{m1} & \dots & a_{mn}
\end{pmatrix}\!,\;
b = \!\begin{pmatrix}
b_1\\
\vdots\\
b_m
\end{pmatrix}\!,\;
x = \!\begin{pmatrix}
x_1\\
\vdots\\
x_n
\end{pmatrix}\!.
$$

例：さっきの連立方程式は：

$$
\!\begin{pmatrix}
2 & -3 & 4\\
-3 & 1 & -1\\
20 & 10 & 0\\
0 & 10 & 25
\end{pmatrix}\!
\!\begin{pmatrix}
x_1\\
x_2\\
x_3
\end{pmatrix}\!
=
\!\begin{pmatrix}
-7\\
0\\
80\\
90
\end{pmatrix}\!.
$$

この左辺の乗算の意味はさっきの連立方程式の左辺をまとめたものとみなす。

以上

