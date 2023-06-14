---
title: Linear Algebra - Part 34 - Range and Kernel of a Matrix
video: https://www.youtube.com/watch?v=yWSwuk1kiyE&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=34
---

${m \times n}$ 実行列を $A$ とし、その誘導写像を ${f_A \colon \mathbb R^n \longrightarrow \mathbb R^m}$ とする。
つまり ${f_A(x) = Ax.}$

$$
\operatorname{Ran}(A) \coloneqq \!\left\{\left. Ax \,\middle|\, x \in \mathbb R^n \right.\right\}\!
\subset \mathbb R^m
$$

を $A$ の **値域** だとか **像** だとか言う。
${\operatorname{Ran}(A) = \operatorname{Ran}(f_A).}$

$$
\ker(A) \coloneqq \!\left\{\left. x \in \mathbb R^m\,\middle|\, Ax = 0 \right.\right\}\!
$$

を $A$ の **核** だとか **零空間** だとか言う。
${\ker(A) = f^{-1}_A(\{0\}).}$

* $\operatorname{Ran}(A)$ は $\mathbb R^m$ の部分空間。
* $\ker(A)$ は $\mathbb R^n$ の部分空間。

忘れるな：
$A = (a_1 \dots a_n)$ とすると：

$$
\operatorname{Ran}(A) = \operatorname{span}(a_1, \dotsc, a_n).
$$

連立線形方程式 ${Ax = b}$ の解について、次のように言い換えられる：

* 解の存在性は ${b \in \operatorname{Ran}(A)}$ かどうか
* 一意性は ${\ker(A) \ne \{0\}}$ かどうか

以上
