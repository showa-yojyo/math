---
title: Linear Algebra - Part 3 - Linear Combinations and Inner Products in $\mathbb R^2$
---

[Linear Algebra - Part 3 - Linear Combinations and Inner Products in $\mathbb R^2$ - YouTube](https://www.youtube.com/watch?v=AJPa8Mciq48&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=3)

定義：
ベクトル ${v^{(1)}, \dotsc, v^{(k)} \in \mathbb R}$ とスカラー
$\lambda_1, \dotsc, \lambda_k \in \mathbb R$ に対してベクトル

$$
v = \sum_{j=1}^{k}\lambda_j v^{(j)}
$$

を線形結合という。

質問：ベクトル $u = \begin{pmatrix}2 \\ 1\end{pmatrix}$ に対して垂直な
$v \in \mathbb R^2$ は何か。

プロットにより $v = \begin{pmatrix}-1 \\ 2\end{pmatrix}$ はそのようなベクトルの一つ。
そして、そのスカラー倍もまた垂直だ。これを踏まえて：

回答：ベクトル $u$ と $v$ が直交することと

$$
\begin{pmatrix} v_1 \\ v_2 \end{pmatrix}
= \lambda \begin{pmatrix} -u_2 \\ u_1 \end{pmatrix}
$$

が成り立つ $\lambda \in \mathbb R$ が何かあることは同値。

$$
v1 = -\lambda u_2,\;v_2 = \lambda u_1.
$$

そして $\lambda$ を処理すれば次と同値：

$$
u_1 v_1 + u_2 v_2 = 0.
$$

この左辺を $\left\langle u, v \right\rangle$ を書き、ベクトルの（標準）内積と呼ぶ。

定義：
ベクトル $v$ を直角三角形の斜辺とするような図を書き、
水平成分と垂直成分をそれぞれ $v_1, v_2$ とする。
このベクトルの長さはピタゴラスの定理により

$$
\sqrt{v_1^2 + v_2^2.}
$$

自身との内積の平方根を取った

$$
\lVert v \rVert \coloneqq \sqrt{\left\langle v, v \right\rangle}
$$

を標準ノルムを呼ぶ。

以上
