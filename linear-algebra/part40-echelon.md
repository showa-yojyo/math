---
title: Linear Algebra - Part 40 - Row Echelon Form
video: https://www.youtube.com/watch?v=nRXt9zUNLK4&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=40
---

Row echelon form は正方行列でなくても意味がある概念だ。

$$
\!\begin{pmatrix}
1 & 2 & 0 & 1 & 0\\
0 & 0 & 2 & -1 & 4\\
0 & 0 & 0 & 4 & 8\\
0 & 0 & 0 & 0 & 0\\
\end{pmatrix}\!
$$

なら $1,2,4$ に注目する。

定義：
${m \times n}$ 行列 $A$ が in row echelon form であるとは：

1. すべてゼロの行が（ある場合には）底にある。
2. 各行に対して、最初の非ゼロ要素が上の行の最初の非ゼロ項目より厳密に右側にある。

この最初の要素を pivot という。もちろんどれも非ゼロの値だ。

定義：

$$
\begin{matrix}
x_1 & x_2 & x_3 & x_4 & .
\end{matrix}
\atop
\left(\hspace{-4pt}
\begin{array}{cccc|c}
1 & 3 & 5 & 0 & 1\\
0 & 2 & 0 & 0 & 2\\
0 & 0 & 0 & 3 & 3\\
0 & 0 & 0 & 0 & 0\\
\end{array}
\hspace{-4pt}\right)
$$

* 列に pivot を持たない変数を free variables と呼ぶ ($x_3$)
* 列に pivot を持つ変数を leading variables と呼ぶ ($x_1,x_2,x_4$)

手順：

$$
\begin{aligned}
&Ax = b\\
\longrightarrow &
\left(\hspace{-4pt}
\begin{array}{c|c}
A & b
\end{array}
\hspace{-4pt}\right) \quad \text{augmented matrix}\\
\longrightarrow &
\left(\hspace{-4pt}
\begin{array}{c|c}
A^{\prime} & b^{\prime}
\end{array}
\hspace{-4pt}\right) \quad \text{row echelon form}\\
\longrightarrow&
\text{put free variable to the right-hand side}\\
\longrightarrow&
\text{backwards substitition}\\
\longrightarrow&
\text{solutions}
\end{aligned}
$$

例：

$$
\begin{aligned}

\left(\hspace{-4pt}
\begin{array}{ccccc|c}
1 & 2 & 0 & 1  & 0 & 3\\
0 & 0 & 2 & -1 & 4 & 2\\
0 & 0 & 0 & 4  & 8 & 8\\
0 & 0 & 0 & 0  & 0 & 0\\
\end{array}
\hspace{-4pt}\right)\\

\longrightarrow

\left(\hspace{-4pt}
\begin{array}{ccc|c}
1 & 0 & 1  & 3 - 2x_2\\
0 & 2 & -1 & 2 - 4x_5\\
0 & 0 & 4  & 8 - 8x_5\\
0 & 0 & 0  & 0 \\
\end{array}
\hspace{-4pt}\right)\!

\begin{array}{}
\\
\text{I}\\
\text{II}\\
\text{III}\\
\end{array}\!

\end{aligned}
$$

$$
\text{III} \quad 4x_4 = 8 - 8x_5 \implies x_4 = 2 - 2x_5, x_5 \in \mathbb R.
$$

$$
\text{II} \quad
\begin{aligned}
&2x_3 - x_4 = 2 - 4x_5\\
\implies& 2x_3 - 2 + 2x_5 = 2 - 4 x_5\\
\implies& 2x_3 = 4 - 6x_5\\
\implies& x_3 = 2 - 3x_5.
\end{aligned}
$$

$$
\text{I} \quad
\begin{aligned}
&x_1 + x_4 = 3 - x_2\\
\implies & x_1 + 2 - 2x_5 = 3 - 2x_2\\
\implies & x_1 = 1 - 2x_2 + 2x_5.
\end{aligned}
$$

解の集合：

$$
\begin{aligned}
S &= \!\left\{\left. \!\begin{pmatrix}
1 - 2x_2 + 2x_5\\
x_2\\
2 - 3x_5\\
2 - 2x_5\\
x_5
\end{pmatrix}\!\,\middle|\, x_2,x_5 \in \mathbb R \right.\right\}\!\\
&= \!\left\{\left.
    \!\begin{pmatrix}
    1\\
    0\\
    2\\
    2\\
    0
    \end{pmatrix}\!
    + x_2\!\begin{pmatrix}
    - 2\\
    1\\
    0\\
    0\\
    0
    \end{pmatrix}\!
    + x_5\!\begin{pmatrix}
    2\\
    0\\
    -3\\
    -2\\
    1
    \end{pmatrix}\!
    \,\middle|\, x_2,x_5 \in \mathbb R \right.\right\}\!.
\end{aligned}
$$

以上
