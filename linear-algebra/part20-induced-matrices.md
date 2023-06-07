---
title: Linear Algebra - Part 20 - Linear maps induce matrices
---

[Linear Algebra - Part 20 - Linear maps induce matrices - YouTube](https://www.youtube.com/watch?v=9UcgdR_X2Ys&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=20)

線形写像 ${f \colon \mathbb R^n \longrightarrow \mathbb R^m}$

${x = x_1e_1 + \dotsb + x_n e_n}$ のように正規単位ベクトルの和に書いておく。

$$
\begin{aligned}
f(x)
&= f(x_1e_1 + \dotsb + x_ne_n)\\
&= x_1f(e_1) + \dotsb + x_nf(x_n).
\end{aligned}
$$

$f(x)$ を得るには $f(e_1), \dotsc, f(e_n)$ を知れば十分だとわかる。

命題：線形写像 ${f \colon \mathbb R^n \longrightarrow \mathbb R^m}$ において、
${f = f_A}$ である行列 $A \in \mathbb R^{m \times n}$ がただひとつ存在して、

$$
A = \!\begin{pmatrix}
f(e_1) & \dots & f(e_n)
\end{pmatrix}\!.
$$

存在性の証明：

$$
\def\x{ \!\begin{pmatrix}
x_1\\
\vdots\\
x_n
\end{pmatrix}\! }

\begin{aligned}
f_A(x) &= f_A\left(\x\right)
= A\x\\
&= \!\begin{pmatrix}
f(e_1) & \dots & f(e_n)
\end{pmatrix}\!
\x\\
&= x_1 \!\begin{pmatrix}
f(e_1)
\end{pmatrix}\! + \dotsb + x_n\!\begin{pmatrix}
f(e_n)
\end{pmatrix}\!\\
&= f(x).
\end{aligned}
$$

一意性の証明：
${A, B \in \mathbb R^{m \times n}}$ が ${f = f_A = f_B}$ であるとする。
このとき

$$
\begin{aligned}
& \forall x \in \mathbb R^n (Ax = Bx)\\
\implies & \forall x \in \mathbb R^n ((A - B)x = 0)\\
\implies & A - B = 0\\
& \therefore A = B.
\end{aligned}
$$

以上
