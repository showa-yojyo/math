---
title: Linear Algebra - Part 32 - Transposition for Matrices
video: https://www.youtube.com/watch?v=QzwCtPnOBJY&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=32
---

**転置** とは列と行を入れ替えることだ。

$$
\begin{aligned}
\!\begin{pmatrix}
a_1\\
\vdots\\
a_n
\end{pmatrix}^{\!\mathrm{T}}
&= \!\begin{pmatrix}
a_1 & \dots & a_n
\end{pmatrix}\!.\\

\!\begin{pmatrix}
a_1 & \dots & a_n
\end{pmatrix}^{\!\mathrm{T}}
&= \!\begin{pmatrix}
a_1\\
\vdots\\
a_n
\end{pmatrix}\!.\\

(a^{\!\mathrm{T}})^{\!\mathrm{T}} &= a.
\end{aligned}
$$

定義：
${A \in \mathbb R^{m \times n}}$ に対して
${A^{\!\mathrm{T}} \in \mathbb R^{n \times m}}$ を次で定義する：

$$
A = (a_{ij}) \implies A^{\!\mathrm{T}} = (a_{ji}).
$$

例：

$$
\!\begin{pmatrix}
1 & 2 & 0 & 1\\
2 & 0 & 3 & 0
\end{pmatrix}^{\!\mathrm{T}}
= \!\begin{pmatrix}
1 & 2\\
2 & 0\\
0 & 3\\
1 & 0
\end{pmatrix}\!.
$$

$$
\!\begin{pmatrix}
1 & 2\\
3 & 4
\end{pmatrix}^{\!\mathrm{T}}
= \!\begin{pmatrix}
1 & 3\\
2 & 4
\end{pmatrix}\!.
$$

$$
\!\begin{pmatrix}
1 & 4 & 5\\
4 & 2 & 0\\
5 & 0 & 3
\end{pmatrix}^{\!\mathrm{T}}
= \begin{pmatrix}
1 & 4 & 5\\
4 & 2 & 0\\
5 & 0 & 3
\end{pmatrix}\!.
$$

忘れるな：

$$
(AB)^{\!\mathrm{T}} = B^{\!\mathrm{T}}A^{\!\mathrm{T}}.
$$

以上
