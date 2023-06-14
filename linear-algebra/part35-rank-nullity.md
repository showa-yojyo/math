---
title: Linear Algebra - Part 35 - Rank-Nullity Theorem
video: https://www.youtube.com/watch?v=Ia6J9uwGWgw&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=35
---

${m \times n}$ 実行列を $A$ とする。

$$
\begin{aligned}
\operatorname{rank}(A) &\coloneqq \dim(\operatorname{Ran}(A))\\
&= \dim(\operatorname{span}(a_1, \dotsc, a_n))\\
&\le \min(n, m).
\end{aligned}
$$

${\operatorname{rank}(A) = \min(n, m)}$ ならば $A$ が full rank を持つ。

例：

$$
\text{(a)}\quad
A = \!\begin{pmatrix}
1 & 2 & 0 & 0
\end{pmatrix}\!,\,
\operatorname{rank}(A) = 1.
$$

$$
\text{(b)}\quad
A = \!\begin{pmatrix}
2 & 2 & -4\\
1 & 0 & -1
\end{pmatrix}\!,\,
\operatorname{rank}(A) = 2.
$$

一列目と二列目が線形独立なのでランクは 2 とわかる。

（※謎のイラスト）

定義：

$$
\operatorname{nullity}(A) \coloneqq \dim(\ker(A)).
$$

Rank-nullity 定理：

$$
\dim(\ker(A)) + \dim(\operatorname{Ran}(A)) = n.
$$

（※定義域の次元がある意味で保存される）

証明：
${k = \dim(\ker(A))}$ とおく。
$\ker(A)$ の基底を選ぶ：
${(b_1, \dotsc, b_k).}$

Steinitz exchange lemma により、
${(b_1, \dotsc, b_k, c_1, \dotsc, c_r)}$ を $\mathbb R^n$ の基底にできる。
ここで ${r = n - k.}$

$$
\begin{aligned}
\operatorname{Ran}(A)
&= \operatorname{span}(Ab_1, \dotsc, Ab_k, \dotsc, Ac_1, \dotsc, Ac_r)\\
&= \operatorname{span}(0, \dotsc, 0, \dotsc, Ac_1, \dotsc, Ac_r).
\end{aligned}
$$

ゆえに ${\dim(\operatorname{Ran}(A)) \le r.}$

次に $(Ac_1, \dotsc, Ac_r)$ が線形独立であることを示す。

$$
\begin{aligned}
\lambda_1Ac_1 + \dotsb + \lambda_r A c_r = 0\\
\therefore A\left(\sum_{i=1}^r \lambda_i c_i\right) = 0\\
\therefore \sum_{i=1}^r \lambda_i c_i \in \ker(A).
\end{aligned}
$$

左辺のベクトルは核の基底の線形結合に書ける。
したがって、ある ${\mu_1, \dotsc, \mu_k \in \mathbb R}$ があって：

$$
\begin{aligned}
    \sum_{i=1}^{r}\lambda_i c_i = \sum_{j=1}^{k}\mu_j b_j.\\
    \sum_{i=1}^{r}\lambda_i c_i + \sum_{j=1}^{k}(-\mu_j)b_j = 0.\\
    \therefore \lambda_1 = \dotsb = \lambda_r = 0.
\end{aligned}
$$

$(Ac_1, \dotsc, Ac_r)$ が線形独立であることが示された。
ゆえに ${\dim(\operatorname{Ran}(A)) = r.}$

以上
