---
title: Linear Algebra - Part 33 - Transpose and Inner Product
video: https://www.youtube.com/watch?v=YCs_1qYxs2Q&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=33
---

※転置行列のおさらいから

$\mathbb R^n$ の標準内積 ${\left\langle u,\;v \right\rangle \in \mathbb R.}$

$$
\left\langle u,\;v \right\rangle = u^{\!\mathrm{T}}v.
$$

命題： $m \times n$ 行列 $A$ と ${x \in \mathbb R^n,}$
${y \in \mathbb R^m}$ に対して：

$$
\left\langle y,\;Ax \right\rangle = \left\langle A^{\!\mathrm{T}}y,\;x \right\rangle.
$$

左辺と右辺はそれぞれ $\mathbb R^m, \mathbb R^n$ の内積だ。

証明：

※今回最初の等式と前回の最後の注意を組み合わせる。

$$
\begin{aligned}
    \left\langle y,\;Ax \right\rangle
    &= y^{\!\mathrm{T}}(Ax)\\
    &= (y^{\!\mathrm{T}}A)x\\
    &= (A^{\!\mathrm{T}}y)^{\!\mathrm{T}}x\\
    &= \left\langle A^{\!\mathrm{T}}y,\;x \right\rangle.
\end{aligned}
$$

別の定義：
$A^{\!\mathrm{T}}$ は次を満たすただ一つの $n \times m$ 行列 $B$ である：

$$
\forall x, y \left(
\left\langle y,\;Ax \right\rangle
= \left\langle By,\;x \right\rangle\right).
$$

以上
