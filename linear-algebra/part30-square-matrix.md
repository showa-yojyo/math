---
title: Linear Algebra - Part 30 - Injectivity, Surjectivity for Square Matrices
video: https://www.youtube.com/watch?v=r3RVsfgZOZo&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=30
---

連立線形方程式 ${Ax = b}$ を考える。
$A$ の逆行列が存在すれば、解を次のようにして求められるか：

$$
\begin{aligned}
    Ax &= b\\
    A^{-1}Ax &= A^{-1}b\\
    x &= A^{-1}b.
\end{aligned}
$$

定理：
$A$ を正方行列とし、写像 $f_A$ を $A$ が誘導する写像とする。
このとき $f_A$ が単射であることと $f_A$ が全射であることが同値である。

証明：$(\implies)$
$f_A$ が単射であるとする。$\mathbb R^n$ の正規基底ベクトルに対する各像の族を考える：

$$
(f_A(e_1), \dotsc, f_A(e_n)).
$$

これもまた線形独立である。

（※これを示すのは容易だと言っている。線形結合と $0$ を比較？）

ゆえに、像の族は $\mathbb R^n$ の基底であり、$\mathbb R^n$ を張る。
したがって $f_A$ は全射である。

（※ ${\forall y \in \mathbb R^n}{\exists \mu_1, \dotsc, \mu_n \in \mathbb R:}\:{y = \sum \mu_j f_A(e_j)}$
とすると $y$ は ${\sum \mu_j e_j \in \mathbb R^n}$ の像）

$(\impliedby)$
$f_A$ が全射であるとする。任意の $y \in \mathbb R^n$ に対して
$f_A(x) = y$ なる $x \in \mathbb R^n$ が存在する。

$$
x = x_1 e_1 + \dotsb + x_n e_n
$$

と書けるので、

$$
y = f_A(x) = x_1 f_A(e_1) + \dotsb + x_n f_A(x_n).
$$

ゆえに $(f_A(e_1), \dotsc, f_A(e_n))$ は $\mathbb R^n$ を張る。
ベクトルがちょうど $n$ 個あるので、このベクトル族は線形独立である。

${f_A(x) = f_A(\tilde x)}$ と仮定すると ${f_A(x - \tilde x) = 0.}$
${x - \tilde x}$ の成分を $v_i$ と書くと：

$$
v_1 f_A(e_1) + \dotsb + v_n f_A(e_n) = 0.
$$

各ベクトルが線形独立であることから

$$
v_1 = \dotsb = v_n = 0.
$$

ゆえに ${x = \tilde x.}$ したがって $f_A$ は単射であることが示された。

以上
