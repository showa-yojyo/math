---
title: Linear Algebra - Part 38 - Set of Solutions
video: https://www.youtube.com/watch?v=K9AnooBsjz4&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=38
---

解の集合：
$A$ を $m \times n$ 行列とする。
方程式 ${Ax = b}$ の解 $\tilde x$ は ${A\tilde x = b}$ を満たす。

方程式に解が存在するためには ${b \in \operatorname{Ran}(A)}$ が必要。

解が一意に存在するには ${\ker(A) = \{0\}}$ が必要。

命題：
連立線形方程式 ${Ax = b}$ に対して、解の集合

$$
S \coloneqq \!\left\{\left. \tilde x\,\middle|\, A\tilde x = b \right.\right\}\!
$$

は affine 部分空間である（空集合の場合もある）：

$$
S = \varnothing\ \lor\ \exists v_0 \in \mathbb R^n:\:S = v_0 + \ker(A)
\coloneqq \!\left\{\left. v_0 + x_0 \,\middle|\, x_0 \in \ker(A) \right.\right\}\!.
$$

証明：
${v_0 \in S}$ を仮定すると ${Av_0 = b.}$
$\forall x_0 \in \mathbb R^n$ に対して
${\tilde x \coloneqq v_0 + x_0}$ とおく。このとき

$$
\tilde x \in S \iff A\tilde x = b
\iff Av_0 + Ax_0 = b
\iff Ax_0 = 0.
\iff x_0 \in \ker(A).\ \square
$$

忘れるな：行操作は解の集合を変えない。

$$
S = v_0 + \ker(A) = v_0 + \ker(MA).
$$

この考えが Gausiaan 消去法：

* $b \in \operatorname{Ran}(A)$ を決める
* 特定の解 $v_0$ を与える
* $\ker(A)$ を与える

の基本だ。

以上
