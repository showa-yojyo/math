---
title: Linear Algebra - Part 37 - Row Operations
video: https://www.youtube.com/watch?v=3rnWqjTdQM0&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=37
---

※拡大行列のおさらいから。

行列 $A$ から行列 $\tilde A$ に変換するのは、

$$
MA = \tilde A \longleftrightarrow A = M^{-1}A
$$

連立線形方程式の場合：

$$
Ax = b \longleftrightarrow MAx = Mb
$$

例：

$$
A = \!\begin{pmatrix}
1 & 3\\
2 & -1
\end{pmatrix}
\longrightarrow
MA = \!\begin{pmatrix}
1 & 3\\
0 & -7
\end{pmatrix}\!.
$$

$$
A =
\!\begin{pmatrix}
a_{11} & \dots & a_{1n}\\
\vdots & \dots & \vdots\\
a_{m1} & \dots & a_{mn}
\end{pmatrix}\!
= \!\begin{pmatrix}
\text{\textemdash} \alpha_1^{\!\mathrm{T}} \text{\textemdash}\\
\vdots\\
\text{\textemdash} \alpha_m^{\!\mathrm{T}} \text{\textemdash}\\
\end{pmatrix}\!.
$$

$$
\begin{aligned}
c^{\!\mathrm{T}} &= \!\begin{pmatrix}
0 & \dots & 0 & c_i & 0 & \dots & 0 & c_j & \dots & 0
\end{pmatrix}\!
\\\implies
c^{\!\mathrm{T}}A &= c_i\alpha_i^{\!\mathrm{T}} + c_j\alpha_j^{\!\mathrm{T}}.
\end{aligned}
$$

例：

$$
\!\begin{pmatrix}
1 & 0 & 0\\
0 & 1 & 0\\
\lambda & 0 & 1
\end{pmatrix}\!
\!\begin{pmatrix}
\text{\textemdash} \alpha_1^{\!\mathrm{T}} \text{\textemdash}\\
\text{\textemdash} \alpha_2^{\!\mathrm{T}} \text{\textemdash}\\
\text{\textemdash} \alpha_3^{\!\mathrm{T}} \text{\textemdash}\\
\end{pmatrix}\!
=
\!\begin{pmatrix}
\text{\textemdash} \alpha_1^{\!\mathrm{T}} \text{\textemdash}\\
\text{\textemdash} \alpha_2^{\!\mathrm{T}} \text{\textemdash}\\
\text{\textemdash} \alpha_3^{\!\mathrm{T}} + \lambda \alpha_1^{\!\mathrm{T}} \text{\textemdash}
\end{pmatrix}\!.
$$

この操作行列を $Z_{3 + \lambda1}$ を呼ぼう。逆行列は
$\lambda$ を $-\lambda$ に置き換えたものだ。

定義：
${Z_{i + \lambda j} \in \mathbb R^{m \times m},\,}{i \ne j,\,}{\lambda \in \mathbb R}$
つまり $m$ 次恒等行列の $(i, j)$ 要素を $\lambda$ で置き換えた行列だ。

例：行入れ替え

$$
\!\begin{pmatrix}
0 & 0 & 1\\
0 & 1 & 0\\
1 & 0 & 0\\
\end{pmatrix}\!
\!\begin{pmatrix}
\text{\textemdash} \alpha_1^{\!\mathrm{T}} \text{\textemdash}\\
\text{\textemdash} \alpha_2^{\!\mathrm{T}} \text{\textemdash}\\
\text{\textemdash} \alpha_3^{\!\mathrm{T}} \text{\textemdash}\\
\end{pmatrix}\!
=
\!\begin{pmatrix}
\text{\textemdash} \alpha_3^{\!\mathrm{T}} \text{\textemdash}\\
\text{\textemdash} \alpha_2^{\!\mathrm{T}} \text{\textemdash}\\
\text{\textemdash} \alpha_1^{\!\mathrm{T}} \text{\textemdash}\\
\end{pmatrix}\!.
$$

最初の行列を $P{1 \leftrightarrow 3}$ と置こう。

定義：
${P_{i \leftrightarrow j} \in \mathbb R^{m \times m},\,}{i \ne j}$
つまり恒等行列の $i$ 行目と $j$ 列目を入れ替えた行列だ。

定義：行スカラー倍

$$
\!\begin{pmatrix}
d_1 & & \\
& \ddots & \\
 & & d_m\\
\end{pmatrix}\!
\!\begin{pmatrix}
\text{\textemdash} \alpha_1^{\!\mathrm{T}} \text{\textemdash}\\
\vdots\\
\text{\textemdash} \alpha_m^{\!\mathrm{T}} \text{\textemdash}\\
\end{pmatrix}\!
=
\!\begin{pmatrix}
\text{\textemdash} d_1 \alpha_1^{\!\mathrm{T}} \text{\textemdash}\\
\vdots\\
\text{\textemdash} d_m \alpha_m^{\!\mathrm{T}} \text{\textemdash}\\
\end{pmatrix}\!.
$$

ただし各 ${d_k \ne 0.}$

定義：

行操作：上記行列の有限個の積。例：
${M = Z_{3 + 71}Z_{2 + 8i}P_{1 \leftrightarrow 2}.}$

性質：行列 $A \in \mathbb R^{m \times n}$ と
正則行列 $M \in \mathbb R^{m \times m}$ に対して、

$$
\ker(MA) = \ker(A),\,
\operatorname{Ran}(MA) = M \operatorname{Ran}(A)
\coloneqq \!\left\{\left. My \,\middle|\, y \in \operatorname{Ran}(A) \right.\right\}\!.
$$

証明は宿題。

以上
