---
title: Linear Algebra - Part 5 - Vector Space $\mathbb R^n$
---

[Linear Algebra - Part 5 - Vector Space $\mathbb R^n$ - YouTube](https://www.youtube.com/watch?v=xT0pxcygvLw&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=5)

${n \in \mathbb N}$ とする。
$\mathbb R^n = \mathbb{R} \times \dotsb \times \mathbb{R}$

ベクトルを成分を縦に並べて書く：

$$
v = \begin{pmatrix}v_1 \\ v_2 \\ \vdots \\ v_n\end{pmatrix}
\in \mathbb{R}^n.
$$

加法：

$$
\def\vec#1{ \begin{pmatrix}{#1}_1 \\ \vdots \\ {#1}_n\end{pmatrix} }
u + v = \vec{u} + \vec{v} \coloneqq
\begin{pmatrix}u_1 + v_1 \\ \vdots \\ u_n + v_n\end{pmatrix}\!.
$$

スカラー倍：

$$
\def\vec#1{ \begin{pmatrix}{#1}_1 \\ \vdots \\ {#1}_n\end{pmatrix} }
\lambda u = \lambda\!\vec{u} \coloneqq \vec{\lambda u}\!.
$$

性質： $\text{(a)}$ $(\mathbb{R}^n, +)$ はアーベル群：
$u,v,w\in\mathbb{R}^n$ とし $0$ を零ベクトルとすると次がいつでも成り立つ：

$$
\begin{aligned}
\text{(1)}&&u + (v + w) &= (u + v) + w\\
\text{(2)}&&v + 0 &= v\\
\text{(3)}&&v + (-v) &= 0\\
\text{(4)}&&v + w &= w + v
\end{aligned}
$$

$\text{(b)}$ スカラー倍は互換：
$\lambda,\mu\in\mathbb R$ とすると次がいつでも成り立つ：

$$
\cdot \colon \mathbb R \times \mathbb R^n \longrightarrow \mathbb R^n.
$$

$$
\begin{aligned}
\text{(5)}&&\lambda (\mu v) &= (\lambda \mu) v\\
\text{(6)}&&1 \cdot v &= v
\end{aligned}
$$

$\text{(c)}$ 分配律：

$$
\begin{aligned}
\text{(7)} && \lambda(v + w) &= \lambda v + \lambda w\\
\text{(8)} && (\lambda + \mu)v &= \lambda v + \mu v\\.
\end{aligned}
$$

正規単位ベクトル：

$$
e_1 = \begin{pmatrix}1 \\ 0 \\ \vdots \\ 0\end{pmatrix},
e_2 = \begin{pmatrix}0 \\ 1 \\ \vdots \\ 0\end{pmatrix},
\dotsc,
e_n = \begin{pmatrix}0 \\ 0 \\ \vdots \\ 1\end{pmatrix}.
$$

任意の $v \in \mathbb R^n$ はこれらの線形結合で書ける：

$$
v = \begin{pmatrix}v_1 \\ \vdots \\ v_n\end{pmatrix} = \sum_{j=1}^{n}v_j e_j.
$$

以上
