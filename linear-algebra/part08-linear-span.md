---
title: Linear Algebra - Part 8 - Linear Span
---

[Linear Algebra - Part 8 - Linear Span - YouTube](https://www.youtube.com/watch?v=h7JpJfAcFFk&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=8)

linear span / linear hull / span

$$\operatorname{span}(M)$$

* 線形部分空間
* $M$ のベクトルの線形結合すべてを含む
* この性質である最小の部分空間

定義：$M \subset \mathbb R$ に対して

$$
\operatorname{span}(M) \coloneqq
\begin{cases}
\!\left\{\left. u \in \mathbb R^n\,\middle|\,
\exists \lambda_j \in \mathbb R
\exists u^{(j)} \in M:
u = \sum_{j=1}^{k}\lambda_k u^{(j)} \right.\right\}\!, & M \ne \varnothing,\\
\{0\}, & M = \varnothing.
\end{cases}
$$

例：
$\text{(a)}$
${\left\{\begin{pmatrix}1 \\ 1\end{pmatrix}\right\} \subset \mathbb R^2}$

$$
\def\u{ \begin{pmatrix}1 \\ 1\end{pmatrix} }
\begin{aligned}
\operatorname{span}(M)
&= \!\left\{\left. u \in \mathbb R^2\,\middle|\, 
\exists \lambda \in \mathbb R:
u = \lambda\u \right.\right\}\\
&= \!\left\{\left. \lambda\u \,\middle|\, 
\lambda \in \mathbb R
\right.\right\}\\
&= \mathbb R\u.
\end{aligned}
$$

これは原点と点 ${(1, 1)}$ を通過する直線だ。


$\text{(b)}$
$\!\left\{\begin{pmatrix}1 \\ 1 \\ 0\end{pmatrix}\!, \begin{pmatrix}1 \\ 0 \\ 0\end{pmatrix}\right\}\! \subset \mathbb R^3$

$$
\operatorname{span}\left(
   \begin{pmatrix}1 \\ 1 \\ 0\end{pmatrix},
   \begin{pmatrix}1 \\ 0 \\ 0\end{pmatrix}
\right)
= \!\left\{\left.
    \begin{pmatrix}x \\ y \\ 0\end{pmatrix}
    \,\middle|\,
    x, y \in \mathbb R
\right.\right\}\!.
$$

これらのベクトルによって生成される部分空間であると言う。

例：
${\mathbb R^n = \operatorname{span}(e_1, \dotsc, e_n)}$

以上
