---
title: Linear Algebra - Part 16 - Matrix Product
---

[Linear Algebra - Part 16 - Matrix Product - YouTube](https://www.youtube.com/watch?v=8R0BdG9XnAk&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=16)

行列同士の乗算を定義する。

${A \in \mathbb R^{m \times n},\;b \in \mathbb R^n \implies Ab \in \mathbb R^m.}$

${A \in \mathbb R^{m \times n},\;b_1, \dotsc, b_k \in \mathbb R^n \implies Ab_1, \dotsc, Ab_k \in \mathbb R^m.}$

$$
A\!\begin{pmatrix}
b_1 & \dotsb & b_k
\end{pmatrix}\!
\coloneqq
\!\begin{pmatrix}
Ab_1 & \dots & Ab_k
\end{pmatrix}\!.
$$

定義：
${A \in \mathbb R^{m \times n}}$ と ${B \in \mathbb R^{n \times k}}$ に対して、
行列積が定義され：

$$
AB = 
\!\begin{pmatrix}
\alpha_1^{\;\mathrm{T}}\\
\vdots\\
\alpha_m^{\;\mathrm{T}}
\end{pmatrix}\!
\!\begin{pmatrix}
b_1 & \dots & b_k
\end{pmatrix}\!
=
\!\begin{pmatrix}
\alpha_1^{\;\mathrm{T}}b_1 & \dots & \alpha_1^{\;\mathrm{T}}b_k\\
\vdots & \ddots & \vdots\\
\alpha_m^{\;\mathrm{T}}b_1 & \dots & \alpha_m^{\;\mathrm{T}}b_k
\end{pmatrix}\!.
$$

例：ビデオのイラストがわかりやすい。
$A$ と $B$ をそれぞれ矩形の左と上に書いて内積を埋めていくと紛れがない。
（これを LaTeX で書けないか？）

$$
\!\begin{pmatrix}
1 & 2 & 3\\
4 & 5 & 6
\end{pmatrix}\!
\!\begin{pmatrix}
1 & 0\\
0 & 1\\
1 & 1
\end{pmatrix}\!
=
\!\begin{pmatrix}
1\cdot1 + 2 \cdot 0 + 3 \cdot 1 & 1\cdot 0 + 2 \cdot 1 + 3 \cdot 1\\
4 \cdot 1 + 5 \cdot 0 + 6 \cdot 1 & 4 \cdot 0 + 5 \cdot 1 + 6 \cdot 1
\end{pmatrix}\!.\\
$$

以上
