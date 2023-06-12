---
title: Linear Algebra - Part 26 - Steinitz Exchange Lemma
---

[Linear Algebra - Part 26 - Steinitz Exchange Lemma - YouTube](https://www.youtube.com/watch?v=d69Bw-n5fvo&list=PLBh2i93oe2quLc5zaxD0WHzQTGrXMwAI6&index=26)

**Steinitz Exchange Lemma**:
${U \in \mathbb R^n}$ を部分空間とする。
${\mathcal{B} = (v^{(1)}, \dotsc, v^{(k)})}$ を $U$ の基底とする。
${\mathcal{A} = (a^{(1)}, \dotsc, a^{(l)})}$ を $U$ における線形独立のベクトル族とする。
このとき、$\mathcal{B}$ から ${k - l}$ 個のベクトルを $\mathcal{A}$ に加えて $U$ の新しい基底を得る。

証明：
${l = 1}$ のとき、${\mathcal B \cup \mathcal A}$ は線形従属。
$B$ が基底であるので、一意に与えられるスカラー $\lambda_1, \dotsc, \lambda_k$
が存在して、次を満たす：

$$
a^{(1)} = \lambda_1 v^{(1)} + \dotsb + \lambda_k v^{(k)}.
$$

${\lambda_j \ne 0}$ なる $j$ を一つ選んで（右辺の線形独立性からそうできる）次のようにする：

$$
v^{(j)} = -\frac{1}{\lambda_j}\left(
    \lambda_1 v^{(1)} + \dotsb
    + \lambda_{j - 1}v^{(j - 1)} + \lambda_{j + 1}v^{(j + 1)}
    + \dotsb + \lambda_k v^{(k)}
    - a^{(1)}
\right) \quad \spadesuit
$$

$v^{(j)}$ を $\mathcal B \cup \mathcal A$ から取り除いたものを
$\mathcal C$ とする。

$\mathcal C$ は線形独立であることを示す。

$$
\tilde{\lambda}_1 v^{(1)}
+ \dotsb + \tilde \lambda_{j - 1}v^{(j - 1)}
+ \tilde \lambda_j a^{(1)}
+ \tilde \lambda_{j + 1}v^{(j + 1)}
+ \dotsb + \tilde \lambda_k v^{(k)} = 0
$$

とおく。

${\tilde\lambda_j \ne 0}$ を仮定すると、
$a^{(1)}$ は $v^{(1)}, \dotsc, v^{(j - 1)}, v^{(j + 1)}, \dotsc, v^{(k)}$ の線形結合になるが、
これは先ほどの等式と矛盾する。したがって ${\tilde\lambda_j = 0.}$ である必要がある。

すると、次が成り立つ：

$$
\tilde{\lambda}_1 v^{(1)}
+ \dotsb + \tilde \lambda_{j - 1}v^{(j - 1)}
+ \tilde \lambda_{j + 1}v^{(j + 1)}
+ \dotsb + \tilde \lambda_k v^{(k)} = 0
\implies \tilde \lambda_i = 0.
$$

したがって $C$ は線形独立であるこをが示された。

$\mathcal C$ は $U$ を張る。
${u \in U}$ に対して次を満たすスカラー $\mu_1, \dotsc, \mu_k$ が存在する：

$$
u = \mu_1v^{(1)}
  + \dotsb
  + \mu_{j - 1}v^{(j - 1)}
  + \mu_{j}v^{(j)}
  + \mu_{j + 1}v^{(j + 1)}
  + \dotsb
  + \mu_k v^{(k)}.
$$

これに $\spadesuit$ を代入すると次の形に書ける：

$$
u = \tilde\mu_1v^{(1)}
  + \dotsb
  + \tilde\mu_{j - 1}v^{(j - 1)}
  + \tilde\mu_{j}a^{(1)}
  + \tilde\mu_{j + 1}v^{(j + 1)}
  + \dotsb
  + \tilde\mu_k v^{(k)}.
$$

※これで ${l = 1}$ のときは示された。残りはこの要領で数学的帰納法を用いた証明が続くようだ。

以上
