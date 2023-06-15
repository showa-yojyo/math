---
title: Linear Algebra - Part 39 - Gaussian Elimination
video: https://www.youtube.com/watch?v=VpYdBHdgq_U&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=39
---

Gauss の消去法

${Ax = b}$ を解くのに、$(A | b)$ に対して適切な行操作を繰り返し適用し、まず上三角行列に至らせる。
それから後方置換という計算法を適用し、最終的に右列のベクトルが解になる。

例：

$$
\begin{cases}
2 x_1 + 3 x_2 - 1 x_3 &= 4\\
2 x_1 - 1 x_2 + 7 x_3 &= 0\\
6 x_1 + 13x_2 - 4 x_3 &= 9\\
\end{cases}
$$

$$
\begin{aligned}
\left(\hspace{-4pt}
\begin{array}{ccc|c}
2 & 3 & -1 & 4\\
2 & -1 & 7 & 0\\
6 & 13 & -4 & 9\\
\end{array}
\hspace{-4pt}\right)
\begin{matrix}
\\
-1\cdot I\\
-3\cdot I\\
\end{matrix}
&\longrightarrow
\left(\hspace{-4pt}
\begin{array}{ccc|c}
2 & 3 & -1 & 4\\
0 & -4 & 8 & -1\\
0 & 4 & -1 & -3\\
\end{array}
\hspace{-4pt}\right)
\begin{matrix}
\\
\\
+1 \cdot II\\
\end{matrix}\\
&\longrightarrow
\left(\hspace{-4pt}
\begin{array}{ccc|c}
2 & 3 & -1 & 4\\
0 & -4 & 8 & -4\\
0 & 0 & 7 & -1
\end{array}
\hspace{-4pt}\right)\\
&\longrightarrow\text{backward substitution...}\\
&\longrightarrow
x_3 = -1,\,
x_2 = -1,\,
x_1 = 3.
\end{aligned}
$$

解の集合は：

$$
S = \!\left\{\left. \!\begin{pmatrix}
3\\
-1\\
-1\\
\end{pmatrix}\!\right.\right\}\!.
$$

Gaussian elimination:

$$
\begin{aligned}
&\left(\hspace{-4pt}
\begin{array}{ccc|c}
a_{11} & \dots & a_{1n} & b_1\\
\vdots & \ddots & \vdots & \vdots\\
a_{m1} & \dots & a_{mn} & b_m\\
\end{array}
\hspace{-4pt}\right)
=
\!\begin{pmatrix}
\text{\textemdash} \alpha_1^{\!\mathrm{T}} \text{\textemdash}\\
\vdots\\
\text{\textemdash} \alpha_m^{\!\mathrm{T}} \text{\textemdash}\\
\end{pmatrix}\!\\
\longrightarrow&

\def\arraystretch{1.75}
\!\begin{pmatrix}
\alpha_1^{\!\mathrm{T}}\\
\alpha_2^{\!\mathrm{T}} - \dfrac{a_{21}}{a_{11}}\alpha_1^{\!\mathrm{T}}\\
\vdots\\
\alpha_m^{\!\mathrm{T}} - \dfrac{a_{21}}{a_{11}}\alpha_1^{\!\mathrm{T}}\\
\end{pmatrix}\!\\
\longrightarrow& \text{continue iteratively...}\\
\longrightarrow& \dots \text{row echelon form}
\end{aligned}
$$

次回は row echelon form をやる。

以上
