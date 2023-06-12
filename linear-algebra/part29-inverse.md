---
title: Linear Algebra - Part 29 - Identity and Inverses
video: https://www.youtube.com/watch?v=JUimgJ9E4-c&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=29
---

（※行列と線形写像の対応をおさらい）

定義：$\mathbb R^{n \times n}$ における **恒等行列** を次で定義する：

$$
1_n = \!\begin{pmatrix}
1 & 0 & \dots & 0\\
0 & 1 & \dots & 0\\
0 & 0 & \ddots & 0\\
0 & 0 & \dots & 1
\end{pmatrix}\!.
$$

他の記号：
$I_n, \operatorname{id}, \operatorname{Id}, E_n.$

性質：

* ${\forall B \in \mathbb R^{n \times m} \quad 1_n B = B }$
* ${\forall A \in \mathbb R^{m \times n} \quad A 1_n = A }$

写像水準：

$f_{1_n}$ は恒等写像：

$$
\begin{aligned}
    &f_{1_n}\colon& \mathbb R^n & \longrightarrow & \mathbb R^n\\
    &       & x & \longmapsto & 1_n x = x
\end{aligned}
$$

逆行列、逆写像：

$A \in \mathbb R^{n\times n}$ に対して、
${A \tilde A \in \mathbb R^{n \times n} = \tilde AA = 1_n}$
であるような $\tilde A \in \mathbb R^{n \times n}$ が存在するとき、
この $\tilde A$ は一意に決まる。これを $A$ の **逆行列** と言い、$A^{-1}$ と書く。

定義：
行列 ${A \in \mathbb R^{n \times n}}$ が **可逆**（正則）であるとは、
対応する線形写像が全単射であることを言う。そうでなければ $A$ は **特異** であるという。

行列 $\tilde A$ が $A$ の **逆である** とは、${f_{\tilde A} = \left(f_A\right)^{-1}}$
であることを言う。これを $A^{-1}$ と書く。

まとめ：

$$
f_{A^{-1}}\circ f_A = f_A \circ f_{A^{-1}} = \operatorname{id}
\iff
A^{-1}A = AA^{-1} = 1_n.
$$

以上
