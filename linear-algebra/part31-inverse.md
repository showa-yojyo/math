---
title: Linear Algebra - Part 31 - Inverses of Linear Maps are Linear
video: https://www.youtube.com/watch?v=u6IrirgCuTw&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=31
---

※線形写像の合成の逆写像を考える

$A, B$ を $n$ 次正則行列とする。

$$
f_{B^{-1}}\circ f_{A^{-1}} = (f_{AB})^{-1} \implies
(AB)^{-1} = B^{-1}A^{-1}.
$$

重要な事実：
写像 ${f \colon \mathbb R^n \longrightarrow \mathbb R^n}$ が線形かつ全単射であるならば
逆写像 ${f^{-1}:\mathbb R^n \longrightarrow \mathbb R^n}$ もまた線形である。

証明：
${f(x) = y}$ となる $x, y$ は一意に存在する。${\lambda \in \mathbb R}$ としてスカラー倍の逆像は：

$$
\begin{aligned}
    f^{-1}(\lambda y)
    &= f^{-1}(\lambda f(x))\\
    &= f^{-1}(f(\lambda x))\\
    &= \lambda x\\
    &= \lambda f^{-1}(y).
\end{aligned}
$$

逆像のスカラー倍になっている。

${f(\tilde x) = \tilde y}$ となる $\tilde x, \tilde y$ を取る。和の逆像は：

$$
\begin{aligned}
    f^{-1}(y + \tilde y)
    &= f^{-1}(f(x) + f(\tilde x))\\
    &= f^{-1}(f(x + \tilde x))\\
    &= x + \tilde x\\
    &= f^{-1}(y) + f^{-1}(\tilde y).
\end{aligned}
$$

逆像の和になっている。

これで $f^{-1}$ は線形写像であることが示された。

以上
