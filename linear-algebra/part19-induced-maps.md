---
title: Linear Algebra - Part 19 - Matrices induce linear maps
---

[Linear Algebra - Part 19 - Matrices induce linear maps - YouTube](https://www.youtube.com/watch?v=19-YrCB3hyo&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=19)

${A \in \mathbb R^{m\times n}}$ は写像を規定する：
${f_A \colon \mathbb R^n \longrightarrow \mathbb R^m,\;x \longmapsto Ax.}$

命題：
$f_A$ が線形写像である：

$$
\begin{aligned}
f_A(x + y) &= f_A(x) + f_A(y), & A(x + y) &= Ax + Ay.\\
f_A(\lambda x) &= \lambda f_A(x), & A(\lambda x) &= \lambda (Ax).
\end{aligned}
$$

例：
$a_1,a_2$ を列ベクトル、$x_1,x_2,y_1,y_2$ をスカラーとして：

$$
\begin{aligned}
\!\begin{pmatrix}a_1 & a_2\end{pmatrix}\!
\left(\!\begin{pmatrix}
x_1\\
x_2\\
\end{pmatrix}\!
+
\!\begin{pmatrix}
y_1\\
y_2\\
\end{pmatrix}\!
\right)
&=
\!\begin{pmatrix}a_1 & a_2\end{pmatrix}\!
\left(\!\begin{pmatrix}
x_1 + y_1\\
x_2 + y_2\\
\end{pmatrix}\!
\right)\\
&=
\!\begin{pmatrix}a_1\end{pmatrix}\!
\left(\!\begin{pmatrix}
x_1 + y_1\\
x_2 + y_2\\
\end{pmatrix}\!
\right)
+
\!\begin{pmatrix}a_2\end{pmatrix}\!
\left(\!\begin{pmatrix}
x_1 + y_1\\
x_2 + y_2\\
\end{pmatrix}\!
\right)\\
&=
\!\begin{pmatrix}a_1\end{pmatrix}\!x_1
+ \!\begin{pmatrix}a_2\end{pmatrix}\!x_2
+ \!\begin{pmatrix}a_1\end{pmatrix}\!y_1
+ \!\begin{pmatrix}a_2\end{pmatrix}\!y_2\\
&=
\!\begin{pmatrix}a_1 & a_2\end{pmatrix}\!\!\begin{pmatrix}
x_1\\
x_2\\
\end{pmatrix}\!
+ \!\begin{pmatrix}a_1 & a_2\end{pmatrix}\!\!\begin{pmatrix}
y_1\\
y_2\\
\end{pmatrix}\!.
\end{aligned}
$$

行列 $A$ と抽象的な線形写像 $f_A$ は双方向の関係がある。
今回は行列から線形写像が導かれることを示している。

${A \in \mathbb R^{m \times k},}\;{B \in \mathbb R^{k \times n}}$
ならば ${AB \in \mathbb R^{m \times n}}$ であり、
合成写像：

$$
f_A \circ f_B\colon \mathbb R^n \longrightarrow \mathbb R^m
$$

を表現する行列であると考えられる：

$$
(f_A \circ f_B)(x)
\coloneqq f_A(f_B(x))
= f_A(Bx)
= A(Bx)
= (AB)x.
$$

したがって ${f_A \circ f_B = f_{AB}}$ と書いたとしても自然だ。

以上
