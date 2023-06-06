---
title: Linear Algebra - Part 18 - Linear Maps (Definition)
---

[Linear Algebra - Part 18 - Linear Maps (Definition) - YouTube](https://www.youtube.com/watch?v=Xi-HknrH6OM&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=18)

ベクトル空間の構造（加法およびスカラー倍）を保存する写像。

定義：${f \colon \mathbb R^n \longrightarrow \mathbb R^m}$ が線形であるとは、
${\forall x, y \in \mathbb R^n,\;\lambda \in \mathbb R:}$

$$
\begin{aligned}
& \text{(a)} & f(x + y) &= f(x) + f(y)\\
& \text{(b)} & f(\lambda x) &= \lambda f(x)
\end{aligned}
$$

を満たす場合を言う。

例：

${f \colon \mathbb R \longrightarrow \mathbb R,\;f(x) = x}$ は線形。

${f \colon \mathbb R \longrightarrow \mathbb R,\;f(x) = x^2}$ は線形でない。
${x = 1,}\;{\lambda = 3}$ を確認すれば線形の要件を満たしていないことを確認できる。

${f \colon \mathbb R \longrightarrow \mathbb R,\;f(x) = x + 1}$ は線形でない。
${\lambda = 0}$ を確認すればわかる（※グラフは直線だが線形でない）。

以上
