---
title: Linear Algebra - Part 23 - Linear Independence (Examples)
---

[Linear Algebra - Part 23 - Linear Independence (Examples) - YouTube](https://www.youtube.com/watch?v=Xdx0ZG7T648&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=23)

線形独立の定義の確認をしてから例を挙げる。

例：

$\text{(a)}$ 単一のベクトルからなるベクトル族 $(v^{1})$ は $v^{(1)} \ne 0$ ならば線形独立。

（※逆も成り立つ）

$\text{(b)}$ $(0, v^{2}, \dotsc, v^{k})$ は線形従属。
$\because \lambda_1 = 1, \lambda_2 = \dotsb = \lambda_k = 0.$

$\text{(c)}$ 次の族は線形従属：

$$
\left(
    \!\begin{pmatrix}
    1\\
    0\\
    \end{pmatrix}\!,
    \!\begin{pmatrix}
    1\\
    1\\
    \end{pmatrix}\!,
    \!\begin{pmatrix}
    0\\
    1\\
    \end{pmatrix}\!
\right).
$$

$$
\because \!\begin{pmatrix}
    1\\
    0\\
    \end{pmatrix}\! -
    \!\begin{pmatrix}
    1\\
    1\\
    \end{pmatrix}\! -
    \!\begin{pmatrix}
    0\\
    1\\
    \end{pmatrix}\! = 0.
$$

$\text{(d)}$ 正規単位ベクトルからなる族 $(e_1, \dotsc, e_n),$ ${e_i \in \mathbb R^n}$
は線形独立。

$\text{(e)}$ 正規単位ベクトルすべての族に任意のベクトルを含めた族
$(e_1, \dotsc, e_n, v),$ ${e_i, v \in \mathbb R^n}$ は線形従属。

事実：
$(v^{(1)}, \dotsc, v^{(k)}),$ $v^{(j)} \in \mathbb R^n$ は線形従属
$\iff$
ある $l$ があって次が成り立つ：

$$
\operatorname{span}(v^{(1)}, \dotsc, v^{(k)})
= \operatorname{span}(v^{(1)}, \dotsc, v^{(l - 1)}, v^{(l + 1)}, \dotsc, v^{(k)}).
$$

（※ベクトル族が生成する部分空間が等しい）

以上
