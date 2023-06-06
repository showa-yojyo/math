---
title: Linear Algebra - Part 17 - Properties of the matrix product
---

[Linear Algebra - Part 17 - Properties of the matrix product - YouTube](https://www.youtube.com/watch?v=BqcxYCM19Wo&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=17)

$$
\begin{aligned}
\mathbb R^{m\times n} \times \mathbb R^{n\times k} & \longrightarrow & \mathbb R^{m\times k}\\
(A, B) & \longmapsto & AB
\end{aligned}
$$

は次で定義される：

$$
(AB)_{ij} = \sum_{l = 1}^{n}a_{il}b_{lj}.
$$

性質：演算が可能な行列の組み合わせについて：

$$
\begin{aligned}
&\text{(a)} & (A + B)C &= AC + BC\\
&& D(A + B) &= DA + DB\\
&\text{(b)}& \lambda(AB) &= (\lambda A)B = A(\lambda B)\\
&\text{(c)}& (AB)C &= A(BC)
\end{aligned}
$$

証明：やや複雑な最後の等式だけ示す。

$$
\begin{aligned}
((AB)C)_{ij} &= \sum_{l=1}^{n}(AB)_{il}C_{lj}\\
&= \sum_{l}^{}\left(\sum_{z}^{}a_{iz}b_{zl}\right)c_{lj}\\
&= \sum_z a_{iz} \sum_l b_{zl}{c_lj}\\
&= \sum_z a_{iz}(BC)_{zj}\\
&= (A(BC))_{ij}.
\end{aligned}
$$

重要：可換則は一般には成り立たない

（※反例を簡単に見つけられる）

以上
